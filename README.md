# Apps Script -> Node

A migration guide for moving scripts from Apps Script to Node on GCP.

## Why?

Node as dozens of benefits over Apps Script. On the other hand, we can't just abandon existing Apps Script users. This provides a guide for migrating to Node.

## Core Features

| Feature | Node | Apps Script |
|-|-|-|
|Runtime|V8|Rhino|
|Library System|npm|custom library|
|Open Source|open|closed|
|Platform|Run anywhere|Run on Google Apps Script|
|OAuth|Hard|Easy, no code|
|Hosting|Anywhere that can run Node|Google – US|
|Quotas|Can be handled by user|Fail script|
|G Suite Events|Not possible|Custom event handlers|
|Multi-login|Possible|Not possible|
|Google APIs|Node Client Library|Advanced Services|
|G Suite Sidebar Add-ons|Not possible|Possible – HtmlService|
|Hangouts Chat Bots|HTTP/PubSub|Function + Deployment|
|Web Apps|App Engine|Deploy as Web App|
|API|App Engine/GCF|Deploy as API|
|Tools|npm tools/bash|Apps Script API|
|Billing|API quotas|free but with quotas|
|Quota|Flexible paid|Free w/ hard limits|
|Publishing|npm|G Suite Marketplace|
|Code editor|any editor|script.google.com|
|Management UI|Cloud Console|script.google.com|

## Services

Apps Script has 3 sets of services for computation.

- **G Suite services**: Access APIs like Drive, Gmail, Calendar, Docs, Sheets, and others.
- **Advanced Google services**: Access Google APIs via their REST API.
- **Script services**: Utilities like logging, HTML, and caching.

### G Suite Services

- Calendar
- Contacts
- Data Studio
- Document
- Drive
- Forms
- Gmail
- Group
- Groups
- Language
- Maps
- Sites
- Slides
- Spreadsheet

### Advanced Services

- Admin SDK (Directory/License/Groups Migration/Groups Settings/Reseller/Reports)
- AdSense
- BigQuery
- Calendar
- Classroom
- DoubleClick
- Drive (Drive/Activity)
- Gmail
- G+
- Mirror
- People
- Sheets
- Shopping Content
- Slides
- Tasks
- Tag Manager
- YouTube (Data, Analytics, Content ID)

### Script Services

- Base (Browser, Logger, Session, console, Blob, User)
- Add-on: Menu, Prompt, Ui, 
- CacheService (Ducment/Script/User Cache)
- CardService
- Charts
- ContentService
- HtmlService
- JDBC
- LockService
- MailApp
- LinearOptimizationService
- PropertiesService
- ScriptApp
- *TriggerBuilder
- UrlFetchApp
- Utilities
- XmlService