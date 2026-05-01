# 🌐 Server-Side Development & Web Server Basics

This guide explains server-side languages, web servers, and how a browser request travels through a web application.

---

# a. Introduction to Server-Side Languages

## What is a Server-Side Language?

A **server-side language** is used to build logic that runs on the server instead of the user’s browser.

It is responsible for:

- Processing requests
- Handling business logic
- Connecting to databases
- Authentication & authorization
- Generating dynamic pages
- Returning API responses (JSON/XML/HTML)

When a user clicks a button or submits a form, the request goes to the server where server-side code processes it.

---

# Why Use Server-Side Development?

Frontend technologies like HTML/CSS/JavaScript handle UI, but they cannot securely manage:

- Databases
- Password validation
- Payment processing
- Protected resources
- User sessions
- Backend APIs

That is where server-side languages are used.

---

# 1. Node.js (Primary)

## What is Node.js?

**Node.js** is a JavaScript runtime that allows JavaScript to run outside the browser on the server.

It uses the **V8 Engine** (same engine used by Chrome).

## Why Popular?

- Same language for frontend and backend (JavaScript)
- Fast and scalable
- Non-blocking asynchronous architecture
- Large ecosystem using **npm**
- Excellent for APIs and real-time apps

## Common Use Cases

- REST APIs
- Chat applications
- Streaming apps
- Real-time dashboards
- Full-stack JavaScript apps

## Example (Node.js + Express)

```javascript
const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.send("Hello World");
});

app.listen(3000);
