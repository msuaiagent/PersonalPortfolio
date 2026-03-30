# Week 6: Deployment to Vercel + Environment Variables

## Objective

Deploy your portfolio to Vercel and configure environment variables so your contact form (Resend) works in production.

---

## Final Workflow

1. Push project to GitHub
2. Import repo into Vercel
3. Add environment variables
4. Redeploy project
5. Test live contact form

---

## Required Environment Variables

```bash
RESEND_API_KEY=your_resend_api_key_here
RESEND_FROM_EMAIL=your_verified_sender_email
```

---

## Local Setup (.env.local)

```bash
RESEND_API_KEY=your_resend_api_key_here
RESEND_FROM_EMAIL=your_verified_sender_email
```

⚠️ Do NOT commit `.env.local` to GitHub
make sure that you put .env.local and .env in the .gitignore file that is provided. This is so that our git version controller does not track your private api keys

---

## Step-by-Step Deployment

### 1. Push to GitHub

* Ensure your project runs locally
* Push all code to a GitHub repository

---

### 2. Import into Vercel

* Go to Vercel dashboard
* Click **Add New Project**
* Import your GitHub repo
* Let Vercel detect Next.js
* Deploy

---

### 3. Add Environment Variables in Vercel

* Go to **Project Settings → Environment Variables**
* Add:

  * `RESEND_API_KEY`
  * `RESEND_FROM_EMAIL`
* Apply to:

  * Production
  * Preview
  * Development (optional)

---

### 4. Redeploy

After adding env variables:

```bash
vercel --prod
```

OR redeploy from the dashboard

---

### 5. Test Contact Form

* Open deployed site
* Submit form
* Verify email is received

---

## Common Issues

* Missing `RESEND_API_KEY`
* Sender email not verified in Resend
* No redeploy after adding env variables
* Using env variable in client-side code

---

## Best Practices

* Keep API keys server-side only
* Never commit secrets to GitHub
* Use Vercel environment variables for production

---

## Final Checklist

```text
[ ] Project runs locally
[ ] Code pushed to GitHub
[ ] Repo imported into Vercel
[ ] Environment variables added
[ ] Project redeployed
[ ] Contact form works in production
```

---

## Week 6 Summary

Deploy your portfolio to Vercel, configure environment variables, redeploy the app, and verify that the contact form works in production.
