# Documentation details

The OCDS `documentations` block, which is used widely through the different sections of the standard, provides a means to link out to externally hosted documents. However, some publishers have more detailed information about these documents.
This extension describes a way to:

* Indicate document's specific page numbers
* Describe any additional arrangements required to access the document or find the relevant information
* Record the author of the document

Indicating the specific pages where information is found supports quality assurance of disclosure.

Describing `accessDetails` for a document ensures, even when documents are only accessible through attendance at a location (for example), that users can find how to discover them - and also ensures that auditors can check documents that have been made accessible in the appropriate ways.

Recording the `author` of a document is important for checking whether there are potential conflicts of interest to be aware of: for example, when the author of a feasibility study is later involved in the team submitting a bid.

## Example

```json
{
  "documents": [
    {
      "id": "1",
      "documentType": "equityTransferCaps",
      "title": "Equity transfer cap terms",
      "description": "No equity transfer is permitted until construction is completed. See document for more details.",
      "url": "http://example.com/ppp_unit/documents/contracts/4g_network_signed_contract.pdf",
      "pageStart": "334",
      "pageEnd": "336",
      "accessDetails": "You must register for document access via the following url: http://example.com/ppp_unit/registration/",
      "author": "Contract department, PPP unit"
    }
  ]
}
```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.

## Changelog

### 2019-07-24

* Remove references to core fields from README.md

### 2019-01-30

* Remove obsolete `mergeStrategy` properties
