# Contracts

In WeddingOS, your contract is part of the proposal. Clients read and sign both in a single step. There is no separate contract workflow.

---

## Where your contract text lives

Contract text is stored per package in **Settings > Packages**. Each package has its own contract, so your Full Planning agreement can be different from your Day-Of agreement.

To edit: go to Settings > Packages, click the package, and scroll to the **Contract Text** section. The editor supports basic formatting.

---

## Template variables

Your contract text can include variables that WeddingOS fills in automatically when the proposal is sent:

| Variable | What it inserts |
|---|---|
| `{{CLIENT_NAME}}` | Primary client's full name |
| `{{FIANCE_NAME}}` | Partner's full name |
| `{{EVENT_NAME}}` | Event name (e.g. "Smith/Jones Wedding") |
| `{{WEDDING_DATE}}` | Wedding date |
| `{{VENUE}}` | Venue name |
| `{{TOTAL_PRICE}}` | Total contract value |
| `{{PACKAGE_NAME}}` | Package name |
| `{{COMPANY_NAME}}` | Your business name |
| `{{PLANNER_NAME}}` | Assigned planner's name |

The full list of available variables is shown in the panel next to the contract editor in Settings > Packages.

---

## How signing works

When you send a proposal, WeddingOS takes a snapshot of the contract text at that moment and saves it to the proposal record. Edits to your package contract later do not affect proposals that have already been sent.

The client receives a link to a page showing:
1. Package name and inclusions
2. Total investment and payment schedule
3. Full contract text

They type their name and click Sign. That name, the timestamp, and their IP address are recorded. A signed PDF is generated and saved to their Google Drive folder.

---

## After signing

The proposal status card on the client's profile shows **Signed** with a link to the signed PDF in Drive. Open that link to download it if you need to send the client a copy.

---

## If you don't use WeddingOS proposals

If you sign contracts outside of WeddingOS, the contract section won't appear on the client's profile. Everything else (payments, checklists, vendors, timeline) still works normally. See [Converting a Lead to Booked](converting-lead-to-booked.md) for how to book clients who signed offline.
