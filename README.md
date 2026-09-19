# SORT Privacy Notice

## 1. Responsible company and privacy contact

SORT is operated by:

**GoodBytz GmbH**  
Werner-Otto-Straße 13 g  
22179 Hamburg, Germany

**Privacy and data protection officer contact:**  
Leon Weber  
[leon.weber@goodbytz.com](mailto:leon.weber@goodbytz.com)

This notice explains how GoodBytz GmbH processes information through SORT during designated customer-support cases and troubleshooting sessions. It concerns employees using SORT and other people whose information may appear in those sessions, including callers and customer contacts.

## 2. What SORT collects

SORT combines screen video with a structured timeline of support activity.

### Screen video

During an active recording, SORT records the screen, window or tab selected in Chrome’s sharing dialog. **SORT does not record audio.**

The video can contain whatever is visible in the selected source, including a caller’s name in a hotline widget, customer-associated system numbers and information about the employee carrying out the work.

### Structured timeline

During an active recording, SORT can collect:

- Clicks, scrolling, keyboard interaction information and descriptions of interface elements.
- Entered or committed field values.
- Page titles, URLs, navigation and tab changes.
- Network-request information and WebSocket message payloads.
- Recording identifiers, timestamps, system identifiers, support-ticket associations and information identifying the recording operator.

**The structured timeline can include activity in browser tabs beyond the screen, window or tab selected for video.** Choosing a particular video source does not limit structured collection to that source. WebSocket payloads can also contain information that is not visibly displayed on screen.

Password-type input values are masked in structured capture, but this is not comprehensive redaction. Information in other fields, messages or visible screen content may still be recorded. Employees must avoid unrelated personal or sensitive material during recording.

A numeric system identifier is not necessarily anonymous: it may be possible to associate it with a customer or installation using other company records.

### Operator and upload information

The upload server’s recording listing displays an incrementing number ID, file size, timestamp and assigned ticket ID. It does not display an uploader name or personal ID.

Separately, the uploaded recording bundle contains the recording operator’s configured Sipgate name in its recording metadata. This identifies the person who made the recording, not necessarily whoever later uploaded the file. The absence of a name in the server listing therefore does not make the recording anonymous.

### Configuration and credentials

SORT processes configuration information including the operator’s Sipgate name, Odoo account email, Odoo API key and shared call-state token. Credentials are stored in the local Chrome profile without additional application-level encryption and used to communicate with the relevant services. SORT does not synchronize these settings using Chrome Sync.

Call-state information is used to detect relevant calls and trigger the recording flow. Odoo is used to look up and associate support tickets with recordings.

### Diagnostics

SORT maintains local diagnostic information for troubleshooting. Diagnostic logs use restricted, sanitized fields and are separate from the full recordings. An exported diagnostic file should still be checked before sharing. Full recordings do not receive the same sanitization as diagnostic logs.

## 3. Why information is used

GoodBytz GmbH uses SORT recordings for:

1. **Customer support:** documenting and resolving designated support cases and troubleshooting sessions.
2. **Product improvement:** debugging and improving goodBytz products.
3. **Support quality:** reviewing case quality, providing individual coaching and improving team processes.
4. **AI development:** training, fine-tuning or evaluating AI models using reviewed, de-identified extracts from the structured timeline.

Recording is required for designated support cases or troubleshooting sessions, rather than for all employee activity.

The stated quality-review purposes do not include automated employee scoring or use for pay, promotion or disciplinary decisions. Any proposed change to the purposes or data practices requires assessment and appropriate updated disclosure before it is introduced.

## 4. How information is used for AI development

**Video is not used for AI development.** Only structured timeline extracts are used.

A person reviews the timeline and removes identifying information before an extract is used on company-controlled AI systems. This review must account for identifying information in fields, URLs, payloads and contextual details, not just visible names.

De-identification reduces identifying information but does not automatically make an extract anonymous. Information that can still be associated with a person remains subject to applicable data-protection requirements.

AI timeline extracts are deleted one month after the original recording date. Deletion of an extract does not automatically remove its influence from a model already trained using it.

## 5. Who can access recordings and where they are stored

Access is limited to authorized personnel according to their responsibilities. This includes the employee who made the recording, support or service staff, engineering or AI staff, and team leads or management. AI-development use is limited to the reviewed, de-identified timeline extracts described above.

Uploaded recordings are stored on the company upload server. **Odoo stores a link to the recording, not a copy of its video or structured timeline.**

The upload server, Odoo and company-controlled AI-processing systems are hosted in Germany. This statement concerns those systems, not the separate GitHub Pages website used to publish this notice.

## 6. Retention and deletion

| Information | Retention and deletion |
| --- | --- |
| Uploaded video and structured timeline | Automatically deleted from the upload server one month after the original recording date. Recordings are not included in server backups. |
| De-identified timeline extracts used for AI development | Deleted one month after the original recording date. |
| Recording link in Odoo | Automatically removed when the associated recording is deleted. |
| Recordings stored locally in Chrome and exported files | Employees must delete these within one month of the recording date under the company retention policy. This is a manual obligation, not automatic deletion by SORT. |

The one-month period runs from the **recording date**, not from upload or closure of the support ticket.

These rules cover recordings, AI extracts and recording links. They do not mean that the underlying support ticket, a trained model or separately created work records are deleted at the same time.

Saved credentials are separate from recordings. SORT’s **Remove saved tokens** action removes the locally saved Odoo API key and shared call-state token. Removing a local token does not revoke it at the corresponding service.

## 7. Disclosure and recording controls

Before distributing the installation link and required access credentials, GoodBytz provides employees with the disclosure and this notice by email and requests an explicit acknowledgment. The acknowledgment is retained with the notice version and date. It is separate from recording-upload metadata.

The acknowledgment confirms receipt and understanding of the disclosed practices. It does not, by itself, establish freely given GDPR consent for mandatory workplace processing.

SORT does not require a separate privacy acknowledgment before every recording. An operator may start recording manually, or a relevant call may trigger the recording flow. Chrome’s sharing dialog is used to choose the video source.

**Cancelling the sharing dialog cancels both video recording and timeline collection.** Operators can stop an active recording through SORT or Chrome’s stop-sharing control. These technical controls do not change the company requirement to record designated work activities.

## 8. Access and transport safeguards

The company VPN is mandatory for the work environment: users cannot access the basic work functions without it.

Recording uploads use an HTTP endpoint through that VPN. The upload endpoint itself does not use HTTPS. This notice does not claim that SORT independently detects or enforces VPN connectivity, or that the connection is encrypted end-to-end beyond the VPN termination point.

Access controls, credential handling, human review of AI extracts and the deletion practices described in this notice form part of the company’s handling of recording data. No masking or review process should be treated as a guarantee that recordings cannot contain personal or confidential information.

## 9. Hosting of this privacy notice

This notice is intended for publication on **GitHub Pages**. GitHub hosts the public notice; SORT recordings and AI datasets are not uploaded to GitHub as part of that hosting arrangement.

GitHub states that it logs and stores the IP addresses of GitHub Pages visitors for security purposes, whether or not they are signed in. The statement that SORT’s recording and AI systems are hosted in Germany does not extend to GitHub’s handling of website access information.

Further information is available in [GitHub’s explanation of GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages) and the [GitHub General Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## 10. Your privacy rights and requests

You can contact Leon Weber at [leon.weber@goodbytz.com](mailto:leon.weber@goodbytz.com) with questions or to request access to your personal data, correction, deletion, restriction of processing, data portability or to object to processing. The availability and scope of these rights depend on the applicable legal basis and circumstances.

GoodBytz has an established process for handling relevant requests across server recordings, local copies, Odoo and AI timeline extracts.

If a particular processing activity relies on valid consent, you may withdraw that consent for future processing. Withdrawal does not affect the lawfulness of processing carried out before withdrawal. This does not mean that all SORT processing relies on consent.

You also have the right to lodge a complaint with a competent data-protection supervisory authority, including the authority in the EU Member State of your habitual residence, place of work or the alleged infringement.

## 11. Changes to this notice

GoodBytz will update this notice when relevant practices change. Material changes to collection or use will be prominently communicated before the changed practices are applied, with any further agreement obtained where required. A previous acknowledgment does not authorize undisclosed future uses.

The version of the notice provided with the pre-install disclosure identifies the practices presented to the employee at that time.
