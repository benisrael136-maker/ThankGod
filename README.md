# ThankGod
Overview

This project implements a secure Escrow Smart Contract in Clarity for the Stacks blockchain using Clarinet. The contract enables safe transactions between two parties (payer and payee), ensuring funds are only released when both sides agree.

To bridge business insights into Web3, this contract can be integrated with Google Analytics / Clarity tracking to log user events (wallet connect, escrow deposit, release, refund). This helps businesses monitor customer interactions, detect drop-offs, and improve the user experience.

✨ Features

🔒 Escrow Security: Funds are locked on-chain until released or refunded.

🛡 Fraud Prevention: Only the original payer can release or refund.

📊 Analytics-Ready: Hook frontend events into Google Analytics or Microsoft Clarity.

🖥 Transparency: On-chain, auditable transactions.

⚡ Developer-Friendly: Easy to test with Clarinet, extendable for business use cases.

🛠 Contract Functions

(create-escrow escrow-id payee amount)

Creates a new escrow with payer as tx-sender.

(deposit escrow-id)

Allows the payer to deposit the agreed STX.

(release escrow-id)

Payer releases escrow funds to payee.

(refund escrow-id)

Payer refunds funds to themselves if not yet released.

(get-escrow escrow-id)

Returns escrow details.

🖥 Example Workflow

Payer creates escrow with a payee and amount.

Payer deposits funds into escrow.

Funds are locked until action is taken.

Release (to payee) or Refund (to payer).

Analytics tracking logs events such as wallet_connect, deposit_success, release_success.
