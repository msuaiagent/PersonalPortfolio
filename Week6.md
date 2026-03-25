# Week 5 — Contact Form + Email Integration (Resend)

By this point, you should have a working portfolio website built in **v0.dev**.

This week, you are going to take your project from “just a website” → to a **real, interactive application** by allowing users to contact you directly through your site.

---

## 🎯 Goals for This Week

By the end of this week, you will:

* Move your project from v0.dev into a local development environment (Cursor/Vs-Code)
* Open and run your project in **Cursor**
* Install dependencies using npm
* Create a **Resend account**
* Use AI to implement a **fully working contact form**
* Receive real emails from your portfolio website

---

# 🧱 Part 1 — Download and Set Up Your Project

## Step 1 — Download from v0.dev

Download your project from **v0.dev** as a `.zip` file.

---

## Step 2 — Create a Project Folder

You must organize your files properly.

1. Create a new folder on your computer
   Example:

```bash
my-portfolio-site
```

2. Move the `.zip` file into that folder
3. Unzip the contents **inside that folder**

---

## ✅ Check Your Folder

Make sure your folder contains files like:

* `package.json`
* `app/`
* `components/`
* `public/`

⚠️ If you do NOT see `package.json`, you opened the wrong folder.

---

# 💻 Part 2 — Open in Cursor

1. Open **Cursor**
2. Click **Open Folder**
3. Select your project folder

---

# 📦 Part 3 — Install Dependencies

Open the terminal in Cursor and run:

```bash
npm install
```

This installs everything your project needs.

---

## ❗ If npm does not work

Go back to **Week 1–2 setup instructions** and finish your environment setup.

---

# ▶️ Part 4 — Run Your Project

Run:

```bash
npm run dev
```

Then open:

```bash
http://localhost:3000
```

Make sure your site works before continuing.

---

# ✉️ Part 5 — Create a Resend Account

You will use Resend to send emails from your website.

👉 [Create a Resend account](https://resend.com?utm_source=chatgpt.com)

---

## Get Your API Key

1. Go to the dashboard
2. Click **API Keys**
3. Click **Create API Key**
4. Copy your key

---

# 🤖 Part 6 — One-Shot AI Implementation

Now we will use **Cursor AI** to build the entire contact form system in one prompt.

---

## 🔥 Paste This Prompt Into Cursor

```text
You are a senior Next.js engineer.

I have a portfolio website generated from v0.dev that is already set up locally in Cursor and running with npm.

Your task is to implement a COMPLETE contact form email feature using Resend.

This must be a one-shot implementation. Do not leave anything incomplete.

========================
CONTEXT
========================

This project already exists.
Do NOT rebuild the website.
Do NOT redesign the UI.
Do NOT change unrelated code.

I only want the minimum code changes needed to make the contact functionality work.

Before making changes, inspect the codebase and determine whether a contact form already exists in the footer.

- If a footer contact form already exists, DO NOT create a new one
- Instead, connect the existing inputs/button to the email functionality
- If a contact form does not already exist in the footer, add one there using the site's existing design system and styling patterns

========================
REQUIREMENTS
========================

You must:

1. Add a contact form UI ONLY IF one does not already exist in the footer
2. If the form already exists, wire up the existing inputs and submit button
3. Create a backend API route to handle form submissions
4. Integrate Resend to send emails
5. Use environment variables correctly
6. Keep everything beginner-friendly and minimal

========================
FORM REQUIREMENTS
========================

The contact form must include:
- Name input
- Email input
- Message textarea
- Submit button

UX requirements:
- Disable the button while sending
- Show a loading state while submitting
- Show a success message after submission
- Show an error message if submission fails

========================
BACKEND REQUIREMENTS
========================

- Use a Next.js API route appropriate to the project structure
- Handle POST requests only
- Parse the request body correctly
- Validate required inputs
- Reject empty fields
- Use Resend to send an email to process.env.CONTACT_EMAIL
- Use async/await
- Handle errors cleanly

========================
EMAIL CONTENT
========================

The email must include:
- sender name
- sender email
- message

The email should be formatted professionally and clearly indicate that someone visited the portfolio website and wants to get in contact.

========================
ENVIRONMENT VARIABLES
========================

Create a `.env.local` file in the root of the project if it does not already exist.

Ensure it contains exactly:

RESEND_API_KEY=YOUR_API_KEY_HERE
CONTACT_EMAIL=your_email@gmail.com

Do NOT hardcode secrets anywhere else.
Do NOT expose secrets in frontend code.

Use:
- process.env.RESEND_API_KEY
- process.env.CONTACT_EMAIL

========================
RESEND IMPLEMENTATION
========================

- Use the official resend npm package
- Import and initialize it correctly
- Keep the implementation minimal and clear
- Do not add unnecessary dependencies

========================
PROJECT INTEGRATION RULES
========================

- Do NOT rebuild the site
- Do NOT redesign components
- Only make the minimum changes needed
- Match the current design system
- Reuse existing code patterns where possible
- Keep code modular and readable
- Only add handlers, state, API integration, and minimal UI feedback needed for submission
- Preserve the existing look and layout

========================
OUTPUT FORMAT
========================

Return your answer in this exact format:

1. Summary of what is being added
2. Files to create
3. Files to edit
4. Full code for ALL new files
5. Exact code changes for existing files
6. Instructions to install dependencies
7. Instructions to test locally
8. Common errors and how to fix them

========================
FINAL REQUIREMENTS
========================

The final result must:
- work immediately after copy-pasting code
- require zero additional architecture decisions
- be fully beginner-friendly
- not break the existing portfolio

After providing the code, clearly remind me to:

1. paste my real Resend API key into `.env.local`
2. replace CONTACT_EMAIL with my real email address
3. restart the dev server with `npm run dev`
```

---

# 🔑 Part 7 — Add Your API Key

After Cursor generates the code:

1. Open `.env.local`
2. Replace:

```bash
RESEND_API_KEY=YOUR_API_KEY_HERE
CONTACT_EMAIL=your_email@gmail.com
```

with your real values.

---

# 🔁 Part 8 — Restart Your App

```bash
npm run dev
```

---

# 🧪 Part 9 — Test Your Contact Form

Go to your website and submit the form.

You should:

* See a loading state
* See a success message
* Receive an email in your inbox

---

# ⚠️ Common Mistakes

### ❌ Opened wrong folder

Make sure `package.json` is in your root folder.

### ❌ Forgot npm install

Run:

```bash
npm install
```

### ❌ `.env.local` in wrong place

Must be in root (same level as `package.json`)

### ❌ Forgot to restart server

Always restart after editing `.env.local`

### ❌ API key exposed

Never put your API key in frontend code

---

# ✅ Final Deliverable

You are done when:

* Your site runs locally
* You have a working contact form
* Emails are sent to your inbox
* `.env.local` is configured correctly
* Code is pushed to GitHub

---

# 💡 Why This Matters

This is where your project becomes **real-world ready**.

You are no longer just displaying information.

You now have a website that:

* accepts input
* communicates with a backend
* sends real emails

That is a **full-stack feature**.

---
