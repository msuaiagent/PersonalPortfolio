# 💼 AI Club — Week 3

## LaTeX Resume → Structured JSON → Developer Workflow

---

# 🎯 Goal of Week 3

Last week you made your resume:

* Professional
* LaTeX-based
* Version controlled

This week, we transform it into:

* Structured data
* Machine-readable format
* API-ready JSON
* Git-tracked file

By the end of today, you will have:

* `resume.json`
* A validated structured dataset
* A GitHub repo showing real commits
* An understanding of why structure matters in real systems

---

# 🧠 Recap: Where We Are in the System

Week 1:

```
Resume → LaTeX → GitHub
```

Week 2:

```
LaTeX → Structured JSON → Data Engineering Thinking
```

This week:

```
JSON → Website → Deployment
```


# 🧩 Why Structured Data Matters

Your LaTeX resume is:

* Beautiful
* Professional
* Human-readable

But it is NOT:

* Queryable
* Validatable
* Transformable
* Machine-operable

Real systems operate on structured data.

Everything in modern software flows through:

* JSON (Javascript Object Notation) 
* APIs (Application Program Interface)
* Databases
* Structured schemas

Today, your resume becomes data.

---

# ✅ Step 0 — Confirm Your Setup

From Week 1 you should already have:

* GitHub account
* VS Code installed
* Git installed
* LaTeX resume completed

If not — fix that first.

---

# ✅ Step 1 — Create a New Repo

In your VS-Code terminal:

```
mkdir resume-json
cd resume-json
git init
```

Create two files:

```
resume.json
README.md
```

---

# 🧠 Step 2 — Understand the Difference

Unstructured:

```
Worked at Google from 2022–2023 as a SWE.
```

Structured:

```json
{
  "company": "Google",
  "role": "Software Engineer",
  "start_date": "2022",
  "end_date": "2023"
}
```

Structured data:

* Can power websites
* Can feed AI
* Can be validated
* Can be version-controlled
* Can be transformed


---

# 🧠 Step 3 — Resume → JSON Prompt

We now force AI to behave like a strict parser.

Use this exact prompt:

---

### Resume → JSON Conversion Prompt

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

# ✅ Step 4 — Validate Before You Trust

Engineers validate outputs.

Go to:

[https://jsonlint.com/](https://jsonlint.com/)

Paste your JSON.

If it fails:

* Fix commas
* Fix brackets
* Adjust prompt
* Regenerate

Never blindly trust generated output.

---

# ✅ Step 5 — Save and Commit

In VS Code:

1. Paste JSON into `resume.json`
2. Format the file
3. Save

Then:

```
git add .
git commit -m "Add structured resume JSON"
```

Create a GitHub repo named:

```
Personal-Portfolio
```

Then push.

Your resume is now:

* Version controlled
* Structured
* Machine-usable

---

# 🧠 Why This Is Powerful

Now that your resume is JSON, you can:

* Generate a website automatically
* Create tailored resumes per job
* Run AI skill-gap analysis
* Compare roles programmatically
* Feed into a backend system
* Build a resume parser
* Create a recruiter dashboard

You just turned a PDF into an API-ready object.

That is real engineering thinking.

---

# 🧪 Stretch (Advanced)

Add:

```json
"meta": {
  "last_updated": "",
  "target_role": "",
  "years_experience": ""
}
```

Or create:

```
resume.schema.json
```

And define validation rules.

This is how production systems work.

---

# 📦 Deliverables

By the end of Week 3:

* ✅ resume.json
* ✅ GitHub repo with commits
* ✅ Validated JSON
* ✅ Understanding of structured outputs
* ✅ AI prompt discipline

---

# 🔜 Week 4 Preview

Next week:

```
resume.json → Dynamic Portfolio Website
```

* Parse JSON
* Generate HTML
* Deploy live
* Real dev workflow

We move from:

Resume editing → Data engineering → Web systems.
