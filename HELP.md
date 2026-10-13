# Page Review Reminder — User guide

This guide describes the Confluence Cloud app. Availability depends on your administrator's installation and your page permissions.

## Register a review

Open **Apps → Page Review Reminder** in Confluence. Copy the numeric page ID from a page URL, enter it in **Confluence page ID**, choose the interval in days, and select **Register / update interval**. You must already have access to the page. Each registering user can track up to 100 entries.

The registering user manages the entry's interval, assigned reviewer, pause state, removal, and optional comment reminders. Removing an entry does not delete the Confluence page.

## Assign and complete a review

Choose a person in **Reviewer** and save the reviewer/reminder settings. Check the person's profile when names are identical. Confluence may not return email-address searches. The reviewer must be able to access the page.

Assigned reviewers see accessible entries labeled **Assigned to me**. Select **Mark reviewed** after completing the review. The app records completion and calculates the next review date from the configured interval. Assigned reviewers cannot change another registering user's settings, pause their entry, or remove it.

If a document is missing, first check that you can open its original Confluence page and that the registering user has assigned it to you. Losing page access also hides the app entry. The app does not grant access to pages.

## Optional comment reminders

Comment reminders are off by default. The registering user can enable them separately for each entry. Daily server checks look for overdue entries and check the registering user's and reviewer's page access before attempting a comment mentioning the reviewer.

Your computer does not need to stay on. Checks do not run at a guaranteed minute, and immediate notification at the due time is not promised. Email or push delivery depends on Confluence settings; the app does not send email directly.

The app keeps delivery records to limit duplicate reminders. Some definite failures can be scheduled for retry; uncertain delivery is not automatically retried because a comment may already exist.

## Language and dates

Use **English / 한국어** to change the interface language. English dates show UTC; Korean dates show Korea time. The page title and reviewer name remain in their original language.

## Support and diagnostic reports

Use **Copy diagnostics** in the support panel, then paste the report into your message to **danielanderic@gmail.com**. Include when the problem happened and which action you attempted. The button does not send anything automatically.

The diagnostic report is designed to omit page titles, page bodies, account IDs and email addresses. Do not send passwords, API tokens, confidential page content or sensitive personal information. Support correspondence is handled separately from the app's Forge storage, as explained in the [Privacy Notice](PRIVACY.md).

## Delete your app records

Under **My app data**, read the scope, check the confirmation box, and select **Delete my app records** only when you want to remove your stored entries and delivery records and clear your reviewer assignments on other entries. The app cannot undo this deletion. Original Confluence pages and existing comments remain under your Confluence controls.

For verified privacy or data-return requests, contact **danielanderic@gmail.com**. See the [Privacy Notice](PRIVACY.md), [Customer DPA](DPA.md), and [Terms](TERMS.md).
