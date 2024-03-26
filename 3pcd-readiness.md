# Third-party cookie deprecation (3PCD) readiness list

The purpose of this page is to consolidate information about how companies across the web are preparing for third-party cookie deprecation. The usefulness of this page depends on participants sharing information and updates.

Note: This page is primarily focused on **non-advertising** use cases such as payments, sign-in and other types of non-advertising services and user features. Companies testing and adopting the Privacy Sandbox relevance and measurement APIs can note their status on the GitHub tester pages for [Protected Audience](https://github.com/WICG/turtledove/blob/main/fledge-tester-list.md), [Topics](https://github.com/patcg-individual-drafts/topics/blob/main/topics-tester-list.md) and [Attribution Reporting](https://github.com/WICG/attribution-reporting-api/blob/main/ara-tester-list.md).

## Disclaimers

*   Not a complete list. Participants are strongly encouraged to share their activities and insights publicly for the benefit of the broader community, but sharing is voluntary and therefore this page is not expected to reflect all activity.
*   Not evaluative. Editors will review submissions for relevance and to ensure general conformance to the guidelines above, but are not evaluating or endorsing the information provided.
*   Editors will regularly review and approve submissions that meet the guidelines below. If you believe that there's an error in a submission, please create an issue in the [Privacy Sandbox Developer Support repository](https://github.com/GoogleChromeLabs/privacy-sandbox-dev-support) with the words "[3PCD Readiness List]" in the subject and the Editors will respond in short order.

## Guidelines

*   Enter information on behalf of your own organization.
*   Do not share detailed information inline; instead, link to other public pages (e.g. your own website, customer notes or other resources).
*   Add entries to the relevant category in the 'Table - Readiness' section below. If the entry fits into multiple categories, please list them in each relevant category.
*   Table fields:
    *   **Company/Party/Service**: The organization, company, service, or site entering information about their 3PCD readiness. If the service/site is part of a larger company, provide the company name in parentheses. For example: _news.example (ACME), stocks.example (ACME)_
    *   **Status**: A short free-text status update for the entity listed. For example: _Ready for 3PCD, No reliance on 3PCs, Temporary mitigations applied, No known issues, Implementing CHIPS by June 1, 2024_
    *   _(Optional)_ **Link to relevant documentation**: Link to blog posts, customer-facing documentation, or other relevant guidance supporting your site/service's 3PCD readiness.
    *   _(Optional)_ **How to contact you**: Instructions to contact. This may include items such as an email address or a link to a website form.

## How to submit

1. On the [Developer Support GitHub page](https://github.com/GoogleChromeLabs/privacy-sandbox-dev-support), navigate to the document in the main table called 3pcd-readiness.md (If you can read this sentence then you have already completed this step!)
2. Click the pencil icon on the right side to edit the appropriate table below and add your information:
    1. Use the `|` to make sure that the information that you provide correctly shows up in each cell
    2. After you select 'Propose changes' an editor will review and publish your updates in the coming days.

You can find additional instructions here for [editing tables in GitHub](https://docs.github.com/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables).

## Table - Readiness

### Payments and transactions

_For example: checkout or processing a credit card transaction_

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you |
|---|---|---|---|
| [br.clear.sale/](https://br.clear.sale/)  | Temporary mitigations applied. No site changes required during the [deprecation trial](https://developers.google.com/privacy-sandbox/3pcd/temporary-exceptions/third-party-deprecation-trial#deprecation_trials), updates may be necessary post-trial.  | [Api Documentation](https://api.clearsale.com.br/docs/behavior-analytics)  | [contact](mailto:integracao@clear.sale?subject=Behavior&nbsp;3PCD&nbsp;doubts) | 
| <!-- copy this row -->  | <!-- insert it above this line -->  | <!-- fill in your info -->  | <!-- submit the request -->  | 

### Embedded widgets

_For example: an embedded realtime chat or commenting widget_

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you |
|---|---|---|---|
| [tawk.to](https://tawk.to)  | No reliance on 3PCs  | <!--  -->  | <!-- - -->  | 
| <!-- copy this row -->  | <!-- insert it above this line -->  | <!-- fill in your info -->  | <!-- submit the request -->  | 

### IDP/Sign-In

_For example: single sign-on or social sign-on_

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you |
|---|---|---|---|
| [Sign in with Google for Web](https://developers.google.com/identity/gsi/web/guides/overview)  | Ready for 3PCD, sites may require to make updates to adopt changes  | [Guide - Migrate to FedCM](https://developers.google.com/identity/gsi/web/guides/fedcm-migration) | [StackOverflow Space](https://stackoverflow.com/questions/tagged/google-signin) |
| [Google Identity Services JavaScript library](https://developers.google.com/identity/oauth2/web/guides/overview)  | No reliance on 3PCs  | | [StackOverflow Space](https://stackoverflow.com/questions/tagged/google-signin) |
| [Google Sign-In](https://developers.google.com/identity/sign-in/web/sign-in) | Temporary mitigations applied. No site changes required during the [deprecation trial](https://developers.google.com/privacy-sandbox/3pcd/temporary-exceptions/third-party-deprecation-trial#deprecation_trials), updates may be necessary post-trial. | [Deprecation and Sunset](https://developers.google.com/identity/sign-in/web/deprecation-and-sunset) | File a [GitHub](https://github.com/google/google-api-javascript-client/issues) issue or use the [google-sign](https://stackoverflow.com/questions/tagged/google-signin) tag on Stack Overflow | 
| [Sec4U - Authfy](https://www.sec4u.com.br/authfy)  | No reliance on 3PCs  | <!-- fill in your info -->  | [Sec4U Website](https://www.sec4u.com.br/)  | 
| <!-- copy this row -->  | <!-- insert it above this line -->  | <!-- fill in your info -->  | <!-- submit the request -->  | 

### Infrastructure

_For example: a CDN or CMS_

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you |
|---|---|---|---|
| <!-- copy this row -->  | <!-- insert it above this line -->  | <!-- fill in your info -->  | <!-- submit the request -->  | 

### Other

_Anything that doesn't fit into the above categories_

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you |
|---|---|---|---|
| [br.clear.sale/](https://br.clear.sale/)  | Temporary mitigations applied. No site changes required during the [deprecation trial](https://developers.google.com/privacy-sandbox/3pcd/temporary-exceptions/third-party-deprecation-trial#deprecation_trials), updates may be necessary post-trial.  | [Api Documentation](https://api.clearsale.com.br/docs/behavior-analytics) | [contact](mailto:integracao@clear.sale?subject=Behavior&nbsp;3PCD&nbsp;doubts) | 
| [Lunio](https://lunio.ai/) | No reliance on 3PCs | [Cookieless Product Overview](https://lunio.ai/product/) | [Support](https://lunio.ai/about-us/contact/) |
| <!-- copy this row -->  | <!-- insert it above this line -->  | <!-- fill in your info -->  | <!-- submit the request -->  | 
