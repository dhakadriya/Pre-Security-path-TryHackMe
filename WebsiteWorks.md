# 🌐 How Websites Work  
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room introduces the fundamental concepts of how websites operate, including:

- Frontend vs Backend architecture  
- HTML basics  
- JavaScript fundamentals  
- Sensitive Data Exposure  
- HTML Injection  

Understanding these concepts is crucial for:

- Web Application Security  
- Bug Bounty Hunting  
- Penetration Testing  
- Secure Web Development  

---

# 🧠 Task 1 — How Websites Work

When you visit a website:

1. Your browser sends a request to a web server.
2. The web server responds with data.
3. Your browser renders the data into a webpage.

---

## 🏗 Website Components

| Component | Description |
|------------|------------|
| Front End (Client-Side) | Rendered by your browser |
| Back End (Server-Side) | Processes requests and returns data |

---

## ✅ Task 1 Answer

| Question | Answer |
|----------|--------|
| Component rendered by browser? | **Front End** |

---

# 🧩 Task 2 — HTML Basics

Websites are built using:

- **HTML** → Structure  
- **CSS** → Styling  
- **JavaScript** → Interactivity  

---

## 📄 Basic HTML Structure

html
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>
    <h1>Heading</h1>

## 🔎 Important HTML Concepts

| Element | Purpose |
|----------|----------|
| `<html>` | Root element |
| `<head>` | Page metadata |
| `<body>` | Visible content |
| `<h1>` | Heading |
| `<p>` | Paragraph |
| `<img>` | Image |
| `<button>` | Button |

---

## 🔐 Attributes

| Attribute | Purpose |
|------------|----------|
| `class` | Styling groups |
| `id` | Unique identifier |
| `src` | Image source |

---

## 🏁 Task 2 Flags

| Action | Flag |
|---------|------|
| Fix broken image | `HTMLHERO` |
| Add dog image | `DOGHTML` |

---

# ⚡ Task 3 — JavaScript Basics

JavaScript enables interactivity in web pages.

### 📌 Example
document.getElementById("demo").innerHTML = "Hack the Planet";

<button onclick='document.getElementById("demo").innerHTML = "Button Clicked";'>
Click Me!
</button>

🏁 Task 3 Flag
| Action | Flag |
| Change demo content	| JSISFUN |

##  Task 4 — Sensitive Data Exposure

Sensitive Data Exposure occurs when confidential information is visible in:

Page source

HTML comments

JavaScript files

🔎 During Recon, Always:

View Page Source

Check HTML comments

Look for credentials

Look for hidden endpoints

🏁 Task 4 Flag
Question	Answer
Hidden password in source?	testpasswd
💉 Task 5 — HTML Injection

HTML Injection occurs when:

User input is not sanitised

Input is rendered directly into the page

Browser interprets malicious HTML

🚨 Why It’s Dangerous

Page defacement

Malicious link injection

Potential JavaScript execution

🔐 Golden Rule

Never trust user input.

## 🏁 Task 5 Flag
| Action	| Flag |
| Inject malicious link |	HTML_INJ3CTI0N |

##  Skills & Concepts Practiced

Understanding frontend vs backend

Writing basic HTML

Manipulating DOM with JavaScript

Reviewing page source for secrets

Identifying sensitive data exposure

Performing HTML injection

##  Key Takeaways

Websites consist of frontend & backend components

HTML defines structure

JavaScript enables interactivity

Viewing page source is critical during reconnaissance

Sensitive data can be exposed in frontend code

User input must always be sanitised
