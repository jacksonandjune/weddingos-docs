# Google Integration

Connecting Google syncs your email, calendar, and drive to WeddingOS. The connection is **per planner** — each person on your team connects their own Google account independently.

---

## What connecting Google enables

| Feature | What it does |
|---|---|
| **Gmail** | Bidirectional — send emails from your own Google address inside WeddingOS, and incoming replies sync back to the client's email thread automatically. Without Google connected, emails send from a system address instead of yours. |
| **Calendar** | Bidirectional — consultations and meetings you create in WeddingOS appear in your Google Calendar, and events in your Google Calendar appear in the client's Meetings tab. |
| **Drive** | WeddingOS automatically creates a client folder in Drive when a lead is marked Booked. Export documents from the Docs tab directly to that folder, and view any files stored there from the client detail page. |

---

## How to connect your Google account

1. Go to **Settings → Integrations**
2. Under **Google Workspace**, click **Connect Google**
3. You'll be redirected to Google — sign in and grant the requested permissions
4. You'll land back on the Integrations page with a **Connected** badge

Each planner on your team needs to do this individually. You can see who has connected on the **Settings → Team** page — look for the green Google badge next to each name.

---

## How Google Drive is organized

When a lead is marked **Booked**, WeddingOS automatically creates a dedicated folder for that client in Google Drive. This folder becomes the central place for everything related to that wedding — documents you export from WeddingOS, files your team uploads directly in Drive, vendor contracts, anything you want stored long-term.

You can view the contents of a client's Drive folder directly from their detail page in WeddingOS, without leaving the app.

**Setting a parent folder**

By default, client folders are created in the root of your Google Drive, which can get cluttered fast. We recommend creating a single folder in Drive (e.g., "WeddingOS Clients" or "Weddings 2026") and setting it as the parent — all new client folders will be created inside it, keeping your Drive organized automatically.

To set it up:

1. In Google Drive, create (or navigate to) the folder you want to use as the parent
2. Copy the folder ID from the URL: `drive.google.com/drive/folders/`**`[ID HERE]`**
3. Go to **Settings → Integrations** and paste the ID into **Client Folder Location**
4. Click **Save**

This is an org-wide setting — it applies to all planners. Existing client folders are not moved.

---

## Disconnecting Google

Go to **Settings → Integrations → Google Workspace** and click **Disconnect**. This removes access to Gmail, Calendar, and Drive for your account. Other team members' connections are unaffected.

If you reconnect later, your access is restored immediately.

---

## Troubleshooting

**Emails aren't sending from my Gmail address** — Make sure your Google account is connected under Settings → Integrations. Without it, emails go out from a system address.

**Drive folder wasn't created for a client** — The folder is created automatically when a lead's status changes to Booked. If the status was set before Google was connected, you can trigger folder creation manually from the client's detail page (Details tab → Create Drive Folder button).

**Team member doesn't see a Google badge on the Team page** — They haven't connected yet. Each planner connects at Settings → Integrations using their own login.

---

## For planners

You connect your own Google account independently — your admin doesn't do it for you. Here's what it unlocks and how to get set up.

**What you get when you connect:**
- Emails you send in WeddingOS come from your own Gmail address (not a generic system address)
- Replies from clients sync back into WeddingOS automatically
- Meetings and consultations you create in WeddingOS appear in your Google Calendar
- You can view client Drive folders and export documents to Drive from the client detail page

**To connect:**
1. Go to **Settings → Integrations**
2. Click **Connect Google** under Google Workspace
3. Sign in with your Google account and approve the permissions
4. You'll see a **Connected** badge when it's done

**To disconnect:**
Go to **Settings → Integrations** and click **Disconnect** under Google Workspace. Your teammates' connections are not affected.

**Emails still going out from a system address?** — Check that your Google account shows as Connected on the Integrations page. If it was recently reconnected, try sending a test email to confirm.
