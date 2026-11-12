# What Fibery can and cannot do

Checked 12 November 2026. Sources: the feature pages at [fibery.com/features](https://fibery.com/features) (F), [Fibery 101](https://fibery.com/101-questions-about-fibery) (101), the [pricing page](https://fibery.com/pricing) (P), the user guide (G), and the list of things customers ask for that Fibery lacks, checked against the guide (R).

## How to use this file

Look up the capability the visitor needs and let its status drive the verdict.

| Status | Meaning | Verdict for that need |
|---|---|---|
| Built in | Works as a standard feature | Fits |
| With limits | Works, but a named part is missing | Fits with caveats; say the limit |
| Via automation | Not a feature of its own; built from automation rules | Fits; say how it is done |
| Via custom app | Built as a custom app with AI, on the Pro plan | Fits; say it is a custom app |
| Not available | Fibery does not do this | Not a fit for that need |

If a capability is not in this file or the other reference files, say "I don't know" and point to the support chat. Do not guess from the name of a feature.

One name to watch: the feature page called "Custom domain" is about modelling your own data structure. It is not about a web address. A visitor who asks for a "custom domain" almost always means their own web address, which is not available (see "Access and sharing").

## Data model

| Capability | Status | Notes and limits |
|---|---|---|
| Your own databases, fields and relations, for any process | Built in | One-to-one, one-to-many, many-to-many and self-relations (task and sub-task). About 300,000 records per database works well; 1,000 databases per workspace. (F, 101, G) |
| Field types | Built in | Text, number, date, single and multi select, workflow states, people, files, location, URL, email, phone, checkbox, rich text, documents, lookup, formula. (101) |
| Formulas across linked records | Built in | Totals, averages, progress, cycle time, revenue metrics, calculated through relations. AI can write them. These are fields on a record, not spreadsheet cells. (F, 101) |
| Properties on a relation itself | Not available | Modelled with an extra linking database. (R, not confirmed in the guide) |
| Process templates | Built in | More than 20 from the Fibery team; you can share your own space as a template. Later changes to a template cannot be pushed to workspaces that installed it. (F) |
| Import | Built in | CSV and Markdown files, plus importers for Trello, Asana, Jira, Airtable, ClickUp and Notion. (F, G) |
| Export and backup | With limits | An admin can export the whole workspace as Markdown, CSV and files. There are no scheduled automatic backups. (101, R) |
| Record templates and recurring records | Via automation | Scheduled rules create them. There is no built-in recurrence setting or template picker. (R) |

## Views and planning

| Capability | Status | Notes and limits |
|---|---|---|
| Table | With limits | Spreadsheet-style editing with batch paste, pinned columns, filters, sorting, colours. No per-cell formulas and limited group totals. (F, R) |
| Board, list, calendar, gallery, feed, map | Built in | Board groups by rows and columns; list shows a hierarchy of any depth; calendar has month, week and day. (F) |
| Timeline (roadmap) | With limits | Lanes, milestones, several databases on one timeline. Weekends can be skipped, but there are no holiday calendars and no scheduling by hour or minute. (F, R) |
| Gantt and dependencies | Built in | Planned dates and dependencies between items; dates shift automatically when a linked card is moved. Critical path is not documented, so do not claim it. (F) |
| Smart folders | Built in | Filtered lists in the sidebar and inside records, such as tasks under their project. (F) |
| Forms | With limits | A form for any database, shared by link or QR code; each submission creates a record. No conditional questions, no multi-page forms, no editing of existing records, no sign-in. Fibery branding is removed on Pro. (F, G, R) |
| Advanced forms | Via custom app | A multi-step form with conditional fields is a typical custom app. See `custom-apps.md`. |
| Charts and reports | Built in | Bar, stacked bar, line, area, stacked area, scatter, tables, annotations; burn-up and cumulative flow from history. Historical data needs Pro. Time spent in each state needs a formula or automation workaround. (F, P, R) |
| Dashboards | Built in | Views and charts arranged on one page, at the top level or inside a record such as a project. (F) |
| Whiteboards | Built in | Diagrams, mind maps, journey maps; items can link to real records. Private only on the Free plan. (F, P) |
| PDF export and printing | With limits | Documents export to Markdown. PDFs are produced only through automation buttons with templates. Reports export as an image or print. (R) |
| Presentation mode (slides) | Not available | Dashboards and shared views only. (R, not confirmed in the guide) |
| A screen laid out your own way | Via custom app | See `custom-apps.md`. |

## Documents and knowledge

| Capability | Status | Notes and limits |
|---|---|---|
| Collaborative documents | Built in | Real-time editing, comments, mentions, embeds (video, Figma, Miro, live Fibery views), nested documents, turning text into tasks. (F) |
| Wiki | Built in | Nested documents or a database of documents. (101) |
| Linking text to records | Built in | Highlight text and link it to an idea, feature or task; the record shows the quote as a backlink. (F) |
| Search | Built in | Full-text across names, documents, rich text and comments, with filters. AI search by meaning covers 10 databases on Standard and all of them on Pro. (F, P) |
| History and restore | Built in | Record history, document version history with restore, an activity log that can restore deleted items. Kept 14 days on Free, 90 days on Standard, without limit on Pro. (F, P) |

## Access and sharing

| Capability | Status | Notes and limits |
|---|---|---|
| Access by space, database and single record | Built in | Four levels on a space: creator, editor, contributor, viewer. (F, G) |
| User groups and custom access rules | Built in | Pro plan. (F, P) |
| Each person sees only their own records | With limits | Possible through record sharing, automatic sharing with the creator or assignee, and hiding spaces from admins (Pro and Enterprise), but the set-up is involved. (R) |
| Hiding some fields of a record from people who can see it | Not available | No field-level permissions. The workaround is a separate linked database with tighter access. (R) |
| Free guests and read-only observers | Built in | Limits on shared items per guest are in `pricing.md`. (P) |
| Public links | With limits | Documents, records, reports, forms and whole spaces; links never expire. Always read-only: outside people cannot comment, vote or have accounts. (F, G, R) |
| Public ideas portal with voting | Not available | A space or view can be published read-only and a form can collect ideas. (R) |
| Your own web address or a white-labelled product | Not available | Only the logo and company name can be changed. (R) |

## Automation

| Capability | Status | Notes and limits |
|---|---|---|
| Rules and buttons | Built in | Rules run on an event or a schedule; buttons run on a click. Monthly run limits by plan are in `pricing.md`. (F, 101) |
| Actions | Built in | Create, update and link records, notify people, send email, post to Slack, call another system over the web. (101, G) |
| Scripts | Built in | JavaScript in automations, Pro plan. If/then branching and loops need a script. (P, R) |
| AI steps | Built in | Summarise, classify, extract, translate inside a rule; uses AI credits. (101) |
| Reminders and due-date notifications | Via automation | Scheduled rules send them. No built-in reminder or snooze. (R) |
| Approval steps | Via automation | States, buttons and validation rules. No built-in approval object. (R) |

## AI

| Capability | Status | Notes and limits |
|---|---|---|
| Building a workspace from a description | Built in | Databases, relations, fields and views in a couple of minutes. (101) |
| Asking questions about your data and changing it | Built in | Uses AI credits; paid plans. (101, P) |
| Writing help in documents | Built in | Summarise, rewrite, draft, translate. (101) |
| Call transcription | Built in | Hours per month by plan. (P) |
| Connecting your own AI assistant | Built in | MCP server with more than 50 tools, on every plan; Claude, ChatGPT and others. (F, P) |
| Connectors built by AI | Built in | Beta. See `integrations.md`. |
| Custom apps | Built in | Pro plan. See `custom-apps.md`. |
| Autonomous agents working in the background | Not available | Not released. (F) |
| Your own model for the built-in AI | Not available | Outside agents that use your own model can connect through the MCP server. (R) |
| Switching AI off | Built in | An admin can turn it off for the workspace. (G) |

## Integrations and other apps

Details are in `integrations.md`. The points that most often decide a verdict:

| Capability | Status | Notes and limits |
|---|---|---|
| Syncing data in from other tools | Built in | More than 20 ready-made integrations. One way, into Fibery. (F, G) |
| Two-way sync | With limits | Jira only, for some fields. Everything else needs an automation, a custom action or a third-party sync service. (G, R) |
| Calendars | With limits | Google Calendar, one way. No Outlook calendar and no iCal feed. (G, R) |
| Email | With limits | Gmail, Outlook and IMAP sync in; emails can be sent and replied to from Fibery. It is not a shared inbox client. (G, R) |
| Microsoft 365 | With limits | Outlook mail and Microsoft sign-in. No Teams or OneDrive integration. (R) |
| Messengers other than Slack | Not available | Telegram, WhatsApp and Discord only through web requests or an automation platform. (R) |
| API and webhooks | Built in | Limits are in `hard-limits.md`. API tokens belong to a real user; there are no service accounts. (F, R) |
| Browser extension | Built in | Chrome and Firefox; saves a page as a record. Not a full web clipper. (F) |
| Desktop and mobile apps | Built in | See `hard-limits.md` for what mobile covers. |
