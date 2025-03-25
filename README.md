# IT2234P Web Services and Server Technologies

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)](https://expressjs.com/)
[![HTTP](https://img.shields.io/badge/HTTP-black?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Web/HTTP)
[![Code Quality](https://img.shields.io/badge/Code%20Quality-A-brightgreen?style=for-the-badge)]()

> 📚 A comprehensive collection of daily practical lessons for Web Services and Server Technologies course.

## 📋 Course Overview

This repository serves as a practical guide through various web services and server technologies. Each lesson is organized in dedicated folders containing both source code and visual outputs.

## 🗓️ Latest Session: Server Technologies (March 20, 2025)

### 🎯 Learning Objectives

#### Server Technologies
- Create basic HTTP server using Node.js
- Implement Express.js server setup
- Handle HTTP requests and responses
- Configure server ports and routing

### 💻 Code Examples & Implementations

#### 1. Server Technologies

##### Basic HTTP Server (`server.js`)
```javascript
const { createServer } = require('node:http');
const localhost = '127.0.0.1';
const port = 4444;
const server = createServer((req, res) => {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end('Hello Node JS!');
});

server.listen(port, localhost, () => {
    console.log(`Running on : ${localhost}:${port}`);
});
```
[View Output](outputs/server.png)

##### Express Server (`app.js`)
```javascript
const express = require('express');
const app = express();
const port = 3000;
app.get('/', (req, res) => {
  res.send('Hello Express JS!');
});
app.listen(port, () => {
  console.log(`Example app listening on port ${port}`); 
});
```
[View Output](outputs/server.png)

### 📊 Implementation Summary

| Category | File | Description | Output |
|----------|------|-------------|--------|
| Server Technologies | `server.js` | Basic HTTP server implementation | [View](output/server.png) |
| Server Technologies | `app.js` | Express.js server implementation | [View](output/server.png) |

### 🔍 Technical Notes

- All implementations are in pure JavaScript
- Each example includes comprehensive console output
- Visual outputs are captured for reference
- Consistent code formatting and naming conventions

---

<div align="center">

📖 **Learning Path** | 🛠️ **Practical Examples** | 📊 **Visual Outputs**

</div>
