# Tracking Payments

WeddingOS tracks your full payment schedule for every client: what's been paid, what's coming up, and what's overdue. You can mark payments paid manually or let clients pay online via Stripe.

---

## The payment schedule

Every booked client has a Payments tab showing their full schedule. The schedule is created automatically when a proposal is signed, based on your payment schedule template.

Each row shows:
- Payment label (Deposit, Payment 2, Final Payment)
- Amount
- Due date
- Status: paid, pending, or overdue
- Payment method and paid date once marked paid

A progress bar at the top shows how much of the total has been collected.

---

## Marking a payment paid

For checks, cash, Zelle, Venmo, or anything paid outside of Stripe:

On the Payments tab, click **Mark Paid** next to any pending or overdue payment. You'll enter:

- **Paid date** -- defaults to today, edit if backdating
- **Payment method** -- check, cash, Zelle, Venmo, card, or Stripe
- **Notes** -- optional

Click **Save** and the payment flips to green. The activity log records who marked it and when.

---

## Online payments via Stripe

If your Stripe account is connected in Settings > Integrations, you can send clients an invoice link from the Payments tab, or let them pay directly from their Client Portal.

When a client pays through Stripe, the payment is automatically marked paid in WeddingOS.

See [Stripe Setup](../owner-admin/stripe-setup.md) for connection instructions.

---

## Overdue payments

WeddingOS flags a payment as **overdue** when its due date passes and it hasn't been marked paid. Overdue payments appear in red on the Payments tab and are surfaced on the admin dashboard.

You can mark an overdue payment paid the same way as a pending one.

---

## Editing a payment

To change the amount or due date on a pending payment, click the edit icon on that row. You can also edit the payment method on a paid payment by clicking the method displayed.

---

## Adding payments

To add a payment outside the standard schedule (for example, a custom add-on fee), click **+ Add Payment** at the bottom of the Payments tab.

---

## What clients see

Clients can view their payment schedule and pay online from their Client Portal. The portal shows the same progress bar and a **Pay Now** button on any unpaid payment if Stripe is connected.
