# Fibery hard limits

Checked 12 November 2026 against fibery.com and the Fibery user guide. Re-check quarterly; owner: TBD.

How to read the "Effect" column: **Blocker** means the answer is "not a fit" when the visitor requires this. **Caveat** means say it plainly and let the visitor decide. **Info** is a fact to answer with, not a limit.

## Deployment and access

| Topic | Fact | Effect | Source |
|---|---|---|---|
| Offline work | No offline mode. Fibery needs an internet connection. | Blocker | Michael, 12 Nov 2026; listed as an open request on [customer feedback](https://fibery.com/customer-feedback) |
| On-premise / self-hosted | Not offered. Cloud only. | Blocker | [Fibery 101](https://fibery.com/101-questions-about-fibery), "Self-hosting" |
| Open source | Fibery is not open source. (Open-source projects get Fibery free; that is a discount, not source access.) | Blocker | Michael, 12 Nov 2026; [pricing](https://fibery.com/pricing) |
| Blocked regions | Workspaces cannot be accessed from Russia, Belarus, Cuba, Iran, North Korea, Crimea, Sudan and Syria (since 9 Sep 2024). Public spaces and forms still open. | Blocker | [Security](https://fibery.com/security) |
| Hosting | Amazon Web Services. | Info | [Security](https://fibery.com/security) |
| Data location | EU by default. Enterprise plan can choose EU, US, UK or APAC. | Blocker if a non-EU region is required below Enterprise | [Pricing](https://fibery.com/pricing); [Fibery 101](https://fibery.com/101-questions-about-fibery) |
| Latency | Servers are in the EU; in some countries the app can feel slow because of latency. | Caveat | [Troubleshooting](https://the.fibery.io/@public/User_Guide/Guide/Troubleshooting-149) |
| Desktop | Apps for macOS and Windows. Linux works in the browser. | Info | [Download](https://fibery.com/download) |
| Mobile | Native iOS and Android apps exist, for viewing updates, adding notes and keeping work moving. Building and configuring (views, fields, deep editing) is desktop and web first. | Caveat for mobile-first or field teams | [Download](https://fibery.com/download); [CRM: what you get and what you don't](https://the.fibery.io/@public/User_Guide/Guide/What-if-you-manage-CRM-in-Fibery:-what-you-get-and-what-you-don't-524) |
| Interface language | English only. Names of spaces, databases, fields and views can be in any language. The guide suggests a browser translation extension for the rest. | Blocker if a fully translated interface is required | [Localization](https://the.fibery.io/@public/User_Guide/Guide/Localization--151) |

## Compliance and security

| Topic | Fact | Effect | Source |
|---|---|---|---|
| HIPAA | Not HIPAA compliant. Not a good choice for data with medical details. | Blocker | [CRM: what you get and what you don't](https://the.fibery.io/@public/User_Guide/Guide/What-if-you-manage-CRM-in-Fibery:-what-you-get-and-what-you-don't-524) |
| SOC 2 | SOC 2 Type II report by an independent auditor. Copy on request: new@fibery.io. | Info | [Security](https://fibery.com/security) |
| GDPR | Committed to GDPR compliance; Data Processing Agreement and EU model clauses. | Info | [Security](https://fibery.com/security); [GDPR in Fibery](https://the.fibery.io/@public/User_Guide/Guide/GDPR-in-Fibery-65) |
| Deletion | A deleted record stays in the audit log until the whole workspace is deleted. | Caveat for strict erasure rules | [Activity & Trash FAQ](https://the.fibery.io/@public/User_Guide/Guide/Activity-&-Trash-FAQ-535) |
| Encryption | TLS in transit, encrypted at rest. | Info | [Security](https://fibery.com/security) |
| Two-factor login | Not native. Workaround: allow only Google, Microsoft or SAML login and enforce it there. | Caveat | [Authentication methods](https://the.fibery.io/@public/User_Guide/Guide/Authentication-methods-48) |
| SAML SSO, SCIM | Enterprise plan only. | Caveat (Enterprise needs 25+ paid seats) | [Pricing](https://fibery.com/pricing); [Security](https://fibery.com/security) |
| IP allowlist | Available. Plan is unclear: Fibery 101 says Enterprise, the CRM guide says Pro and up. | Info; do not state the plan | [Workspace settings](https://the.fibery.io/@public/User_Guide/Guide/Workspace-settings-62) |
| AI data | Fibery AI runs on Anthropic, OpenAI and Google models; transcription on Deepgram. Customer data is not used for training. Bringing your own AI provider is not supported. | Blocker if own AI provider is required | [Pricing](https://fibery.com/pricing) FAQ |
| Switching AI off | An admin can turn Fibery AI off for the whole workspace (Settings → AI). | Info: a "no AI" policy is not a blocker | [Fibery AI Agent FAQ](https://the.fibery.io/@public/User_Guide/Guide/Fibery-AI-Agent-FAQ-506); Michael, 12 Nov 2026 |
| ISO 27001 | Not held. | Blocker when required | Michael, 12 Nov 2026 |
| Other certificates | FedRAMP, PCI for Fibery itself: not mentioned anywhere on the site. Treat as not held. | Blocker when required | Not found (unverified) |

## Scale

| Topic | Fact | Effect | Source |
|---|---|---|---|
| Records per database | Works well up to about 300,000 entities in one database; 300,000–500,000 is the comfortable ceiling. Beyond that performance is not guaranteed. | Blocker for millions of records per database | [Databases](https://the.fibery.io/@public/User_Guide/Guide/Databases-7) |
| Fields per database | Many fields (around 100) make a database slow. Changing a formula on a large database triggers a long recalculation. | Caveat | Same |
| Databases per workspace | 1,000, counting deleted ones, on every plan. | Caveat | [Spaces](https://the.fibery.io/@public/User_Guide/Guide/Spaces-18) |
| Team size | No limit on the number of users; some customers run several thousand users in one workspace. Free plan: up to 10 users. Enterprise plan: at least 25 paid seats. | Info | Michael, 12 Nov 2026; [Pricing](https://fibery.com/pricing) |
| API rate limits | 3 requests per second per token and 7 requests per second for the whole workspace; above that the API answers 429 "Too Many Requests". Each user can hold 3 API tokens. Fibery says these limits may change. | Caveat for heavy API use | [API authentication](https://developers.fibery.com/guides/getting-started/authentication) |

## Things Fibery is not

Do not present workarounds for these as a fit.

| Need | Fact | Source |
|---|---|---|
| Help desk or service desk portal for customers | Not offered. Fibery can track tickets internally and sync conversations from Intercom, Zendesk or email. | Michael, 12 Nov 2026 |
| Community forum | Not offered. Discourse topics can be synced in. | Michael, 12 Nov 2026 |
| Team chat | Not offered. Slack messages can be synced in. | Michael, 12 Nov 2026 |
| E-signature | Not offered. | Michael, 12 Nov 2026 |
| Own web address or white-labelling | Not offered. The workspace cannot run on the customer's own web address or be rebranded as their product; only the logo and company name can be changed. | User guide, via the customer-requests data, 12 Nov 2026 |
| Branded client portal | Not offered. Clients and freelancers can still log in for free: guests see only the entities shared with them (at most 10 per guest on Free, 25 on Standard, 100 on Pro, 250 on Enterprise) and cannot be invited into spaces; observers can read whole spaces but not edit. | [User roles](https://the.fibery.io/@public/User_Guide/Guide/User-Roles-494); [Permissions: use cases](https://the.fibery.io/@public/User_Guide/Guide/Permissions:-some-use-cases-and-examples-430); [Pricing](https://fibery.com/pricing) |
| Live database behind a website or app | Not what Fibery is designed for: it manages processes and is not built to serve site traffic. A site can write to Fibery through the API. | Michael, pre-sales chat, 2026 |

## Smaller gaps worth admitting

- Integrations sync one way, into Fibery. The only true two-way sync is Jira. See `integrations.md`.
- The only ready-made calendar sync is Google Calendar.
- A template can be installed into other workspaces, but later changes to it cannot be pushed out to them. Each workspace is separate and has its own subscription.
- Approval steps are not built in; they are modelled as a status that a person changes.
- Fibery AI works on demand and as a step inside automations. It is not a set of autonomous agents running in the background. Outside agents connect through the MCP server.
- No built-in recurring tasks or follow-up reminders; both are built with automation rules.
- No built-in timer for time tracking; hours are logged in a field, a timer is built with buttons or a custom app.
- People outside the workspace cannot comment on a publicly shared document.
- Live chat support follows European business hours.
- Fibery has a learning curve for people who change the workspace. The first version does not have to be built by hand: Fibery AI builds it from a description in a couple of minutes ([Fibery 101](https://fibery.com/101-questions-about-fibery)).

The four gaps above about calendars, templates, approvals and AI come from answers the Fibery team gave in pre-sales chats in 2026.

## Not published, so say "I don't know"

Uptime SLA, backup retention, penetration tests, right-to-left interface support.
