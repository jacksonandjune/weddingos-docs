# Package Setup

Packages are the foundation of your proposals and contracts in WeddingOS. Each package has a name, price, inclusions list, and contract text. You can have as many packages as you need.

To manage packages, go to **Settings > Packages**.

---

## Creating a package

Click **+ New Package** and fill in:

| Field | Notes |
|---|---|
| **Name** | What clients and planners will see (e.g. "Full Planning", "Day-Of Coordination") |
| **Pricing type** | Fixed (flat rate) or Percentage (percent of wedding budget) |
| **Base price** | The default price shown when building a proposal |
| **Description** | A short summary shown internally |

Save to create the package, then add your inclusions and contract text.

---

## Inclusions text

The inclusions list is the "what you get" section of the proposal. Clients see this when reviewing and signing.

Write this in the **Proposal Inclusions** editor. You can use formatting (bold, bullets, line breaks). Template variables like `{{CLIENT_NAME}}` and `{{WEDDING_DATE}}` are supported and get filled in automatically when the proposal is sent.

---

## Contract text

The contract is the legal agreement the client signs. It appears below the inclusions on the signing page.

Write this in the **Contract Text** editor. Use template variables to personalize it automatically:

- `{{CLIENT_NAME}}` -- primary client's full name
- `{{FIANCE_NAME}}` -- partner's full name
- `{{WEDDING_DATE}}` -- wedding date
- `{{VENUE}}` -- venue name
- `{{TOTAL_PRICE}}` -- total contract value
- `{{COMPANY_NAME}}` -- your business name
- `{{PLANNER_NAME}}` -- assigned planner's name

The full variable list is shown in the reference panel next to the editor.

> Contract text is snapshotted at the time a proposal is sent. Changes you make after sending don't affect proposals already out.

---

## Editing a package

Click any package to open it and edit any field. Changes to price, inclusions, or contract text take effect on future proposals only.

---

## Deactivating a package

If you no longer offer a package, you can deactivate it. Deactivated packages won't appear when building new proposals, but existing clients on that package are unaffected.
