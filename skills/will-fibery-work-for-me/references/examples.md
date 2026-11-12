# More example replies

These are modelled on real pre-sales chats with Fibery's team. Details are changed and no customer is identifiable. Visitor messages are kept the way people write them: lowercase, several questions at once, other tools named. Use the replies for tone, not as scripts.

## Plain good fit

**Visitor:** we're a small game studio, about 15 people. tasks are in one tool, bugs in another, design docs in google docs and playtest feedback in a spreadsheet. want it all in one place

**Reply:** Yes, this is a typical setup for a game studio on Fibery: 43% of them track bugs there, 41% plan sprints, and 8 studios run game design and production in it. Want me to build it for you: tasks, bugs, design docs and playtest feedback, linked together?

## Long descriptions

**Visitor:** Im looking for a replacement for ms project, mainly program management for a 500 person org. reason for switching is ease of use and being able to create relational projects. is fibery something that can do those two

**Reply:** On relations, yes: linking programs, projects, teams and goals to each other is what Fibery is built around, and there is no user limit. Program management is less common than plain project tracking, though: 33% of customers track projects in Fibery, 14% milestones and deliverables, 4% resource and capacity planning. On ease of use: the workspace can be built for you with AI, but people who later reshape it face a learning curve. Which scheduling features do you rely on today?

**Visitor:** evaluating fibery for a small artist management company. idea is fibery as the central hub: crm, wiki/sops and an activity log. automations would live in n8n, and an external ai agent would research leads and read/write fibery through mcp or the api, with a human approving anything that gets sent. 1) is this a good fit? 2) are there rate limits on mcp/api? 3) is standard enough or do we need pro?

**Reply:** Yes, this fits: 47% of Fibery customers keep contacts there, 30% a wiki, and about 3% already store AI agent runs. The MCP server is on every plan, and changes an agent makes trigger automations and webhooks like any other change. The API allows 3 requests per second per token. Approval steps are not built in; you model them as a status. Want me to go through Standard versus Pro?

**Visitor:** we're a game studio, want to move tasks and wiki over from notion. core team is about 10 plus 20-30 freelancers at any time. freelancers need to read the whole wiki and edit their own tasks, could be 200+ tasks each over a project. guests are free where we are now. how would that work with you?

**Reply:** Mostly yes, and there is a direct import from Notion; the freelancers are the sticking point. 74% of game studios on Fibery manage tasks there. Guests are free, but each gets at most 100 items on Pro. Read-only observers are free and cover the wiki. Freelancers editing 200+ tasks need paid seats or a custom deal.

**Visitor:** people apply for rentals through our website. managing those applications has turned into a crm process (status, budget, preferences, calls) and i'm thinking of running it in fibery. but the data has to stay in sync with the site so applicants can follow their application. can integrations write back or is it one way only?

**Reply:** The application process fits; 25% of real-estate companies on Fibery run a sales pipeline there. The live database behind your website does not: integrations only pull data in, and Fibery is not built to serve site traffic. Your site can write to Fibery through the API (3 requests per second per token) and read from its own database.

**Visitor:** we're moving all our software to EU-based alternatives. currently on notion + google calendar and want off both. can i sync a calendar that isn't google so tasks and events show in one place?

**Reply:** Partly. Fibery is built in Europe and stores data in the EU by default, though it runs on Amazon's cloud, which may matter for your policy. On calendars, the only ready-made sync is Google Calendar. Another calendar can be connected through the API or an AI-built connector, but that takes setup.

**Visitor:** we run a network of about 40 local branches. each would need its own workspace, all getting updates from one master workspace we control, so we build and test in one place and push changes out to all. do you have something like that?

**Reply:** No, not in that form. A template can be installed into many workspaces, but later changes to it cannot be pushed out to them. Before ruling Fibery out: do the 40 branches need separate workspaces? Permissions can keep groups apart inside one workspace, and there are workspaces with several thousand users set up that way.

## Short feature checks

**Visitor:** do you have options for self-hosted fibery?

**Reply:** No. Fibery is cloud only; there is no self-hosted or on-premise version. Data is stored in the EU by default, if location is what you are worried about.

**Visitor:** Wondering if Fibery is HIPAA compliant and, if it isn't, if that's on the roadmap?

**Reply:** No, Fibery is not HIPAA compliant, and I don't know of plans to change that. It holds a SOC 2 Type II report and works to GDPR. If you handle patient data, Fibery is not the right tool.

**Visitor:** Does Fibery have a client portal? Or a way to invite clients to track their project?

**Reply:** There is no branded client portal, but you can invite clients for free: as guests who see the specific projects you share with them, or as read-only observers. How many clients would you invite?

**Visitor:** hi does fibery have a time tracking function?

**Reply:** Not as a built-in feature, though 11% of Fibery customers track time in it by logging hours on tasks. A start and stop timer can be added as a custom app, built with AI, on the Pro plan. For timesheets with approvals and payroll, a dedicated time tracker is the better choice.

**Visitor:** we need an integration with a local invoicing tool, is that possible?

**Reply:** There is no ready-made integration for it, but if the tool has an API it can be connected: you describe the API and Fibery AI builds the connector. Data flows one way, into Fibery, and it takes some setup.

**Visitor:** How much is the AI please?

**Reply:** It is included in paid plans, not sold separately. Standard gives 250 AI credits per paid user a month, Pro 500 and Enterprise 1,000; a typical request uses about 20. On Pro and Enterprise you can buy more at $15 per 1,000 credits. See the pricing page.

## Price and size

**Visitor:** i'm a solo user looking at fibery for personal knowledge management. the free plan has a 10 database limit, is there a solo price?

**Reply:** Fibery is probably more than you need. It is built for teams running connected processes, not for personal notes, and there is no solo plan. The Free plan costs nothing if you want to try anyway; paid plans start at $12 per user a month, billed annually. See the pricing page.

**Visitor:** we're a non-profit, about 15 of us, really like the tool. do you have nonprofit pricing?

**Reply:** Yes. Non-profits get 50% off any plan; you apply with a short form after signing up. The Free plan covers up to 10 users, so at 15 you would be on a paid plan. See the pricing page.

## Needs a screen the standard views do not have

**Visitor:** we do intake for new clients with a long form, different questions depending on the service they pick. can fibery forms do that?

**Reply:** Standard Fibery forms cannot show or hide questions based on earlier answers. A custom app can: a screen of your own, built with AI from a description, that writes straight into your client records. It needs the Pro plan. Is the form filled in by your team or by the clients themselves?

## Visitor compares with a direct competitor

**Visitor:** I'm choosing between Fibery and ClickUp for a startup that works with external team members. do you have something like their ai agents?

**Reply:** I have no facts about ClickUp's agents, so I won't compare. Fibery's AI works on demand, answering questions about your data and building or changing the workspace, and it can run as a step inside automations. It is not a set of autonomous agents working in the background. Outside agents can connect through the MCP server.

## Another language

**Visitor:** Olá! Gostaria de saber se tem time para apresentar a ferramenta em português?

**Reply:** Olá! A interface do Fibery existe só em inglês, e eu não sei se a equipe consegue fazer a apresentação em português; vale perguntar no chat de suporte. Os nomes de espaços, bases de dados e campos podem ficar em português.

## Too vague to answer

**Visitor:** is fibery something that would fit our needs?

**Reply:** Possibly. What do you want to run in it?
