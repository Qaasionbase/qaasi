# Qaa Si Updates

What we build, when we build it and how it works. Agent, code and website notes from the Qaa Si team, newest first.

> Also on the website: [qaasi.webflow.io](https://qaasi.webflow.io) → Updates

| # | Date | Area | Update |
|---|---|---|---|
| [006](#006--one-window-for-everything) | 10 Oct 2026 | Website | One window for everything |
| [005](#005--concierge-answers-with-a-status-label) | 03 Oct 2026 | Code | Concierge: answers with a status label |
| [004](#004--agentverse-and-access-requests) | 02 Oct 2026 | Agents | Agentverse and access requests |
| [003](#003--risk-engine-first-permission-check) | 30 Sep 2026 | Risk | Risk engine: first permission check |
| [002](#002--agent-lineup-aql-fxa-zen-and-custom) | 28 Sep 2026 | Agents | Agent lineup: AQL, FXA, ZEN and Custom |
| [001](#001--foundation-brand-website-and-docs) | 26 Sep 2026 | Website | Foundation: brand, website and docs |

**Status:** Pre-launch

---

## 006 · One window for everything

`10 Oct 2026` · `Website` · **Latest**

The new Qaa Si home: a full-screen hall with the Qaa Si logo. Clicking the logo opens one large glass window where every section lives, so visitors never leave the page.

- Agentverse, Documentation, Blog, Updates and Contact as tabs inside the window
- The full documentation readable in the window, without leaving the site
- Blog with the book-shelf animation and reads on superintelligence

```js
// window/tabs.js
// Every header link swaps the window content in place
function show(tab) {
  panels.forEach(p =>
    p.classList.toggle('is-active', p.dataset.panel === tab));
}
```

---

## 005 · Concierge: answers with a status label

`03 Oct 2026` · `Code`

The new Qaa Si Concierge answers questions from our documentation and shows whether each answer is a draft, planned or still pending.

- 14 topics grouped into Project, Token, Safety and Launch
- Every answer shows its source and a DRAFT / PLANNED / PENDING label
- Free-text questions are matched to the closest documented topic

```js
// concierge/answer.js
// Each answer carries its source and how certain it is
const answer = {
  topic:  'Locks & vesting',
  text:   'Planned locks: initial DEX liquidity via UNCX ...',
  source: 'Token & Utility / Locking & Vesting',
  status: 'PENDING',   // DRAFT | PLANNED | PENDING
};
```

---

## 004 · Agentverse and access requests

`02 Oct 2026` · `Agents`

Visitors can explore every agent and request access with a form that checks the wallet address before it is sent.

- Agent overview with AQL, FXA, ZEN and Custom
- Access form: wallet, name, email, agent and purpose
- Wallet input is checked for a valid Base address format

```js
// agentverse/access.js
// A Base address is 0x followed by 40 hex characters
const isBaseAddress = (value) =>
  /^0x[a-fA-F0-9]{40}$/.test(value.trim());
```

---

## 003 · Risk engine: first permission check

`30 Sep 2026` · `Risk`

The first design of the check that sits between an agent proposal and execution. An agent can propose, but only this layer can approve.

- Asset allow-list per account
- Position size and total exposure limits
- Every rejection returns a readable reason for the log

```js
// risk/approve.js
function approve(proposal, limits) {
  if (!limits.assets.includes(proposal.asset))
    return reject('asset not allowed');
  if (proposal.size > limits.maxPosition)
    return reject('position too large');
  return { status: 'approved', checkedAt: Date.now() };
}
```

> [!NOTE]
> Design draft. Logic and limits may change before launch.

---

## 002 · Agent lineup: AQL, FXA, ZEN and Custom

`28 Sep 2026` · `Agents`

We defined the first four agents and what each one is responsible for. Every agent works inside the same permission and risk framework.

- AQL for crypto markets and onchain trade preparation
- FXA for currency-pair analysis
- ZEN for explainable signals, plus Custom agents for your own strategy

```js
// agents/registry.js
export const agents = [
  { id: 'AQL',    market: 'crypto',  role: 'onchain analysis & trade prep' },
  { id: 'FXA',    market: 'forex',   role: 'currency-pair analysis' },
  { id: 'ZEN',    market: 'signals', role: 'explainable alerts' },
  { id: 'CUSTOM', market: 'any',     role: 'your strategy, your limits' },
];
```

---

## 001 · Foundation: brand, website and docs

`26 Sep 2026` · `Website`

The starting point: a clear brand, the first version of the website and our documentation, so everything we build next has one home.

- Brand colors: turquoise, deep teal, graphite and milk white
- Website structure with home, blog and documentation
- Journal articles on how trading agents work

```js
// brand/tokens.js
export const qaa = {
  turquoise: '#32cfc3',
  deepTeal:  '#168e87',
  graphite:  '#171a1b',
  milk:      '#f5f3ed',
};
```

---

<sub>Code samples show how parts of the system are designed. They are simplified and may change before launch.</sub>
