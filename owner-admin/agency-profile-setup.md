# Agency Profile Setup

**Settings → Profile** is where you make WeddingOS your own — your branding, colors, and logo show up on every proposal, signed agreement, and email your clients receive. Spend five minutes here before you send your first proposal.

---

## What You Can Configure

| Setting | What It Controls |
|---|---|
| **Agency Name** | Appears on proposals, signed PDFs, email signatures, and notification emails |
| **Primary Color** | Accent color used on proposals, the sign page, and email headers (enter a hex code, e.g. `#4B5763`) |
| **Logo URL** | Your logo displayed at the top of proposals and client-facing emails |
| **Google Drive Parent Folder** | The Drive folder where client folders are automatically created when a wedding is booked |

---

## Step-by-Step

### 1. Open Profile Settings

From the left nav, go to **Settings → Profile**. You must be an **Owner** or **Admin** to access this page.

### 2. Set Your Agency Name

Enter your business name exactly as you want clients to see it. This is the name that appears:
- In the header of every proposal PDF
- In the "from" line of signing notification emails ("Your agreement with [Agency Name]")
- In the owner notification email when a client signs

### 3. Upload Your Logo

Paste the URL of your logo image. For best results:
- Use a PNG or SVG with a transparent background
- Recommended height: **48px** (will be displayed at that height on proposals)
- Host it somewhere publicly accessible (Google Drive public link, Squarespace, your website CDN)

> **Tip:** If your logo is in Google Drive, open the file → Share → "Anyone with the link" → copy the direct image URL.

### 4. Set Your Brand Color

Enter a hex color code that matches your brand (e.g. `#C8977E` for a dusty rose). This color appears as:
- The header/footer bar on proposal PDFs
- The signature button on the client sign page
- The accent line in signing confirmation emails

If you're unsure of your exact hex code, tools like [coolors.co](https://coolors.co) or your website's CSS can help you find it.

### 5. Connect Your Google Drive Folder (Optional)

If your team uses Google Drive to organize client files, you can set a **parent folder ID** here. When a client signs their proposal and gets marked as Booked, WeddingOS will automatically:
1. Create a new subfolder named `[First Name] [Last Name] Wedding` inside your parent folder
2. Upload the signed agreement PDF to that folder
3. Save the folder link on the client's record so your team can access it directly from WeddingOS

**To find your folder ID:** Open the folder in Google Drive. The ID is the long string at the end of the URL:
```
https://drive.google.com/drive/folders/1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs
                                        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
                                        This is your folder ID
```

Paste just the ID (not the full URL) into the Drive Parent Folder field.

> Note: Drive folder creation only works if the planner who sent the proposal has Google connected in **Settings → Integrations**.

### 6. Save

Click **Save Profile**. Changes take effect immediately on all new proposals.

---

## Frequently Asked Questions

**Does changing my brand color update existing proposals?**
No — proposals snapshot your branding at the time they're sent. Only new proposals will use the updated color.

**My logo isn't showing up on proposals. What's wrong?**
The logo URL must be publicly accessible. If it requires a login (e.g. a private Google Drive link), it won't load in the PDF generator. Try opening the URL in an incognito window — if it shows the image, it'll work.

**Can I have different branding for different planners?**
Not currently. Branding is org-wide — all planners on your team share the same logo, color, and agency name.

---

*Next: [Managing Team Members](managing-team-members.md)*
