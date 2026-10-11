# Qaa Si Documentation

Autonomous AI trading agents with governed execution, transparent risk controls and on-chain infrastructure built around Base.

> Also readable on the website: [qaasi.webflow.io](https://qaasi.webflow.io) → Documentation

## Contents

**Getting started**

- [Introduction](#introduction)
- [Overview](#overview)
- [Vision & Mission](#vision--mission)

**Trading**

- [Trading Agents](#trading-agents)
- [How Agents Trade](#how-agents-trade)
- [Risk Engine](#risk-engine)
- [Inside the Agent](#inside-the-agent)

**Platform**

- [AI Agent Ecosystem](#ai-agent-ecosystem)
- [Architecture](#architecture)
- [Built on Base](#built-on-base)
- [Security & Transparency](#security--transparency)

**Token**

- [Token & Utility](#token--utility)
- [Audit & Certification](#audit--certification)

**Project**

- [Roadmap](#roadmap)
- [Risks & Disclaimer](#risks--disclaimer)

---

## Introduction

<sub>Getting started</sub>

> Autonomous AI trading agents with governed execution, transparent risk controls and on-chain infrastructure built around Base.

### Autonomous intelligence for the markets.

Qaa Si is built around autonomous trading agents that observe markets, reason over signals and context, propose or execute trades within defined permissions, and monitor risk continuously. The goal is controlled automation, not unrestricted automation: intelligence, risk authorization and execution are kept separate.

> [!NOTE]
> **Development status.** The project is under active development. Capabilities are labelled **Live**, **Beta**, **In Development** or **Planned**. Exchange support, strategy availability, tokenomics, contract addresses and launch parameters are only presented as live once they are finalized and verifiable.

### The Qaa Si trading system

`Market Data` → `AI Agent` → `Trade Thesis` → `Risk Engine` → `Execution Layer` → `Position Monitoring` → `Exit / Adjust`

If the Risk Engine blocks a proposed action, the result is **no trade**. After an exit or adjustment the loop starts again with fresh market data. The agent can identify an opportunity, but permissions and risk controls decide whether it acts: a useful signal does not automatically become an order.

### Explore the core product

- **Trading Agents**: The core product layer: autonomous agents for market analysis, governed decisions and trading workflows.
- **How Agents Trade**: The full loop from observation and analysis through risk validation, execution and monitoring.
- **Risk Engine**: How exposure, permissions and execution constraints sit between AI reasoning and the exchange.
- **Inside the Agent**: What an agent can observe, decide, request and execute, and where its authority ends.

### Why the architecture matters

- **Intelligence**: Agents combine market observations, strategy logic, context and tool access to form a trade thesis. *What appears worth doing?*
- **Control**: The risk and execution layers decide whether a proposed action is permitted, within limits and eligible for execution. *What is actually allowed to happen?*

### Four operating principles

| Principle | Meaning |
|---|---|
| Agent-native | Autonomous agents are the primary product layer, not a cosmetic AI add-on. |
| Risk-gated | Trade intent is checked against explicit controls before execution. |
| Transparent | Product status, permissions and on-chain claims can be independently understood and verified. |
| Human-governed | Users keep control over permissions, limits and consequential actions. |

### Beyond trading

Qaa Si is designed as a broader AI-agent ecosystem. Trading is the flagship use case; the architecture can also support research, analysis, workflow automation, integrations and future on-chain interactions.

### Join the Qaa Si community

| Channel | Purpose | Status |
|---|---|---|
| [Telegram](https://t.me/Qaasitoken) | Fast updates, announcements and community conversation. | Live |
| [X / Twitter](https://x.com/Qaasitoken) | Official news, releases and ecosystem updates. | Live |
| Discord | Community discussions, product updates and support. | Coming soon |

> [!WARNING]
> **Official verification matters.** Only links published here or on other verified Qaa Si channels are official. Do not rely on an unverified token contract, treasury address, performance, liquidity or audit claim.

---

## Overview

<sub>Getting started</sub>

> Product thesis, design principles and scope of the Qaa Si ecosystem.

Qaa Si is being designed as an AI-agent ecosystem that combines intelligent autonomous software with blockchain infrastructure on Base. Product capabilities, technical architecture, token mechanics and security controls are documented separately and verified as they mature.

### What Qaa Si is designed to enable

1. **Specialized AI agents** for research, analysis, automation and digital workflows.
2. **Tool-enabled execution** through explicitly authorized APIs, integrations and services.
3. **Permission-aware operations**, with reasoning and execution kept as separate security boundaries.
4. **On-chain infrastructure** for transparent ownership, settlement and ecosystem mechanisms.
5. **Verifiable documentation** for contracts, treasury controls, vesting, liquidity and audits once deployed.

### Product model

`User objective` → `AI agent` → `Context, memory & approved tools` → `Permission boundary` → `Verified result / Base execution`

An agent may judge an action useful, but consequential execution still requires authorization and is subject to system policy.

### Documentation model

| Status | Meaning |
|---|---|
| Live | Available in production and documented as currently usable. |
| Beta | Available in a limited or evolving production form. |
| In Development | Being built or tested; not presented as generally available. |
| Planned | Part of the intended architecture or roadmap, with no production commitment yet. |

> [!NOTE]
> Tokenomics, contract addresses, vesting schedules, liquidity details and other launch parameters are only presented as final once they are verifiable.

### Core principles

1. **AI-native:** agents are the core product layer, not an add-on.
2. **On-chain capable:** blockchain interactions are built around Base infrastructure.
3. **Transparent:** material token, treasury, vesting and liquidity information should be independently verifiable once deployed.
4. **Security-conscious:** agent permissions, smart-contract controls and wallet interactions are documented explicitly.
5. **Utility-focused:** token functionality is tied to defined ecosystem functions rather than unsupported promises.

---

## Vision & Mission

<sub>Getting started</sub>

> The long-term direction and operating mission behind Qaa Si.

### Vision

Qaa Si aims to build an ecosystem in which AI agents help users complete complex digital workflows, while blockchain infrastructure provides transparent ownership, settlement and verifiable economic coordination. The direction is not simply to add AI to a crypto product or a token to an AI interface. The architecture keeps four areas separate so each can be improved and audited independently:

- Intelligence
- Execution
- Authorization
- Economic infrastructure

### Mission

Make sophisticated AI-agent capabilities accessible through one coherent platform, with explicit controls over permissions, data access, tool usage and on-chain execution.

### Three-part operating model

| Layer | Responsibility |
|---|---|
| Intelligence | Interprets intent, reasons over context and coordinates specialized agents. |
| Application | Exposes workflows, integrations and user controls through a consistent product layer. |
| Blockchain | Supports verifiable ownership, settlement and future ecosystem mechanisms on Base. |

### Design philosophy

The documentation separates what is **live**, **in development** and **planned**, so the project is understandable without presenting future concepts as current facts.

> [!TIP]
> A feature becomes part of the documented production system only once its implementation, permissions and operational limitations can be described accurately.

---

## Trading Agents

<sub>Trading</sub>

> Qaa Si’s core product: autonomous agents that analyze markets, operate within defined permissions and carry out governed trading workflows.

Agents are designed to monitor markets, interpret data, evaluate opportunities and execute approved workflows, always within explicit risk and permission limits.

> [!NOTE]
> **Product status.** This section describes the intended architecture, not confirmed production capabilities. Exchanges, strategies, assets, venues and capabilities will carry a status label (Live, Beta, In Development, Planned) once verified.

### What makes an agent autonomous?

An autonomous agent is more than a signal generator. It follows a controlled decision loop: observe, analyze, decide, validate, execute and monitor.

`Market Data` → `Agent Analysis` → `Trade Thesis` → `Risk Engine` → `Execution Layer` → `Position Monitoring` → `Exit / Adjust / Hold`

A rejected thesis ends in **no trade**; after an exit, adjustment or hold the loop returns to market data.

### Core responsibilities

- **Observe**: Continuously evaluate permitted market data and relevant context.
- **Reason**: Form a trade thesis from the configured strategy and available evidence.
- **Validate**: Run proposed actions through portfolio, permission and risk checks before execution.
- **Execute**: Place only actions that the configured execution policy allows.
- **Monitor**: Track positions and respond to changing conditions, limits or exit criteria.
- **Explain**: Record decision context so users can see what the agent did and why.

### Agent profiles

Qaa Si may support specialized agents rather than one general model. Potential profiles include:

- Market scanning
- Trend following
- Mean reversion
- Portfolio coordination
- Execution
- Risk oversight

Specific profiles are listed as product capabilities only after their behaviour, permissions, supported markets and status are confirmed.

### Human control

Autonomy stays bounded. Users keep control over:

- Which accounts an agent can access
- Which actions it can take
- How much capital it may use
- When trading must stop

---

## How Agents Trade

<sub>Trading</sub>

> A transparent view of the trading loop, from market observation through execution to post-trade monitoring.

Qaa Si uses a staged trading loop instead of a single opaque model output, so the path from information to action stays understandable.

### The trading loop

1. **Observe:** the agent receives only the market data, account context and external signals its configuration permits.
2. **Build a trade thesis:** evidence is evaluated against the strategy rules and a candidate action is formed: no trade, enter, reduce, exit or adjust.
3. **Validate risk:** before execution, the action is checked against hard constraints such as position limits, exposure limits, account permissions and other configured controls.
4. **Execute:** only an approved action reaches the execution layer, which should use the minimum account permissions needed for trading.
5. **Monitor:** after execution the agent keeps tracking market conditions, position state and relevant risk thresholds.
6. **Exit or adapt:** the agent decides whether to hold, reduce, close or otherwise adjust the position according to its permitted policy.

### A decision is more than a signal

1. Market data sends the current market state to the trading agent.
2. User controls provide the strategy and permissions.
3. The agent sends a proposed action to the Risk Engine.
4. The Risk Engine approves or rejects it.
5. Only approved orders go to the exchange / execution layer.
6. Execution returns a result to the agent.
7. The agent reports decision, status and outcome to the user.

### No trade is a valid decision

An autonomous agent is never forced to trade. No trade is a valid, and often necessary, outcome when conditions are weak, data is insufficient, risk limits are reached or permissions do not allow an action.

> [!WARNING]
> Autonomous trading does not remove market risk. AI models can be wrong, markets can change quickly and execution can differ from expected results.

---

## Risk Engine

<sub>Trading</sub>

> The control layer that constrains autonomous trading before an order reaches an exchange.

The Risk Engine is an independent control boundary between an agent’s trading decision and execution. Core principle: an agent may identify an opportunity without automatically being allowed to act on it.

### Decision flow

`Permission check` → `Exposure check` → `Position / order limits` → `Market / strategy rules` → `Approved for execution`

Failing any check rejects the trade; only an action that passes all checks is approved.

### Control categories

| Control | Purpose |
|---|---|
| Account permissions | Restricts what an agent may do on a connected account. |
| Position limits | Caps the size of a single position or order. |
| Portfolio exposure | Constrains aggregate risk across positions or assets. |
| Asset / venue allowlists | Restricts trading to approved markets or exchanges. |
| Strategy constraints | Prevents actions outside the configured trading policy. |
| Emergency controls | Pauses or disables trading when predefined conditions are met. |

### Hard limits vs. agent judgment

Critical rules are enforced as deterministic constraints outside the reasoning layer, not left to model judgment alone.

- **Agent judgment**: Reading market context, weighing evidence and proposing an action.
- **Hard controls**: Permissions, exposure ceilings, forbidden actions, account-level limits and emergency shutdown behaviour.

### Emergency stop

A mature deployment should offer a clear way to halt new trading activity, for example a user pause, account disconnect, policy lock or automated circuit breaker. The exact implementation will be published once finalized.

> [!CAUTION]
> The Risk Engine reduces operational risk but cannot eliminate trading losses, model errors, exchange failures, slippage or extreme market events.

---

## Inside the Agent

<sub>Trading</sub>

> A transparency layer: what a Qaa Si agent can see, decide, request and execute.

Instead of treating the agent as a black box, this section defines the boundaries between information, reasoning, permission, risk and execution.

### The five boundaries

| Boundary | Description |
|---|---|
| What it can see | Only data sources, account context and tools explicitly exposed to the agent. |
| What it can decide | It may form a thesis and propose actions within its configured strategy. |
| What it can request | Actions can be passed to permission and risk controls for approval. |
| What it can execute | Only approved operations supported by the connected execution layer. |
| What it cannot do | Anything outside its permissions, blocked by risk controls or unsupported by the system. |

### Agent decision envelope

`Inputs` → `Reasoning` → `Proposed action` → `Permission boundary` → `Risk boundary` → `Execution` → `Audit / monitoring`

Both the permission boundary and the risk boundary can block an action, which then ends as **rejected**.

### What users should be able to inspect

Where technically available, key context around an action can be shown without revealing private chain-of-thought reasoning:

1. The strategy or agent profile involved
2. The market and asset evaluated
3. The action requested
4. Relevant risk checks and whether they passed
5. The execution status
6. Order or transaction identifiers where applicable
7. Position state and subsequent actions

### Why this matters

Autonomous systems are easier to trust when their boundaries and outputs can be inspected, even if the model’s reasoning is not shown word for word.

> [!TIP]
> The goal is accountable autonomy: agents that act independently within defined rules while users keep visibility and control over consequential actions.

### Future transparency features

- Agent activity timelines
- Risk-event histories
- Execution receipts
- Strategy versioning
- Per-agent status dashboards

These are documented as live only once implemented and verified.

---

## AI Agent Ecosystem

<sub>Platform</sub>

> How Qaa Si agents reason, use tools, verify results and stay under human control.

An agent is software that interprets a user’s objective, reasons over available context, selects permitted tools and executes defined actions within explicit boundaries.

### Agent lifecycle

1. **Intent:** identify the user’s objective and relevant constraints.
2. **Context:** retrieve relevant information, approved memory and task state.
3. **Reasoning:** plan a sequence of actions and identify uncertainty or missing requirements.
4. **Tool selection:** consider only tools and integrations permitted for the task.
5. **Authorization & execution:** consequential actions pass the applicable permission boundary before running.
6. **Verification:** check the result before completion is reported.

### Capability categories

| Category | Description | Status |
|---|---|---|
| Research | Gather, compare and synthesize information from approved sources. | In development |
| Analysis | Work with structured data, documents and task-specific context. | In development |
| Automation | Coordinate repeatable digital workflows across connected tools. | In development |
| On-chain interaction | Prepare or execute blockchain actions subject to explicit authorization. | Planned / staged |

### Human control

> [!WARNING]
> **Reasoning is not authorization.** An agent judging an action useful does not by itself grant permission to move assets, sign transactions, expose credentials or perform other consequential operations.

Sensitive workflows use explicit confirmations, scoped credentials, least-privilege tool access and auditable execution boundaries.

---

## Architecture

<sub>Platform</sub>

> A layered technical architecture: intelligence, orchestration, tools and Base infrastructure.

Qaa Si is a layered system, so intelligence, application logic, authorization and blockchain execution can each change independently.

`User / Application` → `Agent orchestration` → `Intelligence & tools` → `Policy & permissions` → `Execution` → `Base & external services` → `Verification & result`

### 1. Intelligence layer

Coordinates language models, task reasoning, contextual retrieval and agent-specific instructions. Model output is a decision input, not an authorization primitive.

### 2. Agent orchestration

Maintains objectives, task state and tool selection, and handles retries, intermediate results and workflow progression.

### 3. Tools & integrations

Agents can be extended through explicitly authorized APIs, applications and data sources. Each integration defines the data it can access and the actions it can perform.

### 4. Policy & permissions

Decides whether a proposed action is allowed, requires confirmation or must be blocked. This boundary matters most for wallets, credentials and external side effects.

### 5. Blockchain layer

Planned around Base. Possible on-chain components include token functionality, smart-contract interactions, treasury operations and other ecosystem mechanisms, once finalized.

### Security boundary

| Decision | Responsible layer |
|---|---|
| What action could solve the task? | Agent reasoning |
| Which tool could perform it? | Orchestration |
| Is the action permitted? | Policy / authorization |
| Was it executed successfully? | Execution + verification |

This separation reduces the risk of treating model output as an unrestricted command channel.

---

## Built on Base

<sub>Platform</sub>

> The planned Base blockchain foundation and how official deployments will be verified.

Qaa Si is planned to use Base for future on-chain components. Blockchain infrastructure offers transparent settlement, token ownership and auditable smart-contract state. Plans and actually deployed, verified contracts are always kept apart.

### Deployment information

| Item | Publication standard |
|---|---|
| Network / chain | Exact network identification and deployment environment |
| Token contract | Official address and verified explorer reference |
| Smart contracts | Contract purpose, version and administrative permissions |
| Treasury | Official addresses and documented control model |
| Vesting | Contract addresses, allocation rules and unlock mechanics |
| Liquidity | Pool or position information and any lock mechanism |

### Verification model

1. **Official publication:** a deployment detail is released through verified Qaa Si documentation or another official channel.
2. **On-chain verification:** users can independently inspect the contract or transaction on Base.
3. **Documentation match:** address, version and described permissions must match the deployed implementation.

> [!CAUTION]
> No token contract, treasury address or liquidity claim is official just because it uses the Qaa Si name. Always check against the official documentation first.

---

## Security & Transparency

<sub>Platform</sub>

> Security boundaries, contract transparency and verification standards.

Security documentation is treated as part of the product specification, not as a marketing claim.

### Security model

| Area | Principle |
|---|---|
| Agent permissions | Agents receive only the tools and access needed for the current task. |
| Consequential actions | Wallet, credential and external side-effect operations need explicit authorization boundaries. |
| Secrets | Sensitive credentials are not exposed to unnecessary components or stored without a defined need. |
| Verification | Execution results are checked before a workflow is reported as complete. |
| On-chain controls | Administrative permissions and control mechanisms are documented for deployed contracts. |

### Token and contract transparency

After deployment the documentation identifies the official token contract, relevant administrative permissions, treasury addresses and the contracts responsible for vesting or liquidity management.

### Team token vesting

Team allocations follow a defined vesting structure. Final allocation, cliff, unlock frequency and duration are published once tokenomics are finalized.

### Liquidity

If liquidity is described as locked, the lock provider or mechanism, the position or transaction identifiers and the lock duration are published so the claim can be verified.

### Audits

An audit is labelled **completed** only when a genuine third-party report exists, stating its scope, date and the contract version reviewed.

> [!WARNING]
> An audit reduces specific classes of risk but does not guarantee that a contract, protocol or economic mechanism is risk-free.

### AI-agent security

- Permission boundaries
- Tool restrictions
- Transaction authorization
- Protection of sensitive credentials
- Resistance to prompt injection
- Explicit confirmation for consequential operations

---

## Token & Utility

<sub>Token</sub>

> Token allocation, liquidity structure and the planned vesting framework.

> [!NOTE]
> **Current framework.** Total supply is 1,000,000,000 tokens and the allocations add up to 100%. Vesting, wallet and lock details are shown at the level currently defined; exact dates, addresses and parameters are added once finalized.

### Token allocation

| Allocation | Share | Tokens |
|---|---|---|
| Liquidity Pool | 50% | 500,000,000 |
| Future Liquidity Reserve | 10% | 100,000,000 |
| Staking Rewards | 5% | 50,000,000 |
| Community / Airdrops | 7% | 70,000,000 |
| Team | 3% | 30,000,000 |
| Ecosystem / Development | 10% | 100,000,000 |
| Marketing / Growth | 5% | 50,000,000 |
| Treasury | 10% | 100,000,000 |
| **Total** | **100%** | **1,000,000,000** |

Half of the total supply goes to the primary liquidity pool. Future liquidity, staking incentives and treasury reserves are kept as separate, identifiable allocations.

### Liquidity structure

| Item | Share | Tokens | Planned treatment |
|---|---|---|---|
| Liquidity Pool | 50% | 500,000,000 | DEX liquidity, intended to be secured by a publicly verifiable liquidity lock once the pool is created. |
| Future Liquidity Reserve | 10% | 100,000,000 | Reserved only for future liquidity needs; every deployment is documented beforehand (wallet source, amount, paired asset, transaction references). |

Deploying liquidity requires both sides of the trading pair. Final pool composition, paired ETH, initial price, pool address, LP position and lock evidence are final only once deployed and publicly verifiable.

> [!NOTE]
> Liquidity supports market depth but does not guarantee price stability, trading depth or protection from volatility.

### Staking rewards

The 5% allocation (50,000,000 tokens) is reserved for potential staking incentives. Reward mechanics, eligibility, duration, emission rate and the smart contract are only presented as active once finalized, deployed and verifiable.

> [!WARNING]
> This allocation is not a promise of yield or return. Any staking program will publish its own terms, contract details and risk disclosures.

### Locking, vesting & custody

| Allocation | Planned control framework |
|---|---|
| Liquidity Pool (50%) | LP position planned to be locked via UNCX or another publicly verifiable lock; details published once created. |
| Future Liquidity Reserve (10%) | Kept separate from operational wallets, preferably in multisig custody until used for documented liquidity purposes. |
| Staking Rewards (5%) | Held in a dedicated wallet or smart contract; distributed only under published staking rules once implemented. |
| Team (3%) | Full allocation planned to be locked via PinkLock: 6-month cliff, then 12 months of vesting. |
| Community / Airdrops (7%) | Distributed under published campaign rules and schedules; undistributed balances stay traceable on-chain. |
| Ecosystem / Development (10%) | Planned 12-month cliff, then 12 months of vesting; multisig recommended for custody. |
| Marketing / Growth (5%) | Planned 6-month cliff, then 12 months of vesting; multisig recommended for custody. |
| Treasury (10%) | Multisig custody with publicly documented control policies; a release schedule may be added once finalized. |

### Wallet & lock verification

Wallet addresses, pool address, multisig addresses, staking contracts, lock records and BaseScan links are added once they exist. All entries are currently **TBD**.

| Allocation | Address | Lock / custody | BaseScan |
|---|---|---|---|
| Liquidity Pool | TBD | UNCX lock link TBD | TBD |
| Future Liquidity Reserve | TBD (multisig) | TBD | TBD |
| Staking Rewards | TBD | TBD | TBD |
| Team | TBD | PinkLock vesting link TBD | TBD |
| Community / Airdrops | TBD | TBD | TBD |
| Ecosystem / Development | TBD (multisig / vesting) | TBD | TBD |
| Marketing / Growth | TBD (multisig / vesting) | TBD | TBD |
| Treasury | TBD (multisig) | TBD | TBD |

Reference tools: [UNCX](https://app.uncx.network/) · [PinkLock](https://www.pinksale.finance/pinklock/) · [BaseScan](https://basescan.org/)

### Utility framework

Potential utility areas: ecosystem access, agent-related services, staking incentives, governance or other platform mechanisms with a defined technical role. Each utility claim must map to an implemented product function or smart-contract mechanism.

### Security audit

A CertiK smart-contract audit and security review is planned after the token contract is created and finalized. *(Status: Planned)*

### Transparency standard

Before launch the documentation should publish:

- Official token contract
- Allocation wallets
- Liquidity-pool details
- Future-liquidity reserve address
- Staking details, where applicable
- UNCX lock evidence
- PinkLock verification links
- Multisig addresses
- BaseScan verification links
- Vesting contracts or schedules
- Official security-audit report, where applicable

> [!WARNING]
> Nothing here is a promise of price appreciation, yield or investment return. Utility describes intended ecosystem function, not market performance.

---

## Audit & Certification

<sub>Token</sub>

> Security verification for the token and related smart contracts: automated scans and a planned independent audit.

### Automated security scans

Planned once the final token contract is deployed and verified. Public report links are added when available.

| Verification | Purpose | Status |
|---|---|---|
| GoPlus DeepScan | Automated token and contract risk checks, incl. permissions and common token risks. | Planned · after deployment |
| TokenSniffer | Public token risk and contract checks. | Planned · after deployment |
| Audit Forge | Automated Solidity security analysis and pre-audit checks. | Planned · before / after deployment |
| Web3defender | Additional token and wallet security checks. | Planned · after wallets & token are live |

> [!NOTE]
> These are automated scans, not independent manual audits or certifications. Every completed scan will be linked publicly.

### Independent audit

| Independent review | Status | Report |
|---|---|---|
| CertiK or comparable independent auditor | Planned · after contract creation | TBD |

Expected scope: the final token contract and any other security-critical contracts at launch. Once completed, auditor, report, scope, completion date and verification link are listed here.

> [!WARNING]
> A contract is only called audited or certified when an official, independently verifiable report exists. Automated scan results stay labelled as automated checks.

### Verification standard

- Deployed contract on BaseScan
- Automated scan results
- Relevant wallet verification records
- Any future independent audit report

---

## Roadmap

<sub>Project</sub>

> Product, infrastructure and ecosystem milestones, not price targets. Dates are shown only where there is a real development commitment.

#### Phase 1 · Foundation

*Status: In development*

- Brand and documentation system
- Core product architecture
- Agent model and permission principles
- Base infrastructure planning
- Security and transparency framework

#### Phase 2 · Product development

*Status: In development / planned*

- Agent workflows and orchestration
- User-facing application interfaces
- Tool and data integrations
- Permission and confirmation systems
- Testing, observability and verification workflows

#### Phase 3 · On-chain deployment

*Status: Planned*

- Finalize token and contract architecture
- Deploy and verify smart contracts
- Implement vesting and treasury controls
- Establish liquidity infrastructure where applicable
- Publish authoritative contract and treasury references

#### Phase 4 · Ecosystem expansion

*Status: Planned*

- Additional specialized agents
- Broader integrations and developer capabilities
- Community and ecosystem features
- Governance mechanisms, if implemented and technically justified

> [!NOTE]
> Roadmap items show intended sequencing, not guaranteed delivery dates. The documentation is updated as milestones move from planned to implemented.

---

## Risks & Disclaimer

<sub>Project</sub>

> Technical, economic and operational risks of AI agents and blockchain systems.

Qaa Si combines AI, external software integrations and blockchain systems; each adds material technical, operational and economic risk.

### Key risk categories

| Risk | Description |
|---|---|
| AI reliability | Models can produce incorrect, incomplete or misleading outputs. |
| Tool execution | External APIs or integrations can fail, change behaviour or return unexpected results. |
| Smart contracts | Deployed code can contain defects, vulnerabilities or unintended economic behaviour. |
| Wallet security | Lost keys, compromised credentials or malicious signing requests can cause irreversible loss. |
| Blockchain infrastructure | Congestion, outages, bridge failures or network-level events can disrupt operations. |
| Liquidity & volatility | Digital-asset markets can see extreme price swings and limited liquidity. |
| Regulatory change | Laws, classifications and compliance obligations can change across jurisdictions. |

### User responsibility

Users should assess the relevant risks independently, verify official contract information and understand the consequences of transactions before interacting with any blockchain component.

> [!CAUTION]
> Never send funds or sign transactions based only on an unverified address, social-media post, direct message or third-party listing. Confirm official deployment information against this documentation.

### Disclaimer

- Nothing in this documentation is financial, investment, legal or tax advice.
- Digital assets are highly volatile and may lose part or all of their value.
- References to planned features, token utility or roadmap items are forward-looking and not guarantees of delivery or economic outcome.
