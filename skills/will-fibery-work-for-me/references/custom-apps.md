# Custom apps

Checked 12 November 2026 against [fibery.com/features/custom-apps](https://fibery.com/features/custom-apps) and the user guide ([Custom Apps](https://the.fibery.io/@public/User_Guide/Guide/Custom-Apps-502), [Custom Apps FAQ](https://the.fibery.io/@public/User_Guide/Guide/Custom-Apps-FAQ-504), [Build Apps via MCP](https://the.fibery.io/@public/User_Guide/Guide/Build-Apps-via-MCP-528)).

## What it is

A custom app is a screen of your own inside Fibery, built on top of the workspace's data. Think of it as a custom view: people use it to see, add, change and delete records in whatever layout fits the job. It lives in the workspace, next to the standard views.

It matters for fit because it covers needs the standard views and forms do not. When a visitor needs a particular screen, form behaviour or way of working with their data, a custom app is often the answer, so check here before calling something a gap.

## Facts

| Topic | Fact |
|---|---|
| How it is built | Describe what you want and Fibery AI builds it. It can also be built with your own AI assistant (Claude, ChatGPT and others) through the MCP server, and the code can be edited by hand afterwards. |
| Time to build | A first version typically takes 5 to 30 minutes, then you iterate by asking for changes. |
| What it can do | Read and write workspace data: show, create, update and delete records across linked databases. |
| What it cannot do | It is interface only, with no server-side logic. Anything that must run on a schedule or in the background belongs to automations. |
| Permissions | People see only the data they already have access to in the workspace. |
| Versions | Every build is saved as a version; you can roll back to any of them. |
| Plan | Pro or Enterprise. The 14-day trial is on Pro, so it includes custom apps. |
| Cost | No add-on. Building with Fibery AI uses the plan's AI credits; building through your own AI assistant costs only that assistant's usage. Using a finished app costs nothing. |
| Who can build | Any user in their private space; people with architect access in a shared space; admins anywhere. |
| Mobile | Works on mobile when the app is built to be mobile-friendly. |
| Look | Matches Fibery's interface, including dark theme. Custom styling is not supported. |
| Sharing outside Fibery | An app cannot be shared or published on its own. Publishing the whole space to the web makes the app visible to everyone along with the rest of the space. |
| Where it can sit | As a view in a space, or embedded in a document or rich text field. |

## Good examples to mention

From the feature page and the guide:

- A multi-step form that shows or hides fields based on earlier answers
- A calendar laid out the way the team needs it
- An inbox-style screen for working through incoming requests
- A time tracker with a start and stop timer and weekly totals
- A test-run tracker for QA
- A barcode scanner
- A dashboard, a tree map of product areas, a release overview

## What a custom app does not fix

- Offline work, self-hosting and the other hard blockers
- Sending mass email, taking payments, e-signature, or anything else that needs a server-side service
- A standalone public app or a branded portal for outside users
- The limits of the plan it runs on

## How to use this in a reply

- When a need is "a screen or form that works a certain way", say a custom app can provide it, and that it is built with AI from a description. When the custom app is what turns the answer into a yes, say that it needs the Pro plan.
- Keep it honest: it is a first version in minutes followed by iteration, not a finished product on the first try.
- Do not present a custom app as the answer to a blocker or to a need that sits outside Fibery.
