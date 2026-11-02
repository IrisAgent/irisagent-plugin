# IrisAgent

Get grounded answers to customer questions and ask about your customer support operation, from Claude and ChatGPT, with the IrisAgent Support Analyst. Answers are grounded in the tickets, chats, and knowledge IrisAgent has already ingested for your organization, and they cite the tickets they used.

## Skills

| Skill | What it does |
|---|---|
| `get-started` | Explains what IrisAgent can do and suggests first questions to ask about your support data. |
| `get-ai-answer` | Gets the grounded AI answer for a question or ticket, from your knowledge base and procedures, with cited articles. Uses the same pipeline as your IrisAgent chatbot, and says so when no grounded answer exists. |
| `weekly-support-briefing` | Summarizes the latest week in support: AI deflection, volume, escalations, knowledge gaps, AutoQA results, and new ticket categories, compared with the previous week. |
| `ticket-volume-trends` | Counts and charts ticket volume over time, grouped by category, priority, status, team, assignee, account, or sentiment, and explains what is driving a change. |
| `ticket-search` | Finds tickets by topic or meaning, not just exact words, plus status, date, priority, assignee, team, or account filters, and searches past conversations for what was said. |
| `escalation-triage` | Lists the cases and customers that need attention now, with escalation scores, reasons, sentiment, and how long they've been waiting. |
| `account-health` | Builds an account overview before a customer call: health score, case volume, categories, recent and escalated cases, and linked Jira issues. |
| `agent-performance` | Reports a support agent's ticket load, resolution time, first response and reply times, and CSAT, and compares agents. |
| `ai-answer-audit` | Checks whether an AI answer already delivered on a ticket or chat was correct, by auditing it against the articles it cited and flagging hallucinations, wrong articles, and knowledge gaps. |
| `conversation-qa` | Scores a ticket conversation against your team's QA rules and shows which rules passed or failed, with evidence. Translates non-English conversations first. |
| `knowledge-drafts` | Drafts knowledge base articles and answer procedures from resolved tickets or a topic, grounded in how your team actually solved the problem. Drafts are never published. |
| `jira-impact` | Connects support to engineering: looks up Jira issues by key, topic, or customer account, read only through your Jira connection, and links them to the tickets they affect. |
| `chatbot-insights` | Analyzes chatbot conversations: how many chats you got, top topics, outcomes and escalations, and the details of any single chat. |

## Requirements

An IrisAgent account with a connected ticketing system, such as Zendesk, Salesforce, Freshdesk, Intercom, or Jira Service Management.

## What this plugin connects to

This plugin contains only skill instructions and a connection to the IrisAgent MCP server at `https://mcp.irisagent.com/mcp`. It runs no local code. Each person signs in with their own IrisAgent account through OAuth, and access is limited to their organization.

Questions and answers, including quoted ticket text, pass between your AI assistant and IrisAgent. See the [IrisAgent privacy policy](https://irisagent.com/privacy-policy/).

The plugin is read only. It can't change tickets, send replies, or publish articles, and knowledge drafts stay drafts until a person publishes them in the IrisAgent portal.

## Documentation and support

- [Setup guide](https://docs.irisagent.com/deploying-irisagent/MCP-Server)
- [Contact support](https://irisagent.com/contact-us/)
