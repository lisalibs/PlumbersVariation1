# Formspree Setup Guide

Your contact form is now ready to use Formspree! Follow these simple steps:

## Step 1: Sign Up for Formspree (2 minutes)

1. Go to **https://formspree.io**
2. Click **"Sign Up"** (top right)
3. Enter **your email address** (this is where form submissions will be sent)
4. Create a password
5. Verify your email

## Step 2: Create Your Form (1 minute)

1. After logging in, click **"+ New Project"**
2. Name it: "ABC Plumbing Website"
3. Click **"+ New Form"**
4. Name it: "Contact Form"
5. **Copy the Form ID** - it looks like: `xyzabc12`

## Step 3: Update Your Website (30 seconds)

1. Open `index.html` in a text editor
2. Find this line (around line 1765):
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" id="contactForm">
   ```
3. Replace `YOUR_FORM_ID` with your actual form ID:
   ```html
   <form action="https://formspree.io/f/xyzabc12" method="POST" id="contactForm">
   ```
4. Save the file

## Step 4: Test It! (1 minute)

1. Open `index.html` in your browser
2. Fill out the contact form
3. Click **"Send Request"**
4. Check your email - you should receive the form submission!

## What You'll Receive

When someone submits the form, you'll get an email with:
- **Name**: Customer's name
- **Phone**: Their phone number
- **Email**: Their email address
- **Service**: What service they need
- **Message**: Their description

## Formspree Free Plan Includes:

- ✅ 50 submissions per month
- ✅ Email notifications
- ✅ Spam filtering
- ✅ File uploads (if you add them later)
- ✅ Dashboard to view all submissions

## Need More Submissions?

If you get more than 50 inquiries per month:
- **Formspree Gold**: $10/month for 1,000 submissions
- **Formspree Platinum**: $40/month for unlimited submissions

## Alternative: Use Your Own Email (No Formspree Account)

If you want to skip the signup, use **Web3Forms** instead:

1. Go to https://web3forms.com
2. Enter your email
3. Get an access key
4. Update the form action to:
   ```html
   <form action="https://api.web3forms.com/submit" method="POST">
   <input type="hidden" name="access_key" value="YOUR-ACCESS-KEY-HERE">
   ```

## Troubleshooting

**Form not working?**
- Make sure you replaced `YOUR_FORM_ID` with your actual ID
- Check that you verified your email in Formspree
- Open browser console (F12) to check for errors

**Not receiving emails?**
- Check your spam folder
- Verify email in Formspree dashboard
- Make sure the email address in Formspree is correct

## Support

- Formspree Docs: https://help.formspree.io
- Formspree Support: support@formspree.io

---

**That's it!** Your contact form is ready to receive customer inquiries and send them straight to your inbox.
