# agentlog-sdk
AgentLog: Audit & Compliance for Autonomous Agents

AgentLog provides an out-of-band audit layer for autonomous AI agents, ensuring enterprise-grade transparency and regulatory compliance (EU AI Act, SOC 2).

The Problem
Autonomous agents are "black boxes." When an agent makes a decision—executing a trade, updating a database, or sending a PII-sensitive email—there is often no immutable record of why it acted that way. This creates a massive liability for enterprises and makes audit compliance impossible.

The Solution
AgentLog acts as a "black box" flight recorder. It intercepts agent reasoning and actions in real-time, stores them in an immutable hash-chained log, and provides the necessary documentation for audit readiness.

Features
Immutable Audit Trail: Cryptographically hash-chained decision logs.

EU AI Act Readiness: Automated record-keeping for Article 50 requirements.

Behavioral Guardrails: Configurable kill-switches and risk scoring.

Zero-Overage Guarantee: Hard caps to ensure predictable enterprise billing.

Getting Started
Integrate AgentLog into your existing agent loop in minutes:

TypeScript
import { AgentLog } from '@agentlog/sdk';

const logger = new AgentLog({ apiKey: 'YOUR_API_KEY' });

// Record a decision/action for your audit trail
await logger.log({
  agentId: 'sales-bot-01',
  action: 'approve_transaction',
  reasoning: 'Customer provided valid proof of funds.',
  metadata: { transactionId: 'TXN-123' }
});


Security & Compliance
AgentLog is designed for high-risk environments in Fintech, Healthcare, and Cyber Security.

https://agentloghq.com/security

https://agentloghq.com/pricing
