# Website Intake Form

WeddingOS gives you a hosted intake form you can embed on your website or link directly in your bio. When someone fills it out, a new lead is created in WeddingOS automatically.

---

## Getting your form link

Your intake form lives at a unique URL:

```
https://app.getweddingos.com/intake/[your-org-id]
```

Your org ID is visible in your account settings. You can link directly to this URL or embed it using an iframe on your website.

---

## What the form collects

By default the form asks for:

- First and last name
- Email address
- Phone number
- Wedding date
- Venue (if known)
- How they heard about you
- A message or notes field

You can turn individual fields on or off in **Settings > Intake Form**.

---

## Configuring the form

Go to **Settings > Intake Form** to:

- Toggle fields on or off
- Add custom questions (short text or long text)
- Set whether the lead source field is a free text box or a dropdown

The form automatically uses your agency name for the page title. Logo and brand color are pulled from your profile.

---

## What happens when someone submits

A new lead is created in WeddingOS with the information they provided. If auto-enroll is turned on in Settings > Email Templates, they are enrolled in your lead follow-up sequence immediately.

You'll see the new lead in your **Leads** list. No notification email is sent to you automatically -- check your leads list regularly or set a reminder to review new inquiries daily.

---

## Embedding on your website

To embed the form directly on a page of your website, use an iframe:

```html
<iframe
  src="https://app.getweddingos.com/intake/[your-org-id]"
  width="100%"
  height="800"
  frameborder="0">
</iframe>
```

Adjust the height as needed. The form is responsive and works on mobile.
