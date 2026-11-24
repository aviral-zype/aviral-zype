<h1 align="center">Aviral Gupta: AI Engineer · Agentic Workflows · React/TypeScript Frontend</h1>

<p align="center">
  <b>I build AI agents that take software from spec to deploy, and polished React front ends for video streaming apps on the web, phones and Smart TVs.</b><br/>
  6+ years of professional experience · AI-native engineer (Claude Code, MCP, Copilot, Cursor) · open-source Video.js plugin author · based in India
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/aviralguptaa"><img alt="Aviral Gupta on LinkedIn" src="https://img.shields.io/badge/LinkedIn-aviralguptaa-0A66C2?logo=linkedin&logoColor=white"></a>
  <img alt="Builds with Claude Code" src="https://img.shields.io/badge/builds%20with-Claude%20Code-D97757?logo=anthropic&logoColor=white">
  <img alt="Model Context Protocol (MCP)" src="https://img.shields.io/badge/MCP-integrations-555">
  <a href="https://www.npmjs.com/package/@video-js/ad-schedule-plugin"><img alt="npm version of @video-js/ad-schedule-plugin" src="https://img.shields.io/npm/v/@video-js/ad-schedule-plugin?label=npm&logo=npm"></a>
  <a href="https://www.npmjs.com/package/@video-js/ad-schedule-plugin"><img alt="Yearly npm downloads of @video-js/ad-schedule-plugin" src="https://img.shields.io/npm/dy/@video-js/ad-schedule-plugin?label=downloads"></a>
</p>

## About me

**Aviral Gupta** (GitHub: `aviral-zype`) is an **AI engineer and frontend engineer** from India with more than six years of professional experience. I build **agentic AI workflows** on **Claude Code, the Claude API and the Model Context Protocol (MCP)**, and **React / TypeScript front ends** for OTT video streaming apps on the web and Smart TVs (Samsung Tizen, LG webOS, Xbox, Vizio).

I work **AI-first**. My agents investigate the ticket, write the code, run the tests, review it for bugs and security, and open the pull request. I own the spec, the design decisions and the final review. That lets me ship features across web, iOS, Android, Roku and Smart TV apps much faster, without lowering the quality bar.

## AI engineering

### Personal AI developer agent (TypeScript, Claude Code headless)

A daemon of about 4,000 lines of TypeScript that runs my day-to-day engineering loop with AI agents, with a human in the loop on every outbound action.

- **Event-driven agent pipeline:** watches Jira, Slack and GitHub (polling + webhooks), queues events in SQLite with debounce and de-duplication, then routes each one to an agent capability.
- **Agents that do real work:** investigate tickets across code, docs and logs; write code in isolated git worktrees; run lint and tests with retries; open draft PRs; review PRs with inline comments; fix review feedback; draft Slack replies and stand-ups.
- **Autonomy gate:** every action type (comment, push, PR, reply…) is set to `off`, `draft` or `auto`. Drafts are approved from Slack buttons or a local web dashboard, so autonomy is earned one action at a time.
- **Guardrails by design:** least-privilege tool profiles (the LLM can't post or push by itself; only a separate executor can), protected branches never pushed, dry-run by default, kill switch, daily cost caps and per-run budgets, and a full audit trail.
- **Learning loop:** my edits to the agent's drafts are stored and fed back into future prompts, so its output matches my style over time.

### Claude Code skills and multi-agent workflows

- **AI code review:** reviews PRs against the ticket's acceptance criteria, cross-repo API contracts and a security checklist, plus lessons mined from past human review comments.
- **Ship-a-PR pipeline:** build gate → AI correctness and security review → commit → PR → reviewer and Copilot review → ticket update.
- **Parallel end-to-end testing:** one test agent per platform (web, iOS/tvOS simulators, Android TV, Roku, Smart TVs) running at the same time, which posts test cases and screenshot evidence back to the ticket.
- **Cross-platform status:** one view of ticket × repo × PR × CI × review state for multi-platform features.
- **MCP integrations:** Jira, Confluence, Slack, GitHub and Grafana wired into the agents as tools.

### How I ship with AI

**Spec → API contract → parallel agents per platform → cross-platform consistency check → AI review + security review → human review → tests with evidence → deploy.**

## Frontend engineering

- **React and Next.js user interfaces:** reusable components, responsive layouts, and clean, maintainable frontend architecture for large apps.
- **Video in the browser:** HTML5 video, **Video.js** and **Bitmovin** player integrations, and player UI that works across browsers and TV platforms.
- **Video advertising:** **VAST and VMAP** pre-roll, mid-roll and post-roll ads, ad tracking, skip buttons and click-throughs, all in a single video element.
- **Smart TV and 10-foot UIs:** web apps for **Samsung Tizen, LG webOS, Xbox and Vizio** that run on low-power TV hardware and are driven by a TV remote.
- **Sign-in, purchase and paywall flows:** TVOD purchases, entitlements and TV-provider sign-in screens.
- **Frontend quality:** **Cypress** end-to-end tests, ESLint, esbuild and Webpack builds, CommonJS + ES-module packages, and automated npm releases with GitHub Actions.

## Featured open source

### [videojs-vast-plugins](https://github.com/aviral-zype/videojs-vast-plugins): Video.js VAST/VMAP ad plugin

Published on npm as **[`@video-js/ad-schedule-plugin`](https://www.npmjs.com/package/@video-js/ad-schedule-plugin)**.

- Plays **VAST and VMAP ads** (pre-roll, mid-roll, post-roll) inside the **same video element** as the content, so there are no visual or audio glitches when switching between ad and content.
- **Schedules ad breaks** at any moment of playback, with ad timeouts, skip button, click-through (CTA) zone and limited-ad-tracking support.
- Built for **HTML5 Smart TV apps**: Samsung Tizen, LG webOS, Vizio, Xbox and Zeasn.
- Works with **Video.js 5, 6, 7 and 8**, ships CommonJS and ES-module builds, is tested with Cypress, and has 10 npm releases (Apache-2.0).

### [countbase-sdk-web](https://github.com/aviral-zype/countbase-sdk-web): web analytics SDK

A JavaScript SDK for **web analytics, crash reporting, remote config and feedback widgets**, maintained as a fork of the Countly Web SDK and tested with Cypress.

## Beyond the frontend

- **Backend and APIs:** Node.js, Fastify, Ruby on Rails, GraphQL, PostgreSQL, Redis, SQLite.
- **Native and TV apps:** iOS and tvOS, Android and Android TV, Roku (BrightScript).
- **Build and release:** GitHub Actions, CircleCI, Xcode Cloud, app-store signing.
- **Cloud and security:** AWS, private storage, signed links and KMS-backed secrets.

## Tech stack

**AI and agents:** Claude Code (skills, subagents, headless mode) · Claude API · Model Context Protocol (MCP) · AI agents and tool use · prompt engineering · human-in-the-loop guardrails · GitHub Copilot · Cursor · OpenAI / ChatGPT<br/>
**Frontend:** React · Next.js · JavaScript (ES6+) · TypeScript · HTML5 · CSS3 · Video.js · Bitmovin Player<br/>
**Smart TV and devices:** Samsung Tizen · LG webOS · Xbox · Vizio · Roku · tvOS · Android TV<br/>
**Testing and tooling:** Cypress · ESLint · esbuild · Webpack · Babel · npm · GitHub Actions<br/>
**Backend and cloud:** Node.js · Fastify · Ruby on Rails · GraphQL · PostgreSQL · Redis · SQLite · AWS

## FAQ

<details>
<summary><b>Is Aviral Gupta an AI engineer?</b></summary>

Yes. Aviral builds agentic AI systems on Claude Code, the Claude API and MCP: a TypeScript developer agent with an autonomy gate, tool guardrails and cost limits, plus multi-agent Claude Code workflows for code review, shipping pull requests and parallel cross-platform testing.
</details>

<details>
<summary><b>What does Aviral Gupta specialise in?</b></summary>

AI agents and agentic developer workflows, and frontend engineering with React and TypeScript for video streaming (OTT) apps on the web and Smart TVs: video players, video ads (VAST/VMAP), and sign-in and purchase flows.
</details>

<details>
<summary><b>Which AI tools does Aviral Gupta use?</b></summary>

Claude Code (custom skills, subagents and headless mode), the Claude API, MCP servers for Jira, Confluence, Slack, GitHub and Grafana, GitHub Copilot, Cursor, and OpenAI / ChatGPT.
</details>

<details>
<summary><b>How much experience does Aviral Gupta have?</b></summary>

More than six years of professional software development: React and JavaScript front ends, full-stack work on Ruby on Rails and GraphQL backends and native TV apps, and AI agent engineering.
</details>

<details>
<summary><b>Has Aviral Gupta built Smart TV apps?</b></summary>

Yes. Aviral builds and maintains web-based streaming apps for Samsung Tizen, LG webOS, Xbox and Vizio, and wrote an open-source Video.js plugin that plays ads on those platforms.
</details>

<details>
<summary><b>How can I contact Aviral Gupta?</b></summary>

Message Aviral on <a href="https://www.linkedin.com/in/aviralguptaa">LinkedIn</a>.
</details>

## GitHub stats

<img alt="Aviral Gupta's GitHub stats" src="https://github-readme-stats.vercel.app/api?username=aviral-zype&show_icons=true&theme=radical">

## Let's connect

I enjoy talking about AI agents, developer tooling, React and building UIs for the big screen. Find me on **[LinkedIn](https://www.linkedin.com/in/aviralguptaa)**.
