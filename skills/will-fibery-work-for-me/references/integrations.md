# Fibery integrations

Checked 12 November 2026 against [fibery.com/templates](https://fibery.com/templates) and the user guide ([Integrations overview](https://the.fibery.io/@public/User_Guide/Guide/Integrations-overview-501), [Import and integrations](https://the.fibery.io/@public/User_Guide/Guide/Import-and-integrations-541)).

## Rules that apply to every integration

- **Direction:** sync is one way, into Fibery. Synced fields are read-only in Fibery; you can add your own fields, relations, formulas and automations on top.
- **The one exception:** Jira has a true two-way sync for specific fields (Pro and Enterprise).
- **Sending data out:** possible but takes effort. Use pre-built actions (table below), the "send web request" automation action, scripts, or an automation platform.
- **Frequency:** every 60, 120 or 240 minutes, daily, or manual. Some integrations also get near-instant updates through webhooks. Email syncs every 5 minutes by default.
- **Limits:** synced entities per month depend on the plan; Free allows one synced integration. See `pricing.md`.
- **Leaving:** "disconnect and migrate" turns synced databases into normal Fibery databases.

## Native integrations

| Tool | What comes in | Sends data back | Notes |
|---|---|---|---|
| Email (Gmail, Outlook business, IMAP) | Messages, threads, attachments, contacts | Yes: send and reply from Fibery | Several accounts into one database; auto-link to companies and contacts |
| Slack | Messages from public channels | Yes: actions in automations | Private and archived channels are not synced |
| Slack Bot | — | Creates entities from Slack, `/fibery` commands, notifications | Bot sends direct messages only |
| Intercom | Conversations, companies, contacts, tags | No | Near real time on reply, status change, tag |
| Zendesk | Tickets | No | |
| Discourse | Topics, posts, users | No | Webhooks for instant updates |
| GitHub | Pull requests and related code data | Yes: actions | |
| GitLab | Projects, merge requests | Yes: actions (for example close a merge request) | |
| Bitbucket | Projects, repositories, branches | No | |
| Jira | Issues and related data | Yes: two-way for specific fields | Two-way needs Pro or Enterprise |
| Linear | Issues, initiatives | No | |
| HubSpot | Companies, deals, engagements | No | First sync can take hours |
| Stripe | Customers, subscriptions, invoices, products, prices | No | |
| Braintree | Plans, subscriptions, transactions | No | |
| Google Calendar | Events | No | Two-way calendar sync is an open customer request |
| Productboard | Product hierarchy, customers, feedback | No | Mostly used to migrate |
| Trello, Asana | Existing work items | No | Mostly used to migrate; Trello does not bring labels, covers or comments |
| Readwise | Highlights and notes | No | |
| RSS | Feed items | No | |
| World, Currency Exchange, Periods | Countries, exchange rates, calendar periods | — | Reference data |
| Fibery-to-Fibery | Databases from another workspace | No | Enterprise on the receiving workspace |

Imports from files: CSV and Markdown.

**Direct competitors:** importers also exist for three tools that are direct competitors (Airtable, ClickUp, Notion). You may confirm that "there is a direct import from the tool you use now" but do not write those names in a reply.

## Everything else

| Route | Use it for | Source |
|---|---|---|
| Automation platforms: Zapier, Make, n8n, viaSocket | Connecting tools with no native integration; pushing data out | [Make](https://the.fibery.io/@public/User_Guide/Guide/Make-(Integromat)-integration-82), [n8n](https://the.fibery.io/@public/User_Guide/Guide/n8n-integration-452) |
| Byteline | Third-party two-way sync with other apps | [Byteline](https://the.fibery.io/@public/User_Guide/Guide/Byteline-integration-426) |
| AI connectors (beta) | Any tool with an HTTP API, including internal company APIs. Describe the integration in plain language and Fibery AI writes, tests and publishes the connector. Signs in with an API key or OAuth. Data syncs one way into Fibery; the AI can also add custom actions that write back to the tool from automations, and webhooks when the tool's API has them. Building costs AI credits; running is free for now. | [AI connectors](https://the.fibery.io/@public/User_Guide/Guide/AI-Connectors:-creating-custom-integrations-488); Michael, 12 Nov 2026 |
| Custom connector | Developer hosts a small service that follows the integrations API | [Developers](https://developers.fibery.com) |
| HTTP API, GraphQL API, webhooks, history API | Reading and writing data from code | [API overview](https://the.fibery.io/@public/User_Guide/Guide/Fibery-API-overview-279) |
| MCP server | Connecting AI assistants (Claude, ChatGPT, Gemini, Cursor and others) to the workspace. On every plan, including Free. | [MCP server](https://the.fibery.io/@public/User_Guide/Guide/Fibery-MCP-Server-401) |
| Browser extension | Saving web pages as entities (Chrome, Firefox) | [Fibery 101](https://fibery.com/101-questions-about-fibery) |

## No native integration

State these plainly. None is a blocker when the tool has an API: the route is an AI-built connector, an automation platform, or a custom connector.

- LinkedIn (no connector or scraper)
- Meeting recording tools
- Confluence
- Microsoft Teams (only through Make)
- Not found in the guide, so treat as not native until confirmed: Outlook Calendar, Salesforce, Discord, Google Drive, Figma, accounting tools

## How to answer integration questions

- "Does Fibery integrate with X?" If X is in the native table, say yes and say what comes in. If the visitor needs changes in Fibery to appear in X, say sync is one way unless X is Jira.
- If X is not native, say so, then say that any tool with an API can be connected with an AI-built connector, and that it takes some setup. Only a tool with no API at all is a dead end.
- API limits (3 requests per second per token, 7 per workspace) are in `hard-limits.md`.
- Never describe a one-way sync as "connects with" without saying the direction.
