# Integrations

---

## Google

Connecting Google syncs your email, calendar, and drive to WeddingOS. The connection is **per planner** — each person on your team connects their own Google account independently.

### What connecting Google enables

| Feature | What it does |
|---|---|
| **Gmail** | Bidirectional — send emails from your own Google address inside WeddingOS, and incoming replies sync back to the client's email thread automatically. Without Google connected, emails send from a system address instead of yours. |
| **Calendar** | Bidirectional — consultations and meetings you create in WeddingOS appear in your Google Calendar, and events in your Google Calendar appear in the client's Meetings tab. |
| **Drive** | WeddingOS automatically creates a client folder in Drive when a lead is marked Booked. Export documents from the Docs tab directly to that folder, and view any files stored there from the client detail page. |

### How to connect your Google account

1. Go to **Settings → Integrations**
2. Under **Google Workspace**, click **Connect Google**
3. You'll be redirected to Google — sign in and grant the requested permissions
4. You'll land back on the Integrations page with a **Connected** badge

Each planner on your team needs to do this individually. You can see who has connected on the **Settings → Team** page — look for the green Google badge next to each name.

### How Google Drive is organized

When a lead is marked **Booked**, WeddingOS automatically creates a dedicated folder for that client in Google Drive. This folder becomes the central place for everything related to that wedding.

**Setting a parent folder**

By default, client folders are created in the root of your Google Drive, which can get cluttered fast. We recommend creating a single folder in Drive (e.g., "WeddingOS Clients") and setting it as the parent — all new client folders will be created inside it automatically.

To set it up:

1. In Google Drive, create (or navigate to) the folder you want to use as the parent
2. Copy the folder ID from the URL: `drive.google.com/drive/folders/`**`[ID HERE]`**
3. Go to **Settings → Integrations** and paste the ID into **Client Folder Location**
4. Click **Save**

This is an org-wide setting — it applies to all planners. Existing client folders are not moved.

### Consultation sync

When Google is connected, WeddingOS automatically detects new consultation bookings from your Google Calendar and updates lead status accordingly.

**How it works:** Once per day, WeddingOS checks your Google Calendar for newly added events. If an event's attendee email matches a lead in your system who is in **Lead** or **Contacted** status, their status automatically advances to **Consultation Scheduled** — including setting the consultation date, unenrolling them from any active email sequence, and logging the activity.

This means if a lead books directly through your **Google Calendar Appointment Booking page**, their CRM record updates automatically overnight. No manual status change needed.

### Disconnecting Google

Go to **Settings → Integrations → Google Workspace** and click **Disconnect**. This removes access to Gmail, Calendar, and Drive for your account. Other team members' connections are unaffected.

### Troubleshooting

**Emails aren't sending from my Gmail address** — Make sure your Google account is connected under Settings → Integrations. Without it, emails go out from a system address.

**Drive folder wasn't created for a client** — The folder is created automatically when a lead's status changes to Booked. If the status was set before Google was connected, you can trigger folder creation manually from the client's detail page (Details tab → Create Drive Folder button).

**Team member doesn't see a Google badge on the Team page** — They haven't connected yet. Each planner connects at Settings → Integrations using their own login.

---

## Calendly

If your team uses Calendly for consultation booking, you can connect it to get automatic lead status updates.

**What it does:** When a lead books through your Calendly link, their status in WeddingOS automatically advances to **Consultation Scheduled** — immediately, not on the next daily sync.

**How to connect:**
1. Go to **Settings → Integrations**
2. Under **Calendly**, click **Connect Calendly**
3. Sign in to your Calendly account and authorize the connection
4. Done — the webhook is registered automatically

**What happens on booking:**
- Lead status → Consultation Scheduled
- Consultation date stamped with the booked time
- Lead unenrolled from any active email sequence
- Activity logged on the lead's record

**On cancellation:** If a lead cancels their Calendly booking, a note is logged on their record but status is not automatically reverted — your planner reviews and decides next steps.

**Personal booking link:** You can save your personal Calendly URL under Settings → Integrations. Use `{{calendlyLink}}` in email templates to insert it automatically.

---

## Stripe

Connecting Stripe lets you send clients a direct payment link from their payment schedule. Instead of chasing checks or manual transfers, clients click a link and pay online — and WeddingOS automatically marks the payment as received.

### What Stripe enables

- **Send invoice links** directly from a client's Payments tab
- **Auto-reconcile payments** — when a client pays, their payment row updates to Paid automatically
- Stripe is connected once at the org level, so all planners can use it

### How to connect

1. Go to **Settings → Integrations**
2. Scroll to the **Stripe** section
3. Click **Connect Stripe**
4. You'll be redirected to Stripe to log in or create an account
5. Follow Stripe's prompts to connect your business account
6. Once complete, you'll land back in WeddingOS with a "Connected" confirmation

> If you don't have a Stripe account yet, you can create one during this flow — it takes about 5 minutes.

### Sending a payment link to a client

Once Stripe is connected:

1. Open a client's detail page and go to the **Payments** tab
2. Find the payment row you want to collect
3. Click **Send Invoice** — this generates a Stripe payment link and emails it to the client
4. When the client pays, the row automatically updates to **Paid**

### Disconnecting Stripe

1. Go to **Settings → Integrations**
2. Click **Disconnect** under the Stripe section
3. Confirm the prompt

> Disconnecting removes the ability to send new invoice links. Existing payments already collected are not affected.
