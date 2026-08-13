# n8n Workflow Export

Place the **sanitized public export** of the latest CCS Factory Operations n8n workflow in this directory.

Recommended filename:

`CCS_Stores_AI_Factory_Operations_Assistant_PUBLIC.json`

Before committing an export, remove or replace:

- credential IDs and credential names that expose private setup details
- API keys / tokens
- webhook IDs and production webhook URLs
- Google Spreadsheet IDs and production URLs
- WhatsApp tokens / phone-number IDs
- private customer or supplier data
- instance-specific identifiers that are not required for a public template

Use placeholders such as:

- `YOUR_GOOGLE_SHEET_ID`
- `YOUR_WHATSAPP_CREDENTIAL`
- `YOUR_WEBHOOK_URL`

Then import the sanitized file into a clean n8n instance and verify that it still loads correctly before publishing.
