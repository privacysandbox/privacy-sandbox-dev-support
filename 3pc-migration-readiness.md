# Third-party cookie migration readiness list

The purpose of this page is to consolidate information about how companies across the web are reducing their reliance on third-party cookies. The usefulness of this page depends on participants sharing information and updates.

Note: This page is primarily focused on **non-advertising** use cases such as payments, sign-in and other types of non-advertising services and user features. Companies testing and adopting the Privacy Sandbox relevance and measurement APIs can note their status on the GitHub tester pages for [Protected Audience](https://github.com/WICG/turtledove/blob/main/fledge-tester-list.md), [Topics](https://github.com/patcg-individual-drafts/topics/blob/main/topics-tester-list.md) and [Attribution Reporting](https://github.com/WICG/attribution-reporting-api/blob/main/ara-tester-list.md).

## Disclaimers

* Not a complete list. Participants are strongly encouraged to share their activities and insights publicly for the benefit of the broader community, but sharing is voluntary and therefore this page is not expected to reflect all activity.  
* Not evaluative. Editors will review submissions for relevance and to ensure general conformance to the guidelines above, but are not evaluating or endorsing the information provided.  
* Editors will regularly review and approve submissions that meet the guidelines below. If you believe that there's an error in a submission, please create an issue in the [Privacy Sandbox Developer Support repository](https://github.com/GoogleChromeLabs/privacy-sandbox-dev-support) with the words "\[3PC Migration Readiness List\]" in the subject and the Editors will respond in short order.  
* Some entries may reference third-party cookie “deprecation.” These entries were added prior to the announcement of [a new way forward for Privacy Sandbox on the web](https://privacysandbox.com/news/privacy-sandbox-update/) and are not reflective of Chrome’s [plans for third-party cookies](https://developers.google.com/privacy-sandbox/cookies).

## Guidelines

* Enter information on behalf of your own organization.  
* Do not share detailed information inline; instead, link to other public pages (e.g. your own website, customer notes or other resources).  
* Add entries to the relevant category in the 'Table \- Readiness' section below. If the entry fits into multiple categories, please list them in each relevant category.  
* Table fields:  
  * **Company/Party/Service:** The organization, company, service, or site entering information about their use of third-party cookies. If the service/site is part of a larger company, provide the company name in parentheses. For example: *news.example (ACME), stocks.example (ACME)*  
  * **Status:** A short free-text status update for the entity listed. For example: *Ready for 3PC unavailability, No reliance on 3PCs, Temporary mitigations applied, No known issues, Implementing CHIPS by end Q4 2024*  
  * *(Optional)* **Link to relevant documentation:** Link to blog posts, customer-facing documentation, or other relevant guidance supporting your site/service's plans for reducing 3PC reliance.  
  * *(Optional)* **How to contact you:** Instructions to contact. This may include items such as an email address or a link to a website form.  
  * *(Optional)* **Action required:** True/false to indicate whether or not sites embedding your service need to take action. In the future, this detail may be consumed by Chrome DevTools to help inform top-level sites of any action required to prepare for 3PC changes.  
  * *(Optional)* **Cookie domains:** A comma separated list of domains (or subdomains) used by your service to serve third-party cookies. This detail may be consumed by Chrome DevTools to help inform top-level sites of the status of your 3PC migration. If you do not wish for your entry to be visible to Chrome DevTools users, leave this field blank.

## How to submit

1. On the [Developer Support GitHub page](https://github.com/GoogleChromeLabs/privacy-sandbox-dev-support), navigate to the document in the main table called 3pc-migration-readiness.md (If you can read this sentence then you have already completed this step\!)  
2. Click the pencil icon on the right side to edit the appropriate table below and add your information:  
   1. Use the | to make sure that the information that you provide correctly shows up in each cell  
   2. You may be directed to fork this repo to apply your own changes.  
   3. After you select ‘Propose changes’ an editor will review and publish your updates in the coming days.  
3. You can find additional instructions here for [editing tables in GitHub](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables).

   ## Table \- Migration readiness

### Payments and transactions

*For example: checkout or processing a credit card transaction*

| Company / Party / Service | Status | Link to more information or documentation | How to contact you | Action required | Cookie domains |
| :---- | :---- | :---- | :---- | :---- | :---- |
| [br.clear.sale/](https://br.clear.sale/) | Temporary mitigations applied. No site changes required during the [deprecation trial](https://developers.google.com/privacy-sandbox/3pcd/temporary-exceptions/third-party-deprecation-trial#deprecation_trials), updates may be necessary post-trial. | [Api Documentation](https://api.clearsale.com.br/docs/behavior-analytics) | [contact](mailto:integracao@clear.sale?subject=Behavior&nbsp;3PCD&nbsp;doubts) |  |  |
| <!-- copy this row and insert above this line -->  | <!-- Status goes here -->  | <!-- Add a link to more information -->  | <!-- How can we contact you? -->  | <!-- Do sites using your service need to do anything? True/False --> | <!--comma separated domains that set cookies, like example.com, example.net --> |

### Embedded widgets

*For example: an embedded realtime chat or commenting widget*

| Company / Party / Service | Status | Link to more information or documentation | How to contact you | Action required | Cookie domains |
| :---- | :---- | :---- | :---- | :---- | :---- |
| [tawk.to](https://tawk.to) | No reliance on 3PCs |  |  |  |  |
| <!-- copy this row and insert above this line -->  | <!-- Status goes here -->  | <!-- Add a link to more information -->  | <!-- How can we contact you? -->  | <!-- Do sites using your service need to do anything? True/False --> | <!--comma separated domains that set cookies, like example.com, example.net --> |

### IDP/Sign-In

*For example: single sign-on or social sign-on*

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you | Action required | Cookie domains |
| :---- | :---- | :---- | :---- | :---- | :---- |
| [Sign in with Google for Web](https://developers.google.com/identity/gsi/web/guides/overview) | Ready for 3PCD, sites may require to make updates to adopt changes | [Guide \- Migrate to FedCM](https://developers.google.com/identity/gsi/web/guides/fedcm-migration) | [StackOverflow Space](https://stackoverflow.com/questions/tagged/google-signin) |  |  |
| [Google Identity Services JavaScript library](https://developers.google.com/identity/oauth2/web/guides/overview) | No reliance on 3PCs |  | [StackOverflow Space](https://stackoverflow.com/questions/tagged/google-signin) |  |  |
| [Google Sign-In](https://developers.google.com/identity/sign-in/web/sign-in) | Temporary mitigations applied. No site changes required during the [deprecation trial](https://developers.google.com/privacy-sandbox/3pcd/temporary-exceptions/third-party-deprecation-trial#deprecation_trials). However, updates may be necessary post-trial when the library transitions to new FedCM APIs. | [Google Sign-in with FedCM APIs](https://developers.google.com/identity/sign-in/web/gsi-with-fedcm) | File a [GitHub](https://github.com/google/google-api-javascript-client/issues) issue or use the [google-sign](https://stackoverflow.com/questions/tagged/google-signin) tag on Stack Overflow | True |  |
| [Sec4U \- Authfy](https://www.sec4u.com.br/authfy) | No reliance on 3PCs |  | [Sec4U Website](https://www.sec4u.com.br/) |  |  |
| <!-- copy this row and insert above this line -->  | <!-- Status goes here -->  | <!-- Add a link to more information -->  | <!-- How can we contact you? -->  | <!-- Do sites using your service need to do anything? True/False --> | <!--comma separated domains that set cookies, like example.com, example.net --> |

### Infrastructure

*For example: a CDN or CMS*

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you | Action required | Cookie domains |
| :---- | :---- | :---- | :---- | :---- | :---- |
| <!-- copy this row and insert above this line -->  | <!-- Status goes here -->  | <!-- Add a link to more information -->  | <!-- How can we contact you? -->  | <!-- Do sites using your service need to do anything? True/False --> | <!--comma separated domains that set cookies, like example.com, example.net --> |

### Anti-Fraud and Anti-Abuse

*For example: a security or anti-fraud vendor*

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you | Action required | Cookie domains |
| :---- | :---- | :---- | :---- | :---- | :---- |
| [reCAPTCHA V2](https://developers.google.com/recaptcha/docs/display) | No action needed by sites. Service is compatible with 3PCD. |  | [reCAPTCHA Help Center](https://support.google.com/recaptcha/?hl=en) |  |  |
| [reCAPTCHA V3](https://developers.google.com/recaptcha/docs/v3) | No action needed by sites. Service is compatible with 3PCD. |  | [reCAPTCHA Help Center](https://support.google.com/recaptcha/?hl=en) |  |  |
| [reCAPTCHA Enterprise](https://cloud.google.com/recaptcha-enterprise/docs) | No action needed by sites. Service is compatible with 3PCD. |  | [reCAPTCHA Enterprise Help](https://cloud.google.com/recaptcha-enterprise/docs/getting-support) |  |  |
| [br.clear.sale/](https://br.clear.sale/) | Temporary mitigations applied. No site changes required during the [deprecation trial](https://developers.google.com/privacy-sandbox/3pcd/temporary-exceptions/third-party-deprecation-trial#deprecation_trials), updates may be necessary post-trial. | [Api Documentation](https://api.clearsale.com.br/docs/behavior-analytics) | [contact](mailto:integracao@clear.sale?subject=Behavior&nbsp;3PCD&nbsp;doubts) |  |  |
| <!-- copy this row and insert above this line -->  | <!-- Status goes here -->  | <!-- Add a link to more information -->  | <!-- How can we contact you? -->  | <!-- Do sites using your service need to do anything? True/False --> | <!--comma separated domains that set cookies, like example.com, example.net --> |

### Analytics and Business Tools

*For example: a page analytics or customer experience tool*

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you | Action required | Cookie domains |
| :---- | :---- | :---- | :---- | :---- | :---- |
| [Chartbeat \- Heads Up Display](https://chartbeat.com/products/optimization/) | Temporary mitigations applied with a long-term solution in progress. No site changes are expected to be required. | [HUD Documentation](https://help.chartbeat.com/hc/en-us/sections/201761058-Heads-Up-Display) | [Support](mailto:support@chartbeat.com?subject=hud&nbsp;3PCD) |  |  |
|[Mather Economics](https://www.mathereconomics.com/), <br>[Listener First Party Data Platform](https://www.mathereconomics.com/listener-mathers-data-analytics-platform/), & <br>[Sophi AI](https://www.mathereconomics.com/sophi-start/)  | Prepared for 3PCD. All Mather Economics and Sophi clients will not be impacted. All of Mather Economics products and services use first party data and are integrated directly in collaboration with our clients.  | [Privacy Policy - Mather Economics](https://www.mathereconomics.com/privacy-policy/) <br>[Content Paywall (2.0) (sophi.io)](https://resources.sophi.io/integrations/docs)  | info@mathereconomics.com  |  |  |
| <!-- copy this row and insert above this line -->  | <!-- Status goes here -->  | <!-- Add a link to more information -->  | <!-- How can we contact you? -->  | <!-- Do sites using your service need to do anything? True/False --> | <!--comma separated domains that set cookies, like example.com, example.net --> |

### Other

*Anything that doesn't fit into the above categories*

| Company / Party / Service | State of 3PCD readiness | Link to more information or documentation | How to contact you | Action required | Cookie domains |
| :---- | :---- | :---- | :---- | :---- | :---- |
| [br.clear.sale/](https://br.clear.sale/) | Temporary mitigations applied. No site changes required during the [deprecation trial](https://developers.google.com/privacy-sandbox/3pcd/temporary-exceptions/third-party-deprecation-trial#deprecation_trials), updates may be necessary post-trial. | [Api Documentation](https://api.clearsale.com.br/docs/behavior-analytics) | [contact](mailto:integracao@clear.sale?subject=Behavior%203PC%20doubts) |  |  |
| [Lunio](https://lunio.ai/) | No reliance on 3PCs | [Cookieless Product Overview](https://lunio.ai/product/) | [Support](https://lunio.ai/about-us/contact/) |  |  |
| [WordPress VIP](https://wpvip.com/) & [rtCamp](https://rtcamp.com/) | Prepared for 3PCD and offering audits to help businesses evaluate and understand the impact of third-party cookie deprecation | [WordPress VIP and rtCamp Partner to Help Businesses Adapt to New Web Privacy Standards](https://wpvip.com/2024/02/21/vip-rtcamp-privacy-sandbox/) | [Get your free audit](https://wpvip.com/website-audit-and-cookie-analysis/) |  |  |
| [Plumrocket](https://plumrocket.com/) | Ready for 3PC deprecation. Conducting cookie audits to help businesses identify issues related to 3PC deprecation and adapt to the changes. | [Third-Party Cookie Audit](https://plumrocket.com/blog/privacy-sandbox) | [Get Audit](https://plumrocket.com/contacts) |  |  |
| <!-- copy this row and insert above this line -->  | <!-- Status goes here -->  | <!-- Add a link to more information -->  | <!-- How can we contact you? -->  | <!-- Do sites using your service need to do anything? True/False --> | <!--comma separated domains that set cookies, like example.com, example.net --> |
