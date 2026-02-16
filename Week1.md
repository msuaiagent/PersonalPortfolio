> Resume → Structured Data → GitHub → Real Dev Workflow


---

#  AI Club — Week 2

## Resume → JSON → Structured Data Engineering

---

## 🎯 Goal of Week 2

By the end of this workshop, you will:

* Convert your LaTeX resume into structured JSON
* Learn how to prompt AI for structured outputs
* Validate JSON formatting
* Store your resume in a GitHub repository
* Understand why structured data matters in real systems

---

## 🧩 Why We’re Doing This

Your resume right now is:

* A PDF
* Or LaTeX
* Or a Word doc

That is **human-readable**, not machine-readable.

In real software systems:

* Frontends need JSON
* APIs send JSON
* Databases store structured data
* AI tools operate on structured formats

Today, your resume becomes **data**.

---

# ✅ Step 0 — Make Sure You Have

* GitHub account
* VS Code installed
* Git installed
* Your LaTeX resume from Week 1

If you don’t have these, stop and fix it.

---

# 🧠 Concept: Unstructured vs Structured

### ❌ Unstructured

```
Worked at Google from 2022–2023 as a SWE.
```

### ✅ Structured

```json
{
  "company": "Google",
  "role": "Software Engineer",
  "start_date": "2022",
  "end_date": "2023"
}
```

Structured data:

* Can be validated
* Can be transformed
* Can power websites
* Can feed AI systems

---

# ✅ Step 1 — Create a New GitHub Repo

Create a new repository using the terminal: 

Make sure git is installed 

Create a new folder
```
resume-json
```

Inside it, create these two files:

```
resume.json
README.md
```
Then we will run the command to initialize a repository:
```
git init 
```


---

# 🧠 Step 2 — The Resume → JSON Prompt

We are going to force AI to parse our resume into a structured prompt.

Use this prompt:

---

### 📌 Resume → JSON Conversion Prompt

```text
You are a strict data transformation engine.

Convert my resume into structured JSON.

STRICT RULES:
- Output ONLY valid JSON
- No markdown
- No commentary
- No explanation
- No trailing commas
- Keys must use snake_case
- All dates must be strings
- All bullet points must be arrays
- Do NOT invent information

Required JSON structure:

{
  "name": "",
  "contact": {
    "phone": "",
    "email": "",
    "linkedin": "",
    "github": ""
  },
  "education": [
    {
      "institution": "",
      "degree": "",
      "location": "",
      "start_date": "",
      "end_date": ""
    }
  ],
  "experience": [
    {
      "company": "",
      "role": "",
      "location": "",
      "start_date": "",
      "end_date": "",
      "bullet_points": []
    }
  ],
  "projects": [
    {
      "name": "",
      "technologies": [],
      "start_date": "",
      "end_date": "",
      "bullet_points": []
    }
  ],
  "technical_skills": {
    "languages": [],
    "frameworks": [],
    "tools": [],
    "libraries": []
  }
}

INPUT RESUME:
[PASTE LATEX OR PLAIN TEXT RESUME HERE]
```

---

# ✅ Step 3 — Validate the JSON

Before committing anything:

Go to:
👉 [https://jsonlint.com/](https://jsonlint.com/)

Paste your output.

If it fails:

* Fix commas
* Fix brackets
* Regenerate with prompt tweaks

Engineers validate. They don’t trust blindly.

---

# ✅ Step 4 — Save It Properly

In VS Code:

1. Paste into `resume.json`
2. Format document
3. Save

Then commit:

```bash
git add . 
git commit -m "Add structured resume JSON"
git push
```

Now your resume is version-controlled data.

---

# 🧠 Why This Matters

Once your resume is JSON, you can:

* Generate a portfolio site automatically
* Generate custom resumes per job
* Run AI analysis on skill gaps
* Compare roles
* Feed it into a backend system
* Train a model on resume data
* Build a resume parser

---

# 🧠 Step 5 — Improve It (Optional Advanced)

Add:

```json
"meta": {
  "last_updated": "",
  "target_role": "",
  "years_experience": ""
}
```


---

# 🧪 Stretch Exercise (If Time Allows)

Write a new AI prompt:

> “Given this resume.json, generate a 2-sentence professional summary tailored for a backend internship.”

This is now you using structured data intelligently to create structured outputs.

---

# 📦 What You Should Leave With

* ✅ resume.json
* ✅ GitHub repo
* ✅ Understanding of structured data
* ✅ AI prompting discipline
* ✅ Developer workflow experience

---

# 🔜 Week 3 Preview

Next week:

* Use resume.json to generate a portfolio site
* Auto-generate a personal website
* Deploy it live

---

If you want, next I can:

* Design Week 3 (JSON → website)
* Add a grading rubric
* Make this into a live demo script
* Add a TA checklist
* Turn this into a polished Google Slides deck

We just shifted them from “resume editing” to “data engineering thinking.”
