## Hi, I'm Eidon 👋

I build **read-only evidence and diagnostics tooling for AI agents on Web3** — CLI-first, no private keys, no auto-payments, JSON output, `PASS / FAIL / UNKNOWN`, and every tool documents what it does *not* cover.

### 🔍 Agent / Chain Evidence Tools

| Tool | Question it answers | Install |
|---|---|---|
| [mcpdoctor](https://github.com/xka0085-byte/mcp-doctor) | Is your MCP/x402 endpoint discoverable by an agent? (402 docs, initialize, tools/list, schemas) | `npx @eidonze/mcpdoctor inspect <url> --json` |
| [x402-reconcile](https://github.com/xka0085-byte/x402-reconcile) | What does an x402 endpoint demand? (scheme, network, asset, amount, payTo) | `npx x402-reconcile inspect <url> --json` |
| [oauthdoctor](https://github.com/xka0085-byte/oauthdoctor) | Does your MCP server advertise OAuth metadata agents can discover? | `npx oauthdoctor inspect <url> --json` |
| [wallet-evidence](https://github.com/xka0085-byte/wallet-evidence) | What does one Solana RPC actually see in this transaction? (says UNKNOWN, never "doesn't exist") | `npx wallet-evidence inspect <sig> --json` |
| [crosschain-incident](https://github.com/xka0085-byte/crosschain-incident) | Normalize cross-chain message incident exports into evidence reports | `npx crosschain-incident inspect --input <json>` |

### 🧾 ReceiptRail — on-chain delivery receipts for x402

Payment → delivery → SHA-256 digest anchored into a Solana PDA → anyone verifies independently, without trusting the seller. Live MCP endpoint, core conformance verified.

- 🌐 https://agenttoll-receipts.app.workbuddy.host
- 🔎 MCP: `https://agenttoll-receipts.app.workbuddy.host/mcp`
- 📦 [Glama listing](https://glama.ai/mcp/servers/xka0085-byte/agenttoll) · [Repo](https://github.com/xka0085-byte/agenttoll)

### 🧰 Suite index

**https://x402-endpoint-inspection.app.workbuddy.host/tools.html**

I also do manual x402 endpoint conformance inspections (payment-to-delivery path, markdown report in 24h): https://x402-endpoint-inspection.app.workbuddy.host/
