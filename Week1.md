# PersonalPortfolioProject



---

# 🧠 AI Club — Week 1

## Resume → LaTeX → GitHub Foundations

---

## 🎯 Goal of Week 1

By the end of this workshop, you will have:

* A **GitHub account**
* A **VS Code setup**
* A resume converted into **LaTeX using Jake’s Overleaf template**
* An AI-generated LaTeX resume you can **compile and edit**
* A foundational understanding of **AI-assisted workflows**

This is the foundation for everything we build this semester.

---

## ✅ Step 0 — Create a GitHub Account (Required)

Before doing *anything else*, create a GitHub account.

👉 [https://github.com/)

### Rules

* Use a **professional username**
* No random numbers or memes
* This will go on your resume

Good examples:

* `firstnamelastname`
* `firstname-lastname`
* `firstnameLastname`

❗ **You cannot proceed without GitHub**

---

## ✅ Step 1 — Install Required Tools

### 1. Install Visual Studio Code

👉 [https://code.visualstudio.com/](https://code.visualstudio.com/)

Open VS Code once installed.

---

### 2. Install Git

👉 [https://git-scm.com/downloads](https://git-scm.com/downloads)

Verify installation:

```bash
git --version
```

If you see a version number, you’re good.

---

## ✅ Step 2 — Open the Resume Template in Overleaf

We are using **Jake’s Resume Template**, a standard in tech.

👉 [https://www.overleaf.com/latex/templates/jakes-resume/syzfjbzwjncs](https://www.overleaf.com/latex/templates/jakes-resume/syzfjbzwjncs)

### Instructions

1. Click **Open as Template**
2. Sign in or create an Overleaf account
3. Do **NOT** manually edit yet


---

## ✅ Step 3 — Prepare Your Resume for AI

You need:

* Your current resume as a **PDF**
* Or resume text copied into plain text

Make sure your resume includes:

* Name + contact info
* Education
* Experience
* Projects
* Skills

---

## 🧩 Step 4 — The Resume-to-LaTeX Prompt (IMPORTANT)

You will paste **this exact prompt** into your AI tool.

---

### 📌 Resume → LaTeX Conversion Prompt

```text
You are an expert technical resume formatter.

Your task is to convert my resume into LaTeX using the exact structure and commands from Jake Gutierrez’s resume template.

STRICT RULES:
- Use ONLY the commands already defined in the template:
  - \resumeSubheading
  - \resumeItem
  - \resumeItemListStart / End
  - \resumeProjectHeading
- Do NOT introduce new LaTeX packas
- Preserve all information from my resume
- Do NOT invent or embellish experience
- Use concise, impact-driven bullet points
- Match sections to the template exactly:
  - Education
  - Experience
  - Projects
  - Technical Skills

OUTPUT FORMAT:
- Output ONLY valid LaTeX code
- Do NOT include explanations
- Do NOT include markdown
- Do NOT include commentary
- The output must be directly pasteable into Overleaf

INPUT RESUME:
[PASTE YOUR RESUME TEXT HERE]
```

---

## ✅ Step 5 — Paste Into Overleaf

1. Copy the AI-generated LaTeX
2. Go back to Overleaf
3. Replace the content **between**:

```latex
\begin{document}
...
\end{document}
```

4. Click **Recompile**

🎉 You now have a LaTeX resume.

---

## 🔧 Step 6 — Fix & Verify

Things to check:

* Does it compile?
* Are dates aligned correctly?
* Are bullets concise?
* Is it **1 page**?

You may:

* Adjust wording
* Shorten bullets
* Re-run the AI prompt with corrections

---

## ✅ Step 7 — Create a GitHub Repo (Optional but Recommended)

If 1. Create a new GitHub repo called:

   ```
   resume
   ```
2. Add:

   * `resume.tex`
   * `README.md`

This introduces **version control** for your resume.

---

## 📦 What You Should Have by the End

* ✅ GitHub account
* ✅ VS Code installed
* ✅ Git installed
* ✅ Overleaf account
* ✅ LaTeX resume compiled
* ✅ AI-assisted workflow experience

---

## 🔜 What’s Next (Week 2 Preview)

Next week:

* Resume → structured JSON
* Verifying AI outputs
* Using resumes as **data**
* Preparing for portfolio generation

---
