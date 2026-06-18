# Email Templates and Sequences

WeddingOS has two types of automated emails: the **lead follow-up sequence** and **proposal follow-up templates**. Both live in Settings > Email Templates.

---

## Lead follow-up sequence

When a new lead comes in, you can enroll them in a sequence of timed emails. WeddingOS sends these automatically based on how many days have passed since enrollment.

### Setting up the sequence

Go to Settings > Email Templates and look for the sequence emails. You can customize:

- **Subject line** -- include `{{firstName}}` to personalize
- **Body** -- use any of the available template variables
- **Send delay** -- the number of days after enrollment to send (e.g. day 2, day 5, day 10)
- **Active toggle** -- turn individual steps on or off without deleting them

### How enrollment works

There are two ways a lead gets enrolled:

1. **Auto-enroll** -- if auto-enroll is turned on in Settings > Email Templates, new leads are enrolled automatically when added (either manually or through your intake form)
2. **Manual enroll** -- toggle enrollment on the lead's profile, or from the three-dot menu in the Leads list

The enrolled icon (circular arrows) appears in the Leads list next to enrolled leads.

### When the sequence stops

The sequence stops automatically when:
- The lead's status changes from **Lead** to anything else (Consultation Scheduled, Booked, etc.)
- The lead replies to any email in the sequence

If you need to stop it manually, unenroll from the lead's profile or from the Leads list menu.

> Only enroll new, active leads who haven't heard from you yet. Do not enroll migrated contacts or anyone you've already been in conversation with -- they'll receive emails that won't make sense in context.

---

## Proposal follow-up templates

These emails go out automatically to leads who have received a proposal but haven't signed. WeddingOS checks daily and sends the right email based on how many days have passed since the proposal was sent.

Default steps are at day 3, day 5, and day 7. You can adjust the timing or turn individual steps off.

### How they stop

Proposal follow-ups stop when the lead signs their proposal or when their status changes.

---

## Template variables

Use these in any template subject or body:

| Variable | What it inserts |
|---|---|
| `{{firstName}}` | Lead's first name |
| `{{lastName}}` | Lead's last name |
| `{{weddingDate}}` | Wedding date |
| `{{venueName}}` | Venue name |
| `{{plannerName}}` | Assigned planner's name |
| `{{companyName}}` | Your business name |

---

## Tips

- Keep sequence emails short. These are follow-ups, not newsletters.
- Vary the tone across steps. Day 2 is warm, day 7 is a gentle closing note.
- Turn off any step you don't want to send rather than leaving a bad template active.
