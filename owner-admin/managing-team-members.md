# Managing Team Members

**Settings → Team** is where you build your roster and control who has access to WeddingOS. There are two distinct concepts here that work together:

- **Staff profiles** — everyone who can be assigned to a wedding (planners, coordinators, assistants). No login required.
- **Users with Login** — staff members who have a WeddingOS account. Logins are invitation-only.

This distinction matters: you might have a day-of assistant you want to assign to weddings and track labor costs for, but who doesn't need to log in themselves. Add them as a staff profile only. Your full-time planners who work in WeddingOS daily get both.

The page has three tabs: **Staff**, **Compensation**, and **Users with Login**.

---

## Staff Tab

### Adding a Staff Member

Click **+ Add Staff Member** and fill in:

| Field | Required | Notes |
|---|---|---|
| **Name** | Yes | Displayed everywhere they're assigned |
| **Role** | No | Their title (e.g. "Lead Coordinator", "Bride Buddy"). Shows on the team list and is used for compensation rate matching. |
| **Email** | No | For your records only — not used for login |
| **Compensation** | No | How they're paid per wedding (see below) |

**Compensation types:**
- **Flat $ per wedding** — a fixed dollar amount each time they're assigned (e.g. $500)
- **% of contract** — a percentage of the client's total contract value (e.g. 8%)
- **Monthly salary** — a fixed monthly amount, regardless of weddings worked

Click **Add Staff Member** to save. They'll immediately appear in the assignment dropdown on client records.

### Importing Staff from CSV

If you're migrating from another system or have a spreadsheet of your team, click **Import CSV**. Your file needs these columns (header names are flexible):

| Column | Accepted header names |
|---|---|
| Name | `name`, `full name`, `staff name` |
| Role | `role`, `title`, `job title`, `position` |
| Email | `email`, `email address` |
| Comp Type | `comp type`, `compensation type`, `pay type` |
| Comp Value | `comp value`, `rate`, `compensation`, `amount` |

For `comp_type`, use `flat` or `flat_rate` for flat per-wedding, and `%` or `percent` or `percentage` for percentage.

After uploading, you'll see a preview of the rows before anything is imported. Rows missing a name are flagged in red and will be skipped.

### Editing a Staff Member

From the Staff tab, click directly on any **Role** or **Compensation** value to edit it inline. Press Enter to save or Escape to cancel.

---

## Compensation Tab

The Compensation tab lets you set **org-wide default rates by role name**. These are used as the baseline when a staff member's individual comp rate is set to percentage with no fixed value.

For example: if "Bride Buddy" has a default of 5% of contract, any staff member with that role and no individual override will earn 5%.

To add a role rate, click **+ Add Role** and enter:
- **Role name** — must match the role title on the staff profile exactly (case-insensitive)
- **Type** — flat $ per wedding, or % of contract
- **Amount** — dollar amount or percentage (leave blank for "planner's own rate")

> Role comp rates only affect future assignments. Past assignments keep the rate that was recorded at the time they were assigned.

---

## Users with Login Tab

This tab shows everyone who has a WeddingOS account. For each user you can see their:
- **Profile** — their access level (Owner, Admin, or Planner) shown as a colored badge
- **Google** — whether they've connected their Google account (green = connected, red = not connected)
- **Joined** — when they accepted their invite

### Inviting a New User

Click **+ Invite Member** and fill in:

**Email** — the email address they'll use to log in.

**Profile** — their access level:
- **Admin** — full access to settings, proposals, all clients, and reports
- **Planner** — can view and work assigned clients; limited settings access

> To set fine-grained permissions (e.g. a planner who can also send proposals), use **Settings → Profiles** after they've accepted the invite.

**Link to existing staff profile** — if this person is already in your Staff tab (e.g. you added them manually or via CSV import), select their name here. This connects their login to their existing staff profile so their name appears correctly and their compensation history is preserved. If you leave this blank, a new staff profile is created automatically when they accept.

Click **Send Invite**. An email is sent to them with a link to set their password and activate their account. The invite link is valid for **30 days**.

### What Happens When They Accept

When the team member clicks the link in their invite email, they'll be prompted to set a password. Once complete, they're logged in and their account appears in the Users with Login list. Their profile (Admin or Planner) controls what they can see and do from day one.

---

## Frequently Asked Questions

**Can I change someone's profile (Admin vs. Planner) after they've joined?**
Yes — go to **Settings → Profiles** where you can change their role and set custom permission overrides.

**Someone left the team. How do I remove their access?**
Account removal isn't self-serve yet — contact WeddingOS support to deactivate a login. Their staff profile and any assignment history will remain intact.

**The invite expired. Can I resend it?**
Yes — generate a new invite from the Users with Login tab using the same email address. A fresh 30-day link will be sent.

**Do staff members without a login count toward my plan seat limit?**
No — only users with a login count as seats.

**Why does the Google column show red for some users?**
They haven't connected their Google account yet. They can do that themselves at **Settings → Integrations**. Google is required to send email from Gmail, sync Calendar events, and auto-create Drive folders.

---

*Next: [Roles and Permissions](roles-and-permissions.md)*
