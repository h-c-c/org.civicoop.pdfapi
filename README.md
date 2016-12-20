# org.civicoop.pdfapi
PDF API for CiviCRM to create a PDF file and send it to a specified e-mail address.
This is usefull for automatic generation of letters

The entity for the PDF API is Pdf and the action is Create.
Parameters for the api are specified below:
- contact_id: list of contacts IDs to create the PDF Letter (separated by ",")
- template_id: ID of the message template which will be used in the API. _You have to enter the text in the HTML part of the template and select PDF Page format_
- to_email: e-mail address where the pdf file is send to
- pdf_format_id: (optional) ID of the PDF format, is not especified the default PDF format is used

*NEW* Parameters added for use with the giftcard-dev branch of CiviDiscount

This giftcard-dev branch is a dependency of: https://github.com/h-c-c/org.civicrm.module.cividiscount/tree/giftcard-dev

- message_text: appears in email body.
- giftcard_id: gift card code that can be redeemed.
- giftcard_amount: gift card amount, for displaying to the recipient. 

