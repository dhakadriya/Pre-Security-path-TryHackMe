# 🌐 HTTP & HTTPS Fundamentals  
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room covers the fundamentals of **HTTP (HyperText Transfer Protocol)** and **HTTPS (Secure HTTP)** — the core protocols that power web communication.

Topics Covered:

- HTTP vs HTTPS  
- URL Structure  
- HTTP Requests & Responses  
- HTTP Methods  
- HTTP Status Codes  
- Headers  
- Cookies  
- Practical HTTP Request Manipulation  

Understanding HTTP is essential for:

- Web Application Security  
- Bug Bounty  
- Penetration Testing  
- SOC Analysis  
- Traffic Inspection  

---

# 🧠 Task 1 — What is HTTP(S)?

## 🌍 HTTP (HyperText Transfer Protocol)

HTTP is the protocol used for transmitting web content such as:

- HTML  
- Images  
- Videos  
- CSS & JavaScript  

It was developed by **Tim Berners-Lee** between 1989–1991.

---

## 🔐 HTTPS (Secure)

HTTPS is the encrypted version of HTTP.

It provides:

- Data encryption  
- Protection from eavesdropping  
- Server authenticity verification  

---

## 🏁 Challenge Flag
THM{INVALID_HTTP_CERT}


---

## ✅ Task 1 Answers

| Question | Answer |
|----------|--------|
| What does HTTP stand for? | **HyperText Transfer Protocol** |
| What does the S in HTTPS stand for? | **secure** |

---

# 🔗 Task 2 — URLs & Requests

## 📌 What is a URL?

URL = **Uniform Resource Locator**

A URL instructs the browser how to access a resource.

Example:
http://user:password@tryhackme.com:80/view-room?id=1#task3

---

## 🧩 URL Breakdown

| Component | Description |
|------------|------------|
| Scheme | Protocol (HTTP, HTTPS, FTP) |
| User | Authentication credentials |
| Host | Domain or IP |
| Port | Communication port (80, 443, etc.) |
| Path | Resource location |
| Query String | Additional parameters |
| Fragment | Page anchor location |

---

## 📤 Example HTTP Request
GET / HTTP/1.1
Host: tryhackme.com
User-Agent: Mozilla/5.0
Referer: https://tryhackme.com/

---

## 📥 Example HTTP Response
HTTP/1.1 200 OK
Content-Type: text/html
Content-Length: 98

---

## ✅ Task 2 Answers

| Question | Answer |
|----------|--------|
| What HTTP protocol is used in example? | **HTTP/1.1** |
| What header tells browser how much data to expect? | **Content-Length** |

---

# 🔄 Task 3 — HTTP Methods

HTTP Methods define client intent.

| Method | Purpose |
|--------|----------|
| GET | Retrieve data |
| POST | Create data |
| PUT | Update data |
| DELETE | Remove data |

---

## ✅ Task 3 Answers

| Action | Method |
|--------|--------|
| Create user | **POST** |
| Update email | **PUT** |
| Delete picture | **DELETE** |
| View article | **GET** |

---

# 📊 Task 4 — HTTP Status Codes

Status codes indicate request outcome.

## 🔢 Status Code Categories

| Range | Meaning |
|-------|----------|
| 100–199 | Informational |
| 200–299 | Success |
| 300–399 | Redirection |
| 400–499 | Client Errors |
| 500–599 | Server Errors |

---

## 📌 Common Status Codes

| Code | Meaning |
|------|---------|
| 200 | OK |
| 201 | Created |
| 301 | Moved Permanently |
| 302 | Found |
| 400 | Bad Request |
| 401 | Not Authorised |
| 403 | Forbidden |
| 404 | Not Found |
| 500 | Internal Server Error |
| 503 | Service Unavailable |

---

## ✅ Task 4 Answers

| Scenario | Code |
|----------|------|
| Created new user | **201** |
| Page doesn't exist | **404** |
| Server database crash | **503** |
| Edit profile without login | **401** |

---

# 📦 Task 5 — Headers

Headers provide additional metadata in HTTP communication.

---

## 📤 Common Request Headers

| Header | Purpose |
|--------|---------|
| Host | Specifies requested domain |
| User-Agent | Browser information |
| Content-Length | Length of request body |
| Accept-Encoding | Supported compression |
| Cookie | Client-stored session data |

---

## 📥 Common Response Headers

| Header | Purpose |
|--------|---------|
| Set-Cookie | Stores cookie on client |
| Cache-Control | Caching rules |
| Content-Type | Type of returned data |
| Content-Encoding | Compression method |

---

## ✅ Task 5 Answers

| Question | Answer |
|----------|--------|
| Header that tells server what browser is used? | **User-Agent** |
| Header that tells browser data type? | **Content-Type** |
| Header that specifies website requested? | **Host** |

---

# 🍪 Task 6 — Cookies

Cookies are small pieces of data stored on the client.

They are set via:
Set-Cookie

Cookies allow:

- Session tracking  
- Authentication  
- Personalization  

HTTP is stateless, so cookies maintain state.

---

## ✅ Task 6 Answer

| Question | Answer |
|----------|--------|
| Header used to save cookies? | **Set-Cookie** |

---

# 🧪 Task 7 — Making Requests (Practical)

Using the HTTP emulator:

---

### 🏁 Flags Retrieved

| Request | Flag |
|----------|------|
| GET /room | **THM{YOU'RE_IN_THE_ROOM}** |
| GET /blog?id=1 | **THM{YOU_FOUND_THE_BLOG}** |
| DELETE /user/1 | **THM{USER_IS_DELETED}** |
| PUT /user/2 (username=admin) | **THM{USER_HAS_UPDATED}** |
| POST /login (thm:letmein) | **THM{HTTP_REQUEST_MASTER}** |

---

# 🛠️ Skills & Concepts Practiced

- Understanding HTTP vs HTTPS  
- Parsing URLs  
- Reading raw HTTP requests & responses  
- Using HTTP methods  
- Interpreting status codes  
- Analyzing headers  
- Working with cookies  
- Crafting custom HTTP requests  

---

# 📚 Key Takeaways

- HTTP powers web communication  
- HTTPS ensures encrypted communication  
- URLs structure resource access  
- Methods define intent  
- Status codes define response outcome  
- Headers control request/response behavior  
- Cookies enable authentication  
- Manual HTTP manipulation is key for web exploitation  

---

