# Fibery pricing and plan gating

Checked 12 November 2026 against [fibery.com/pricing](https://fibery.com/pricing) and [Subscription & Billing](https://the.fibery.io/@public/User_Guide/Guide/Subscription-&-Billing-60). Prices change; always add "see the pricing page" when quoting one.

## Plans

| Plan | Price per paid user per month, billed annually | Who can buy |
|---|---|---|
| Free | $0 | Up to 10 users and 10 guests |
| Standard | $12 | Any size |
| Pro | $20 | Any size |
| Enterprise | $40 | At least 25 paid seats, billed even if fewer are used |

- Monthly billing exists and costs more; the page says annual saves 20% but does not print the monthly prices. Do not quote monthly prices.
- Only Admins and Members need a paid seat. Observers (read-only) and Guests are free on every plan.
- Every new workspace gets a 14-day Pro trial, no credit card. Afterwards: stay on Pro, pick another paid plan, or move to Free.
- Free is a permanent plan, not a trial.
- Each workspace is a separate subscription. Workspaces do not share data, except through Fibery-to-Fibery sync on Enterprise.

## What each plan adds

| Plan | Adds |
|---|---|
| Free | 10 databases, unlimited entities, documents, formulas, automations, integrations, remote MCP server |
| Standard | Unlimited databases, AI, charts, whiteboards, human support |
| Pro | Custom apps, advanced permissions (user groups, custom access templates), JavaScript in automations, unlimited version history, no Fibery branding on forms, two-way Jira sync, payment by invoice |
| Enterprise | SAML SSO, SCIM, choice of data region (EU, US, UK, APAC), Fibery-to-Fibery sync, unlimited automations and syncs, customer success manager |

## Limits

| Item | Free | Standard | Pro | Enterprise |
|---|---|---|---|---|
| Databases | 10 | Unlimited | Unlimited | Unlimited |
| File storage | 1 GB | Unlimited | Unlimited | Unlimited |
| Version history / activity log | 14 days | 90 days | Unlimited | Unlimited |
| Automation runs per month | 250 | 1,000 + 100 per seat | 10,000 + 1,000 per seat | Unlimited |
| Synced entities per month | 5,000 | 25,000 + 2,500 per seat | 250,000 + 25,000 per seat | Unlimited |
| Synced integrations | 1 | Unlimited | Unlimited | Unlimited |
| Free guests | 10 | Unlimited | Unlimited | Unlimited |
| Entities shared per guest | 10 | 25 | 100 | 250 |
| AI credits per month | None | 250 per seat, up to 10,000 | 500 per seat, up to 25,000 | 1,000 per seat, up to 50,000 |
| Transcription per month | Not listed | 10 h + 1 h per seat | 50 h + 5 h per seat | 100 h + 10 h per seat |
| Data region | EU | EU | EU | EU, US, UK or APAC |

- On Free, whiteboards, timeline, Gantt, feed, map, chart, app and dashboard views are private only (cannot be shared with the team).
- Extra AI usage: Pro and Enterprise can buy more at $15 per 1,000 credits, with a monthly cap. A typical AI request costs about 20 credits.

## Gating that changes a fit answer

| If the visitor needs | Minimum plan | Say |
|---|---|---|
| SAML SSO, SCIM, or data outside the EU | Enterprise | Needs 25+ paid seats at $40, so about $12,000 a year minimum (calculated: 25 × $40 × 12) |
| User groups or custom access rules | Pro | |
| Two-way Jira sync | Pro | |
| Custom apps shared with the team | Pro | |
| Forms without Fibery branding | Pro | |
| Many read-only stakeholders or clients | Any paid plan | Observers and guests are free |
| A team of 10 or fewer with up to 10 databases | Free | |

## Discounts

| Who | Offer | Source |
|---|---|---|
| Startups: under 42 employees, not a service provider (such as a consultancy), not already paying | 6 months of Pro free | [Startup program](https://fibery.com/startup-program) |
| Non-profit and educational organizations | 50% off | [Free offers and discounts](https://the.fibery.io/@public/User_Guide/Guide/Free-offers-and-discounts-61) |
| Ukrainian companies | 50% off, until 2030 | Same |
| Open-source projects | Free | Same |

Never offer a discount that is not in this table.

## Payment and cancellation

- Cards, PayPal, Apple Pay. Bank transfer on Pro and Enterprise for annual billing or invoices over $1,000.
- Refund within 30 days of payment, on request.
- Cancel any time; paid features last to the end of the billing cycle, then the workspace moves to Free.
- Adding a user mid-cycle is charged pro rata; removing one gives a credit on the next bill.

## Help with setup

From [Expert help](https://fibery.com/expert-help): free live demo, support chat, workspace review, and a concierge service where the Fibery team sets up the workspace, imports data and trains the team. The demo is free; prices for the others are not published.

## To verify with the team

- Whether Standard can share Gantt and app views (the pricing table suggests private only).
- Whether Microsoft login and login restriction are plan-gated (Fibery 101 says paid plans, and Pro and up).
