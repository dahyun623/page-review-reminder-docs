# Page Review Reminder — Security information

Operator: dahyun kim, Republic of Korea. Security contact: **danielanderic@gmail.com**.

## Application hosting and access

The app runs on Atlassian Forge and uses Confluence APIs and Forge hosted key-value storage. Its application manifest does not configure an external application backend or external network egress. Atlassian supplies the hosting platform protections. The app does not claim its own independent security certification, a completed CAIQ Lite assessment or participation in a security bug bounty program.

The app requires an authenticated Confluence user. It checks record ownership and assigned-reviewer status on the server. Registering users manage their own entries; assigned reviewers can mark accessible assigned entries reviewed. Confluence page access is checked before showing an entry or attempting a reminder. The app does not grant page access or ask end users for Atlassian passwords, API tokens or other shared secrets.

## Stored information and diagnostics

Stored workflow information includes account and page identifiers, review dates and settings, reminder delivery records and privacy-processing metadata. The app retrieves page titles for display but does not store page-body copies or user email addresses in its workflow database.

Application logging is designed around events, aggregate counts and execution states. The diagnostic report is designed to omit page titles, page bodies, account identifiers and email addresses. Customers decide whether to copy a diagnostic report and send it to support; the copy action does not send a message automatically.

## Locations and support

Persistent Forge hosted storage supports Atlassian data residency and follows the host application's supported residency configuration. Hosting, pinning and supported migration are provided by Atlassian. Runtime computation, platform logs, backups and support correspondence should not be assumed to have the same residency scope. See [Atlassian's Forge data residency documentation](https://developer.atlassian.com/platform/forge/data-residency/).

Support email is handled separately in Gmail. Please send only the diagnostic report, a short problem description and the time of the problem. Do not send passwords, tokens, confidential page contents or sensitive personal data. The [Privacy Notice](PRIVACY.md) explains support correspondence and retention.

## Reporting a security issue

Email **danielanderic@gmail.com** with a concise description, affected version, approximate time and safe reproduction steps. Please avoid including other customers' data or performing disruptive tests. Reports are reviewed to investigate and address defects. This document does not promise a fixed response time or resolution deadline.

The [Customer DPA](DPA.md) describes the applicable customer-data incident notification and assistance obligations. The [Terms](TERMS.md) and [Privacy Notice](PRIVACY.md) also apply. This information describes the app's measures and does not establish compliance with every law or certify Atlassian's services independently.
