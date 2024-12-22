# 🛠️ Developer Cheat Sheet 📋
> A quick reference guide to save time and boost productivity during development. Star ⭐ it if you find it useful!

---

## Table of Contents
- [Git Commands](#%EF%B8%8F-git-commands)
- [HTML Structure](#html-structure)
- [CSS Utilities](#css-utilities)
- [JavaScript Snippets](#javascript-snippets)
- [React Essentials](#react-essentials)
- [Command Line Shortcuts](#command-line-shortcuts)
- [VS Code Shortcuts](#vs-code-shortcuts)
- [Docker Basics](#docker-basics)
- [SQL Queries](#sql-queries)
- [Markdown Syntax](#markdown-syntax)
- [Bonus: API Status Codes](#bonus-api-status-codes)

---

## ⚙️ Git Commands
```bash
# Basic Workflow
git init                      # Initialize a repository
git add .                     # Stage all changes
git commit -m "Message"       # Commit changes
git push origin branch-name   # Push to remote

# Branching
git branch                    # List branches
git checkout -b new-branch    # Create and switch to a branch

# Undo Changes
git reset HEAD file.txt       # Unstage a file
git checkout -- file.txt      # Discard changes in a file

# Logs
git log --oneline             # Compact commit history
```

---

## 🌐 HTML Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <header></header>
  <main></main>
  <footer></footer>
</body>
</html>
```

---

## 🎨 CSS Utilities
### Flexbox
```css
.container {
  display: flex;
  flex-direction: row | column;  /* Row is default */
  justify-content: center | space-between | space-around;
  align-items: center | flex-start | flex-end;
}
```

### Grid
```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}
```

---

## 🧠 JavaScript Snippets
### Fetch API
```javascript
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error:', error));
```

### Array Methods
```javascript
const arr = [1, 2, 3, 4, 5];
const doubled = arr.map(x => x * 2);     // [2, 4, 6, 8, 10]
const filtered = arr.filter(x => x > 3); // [4, 5]
const sum = arr.reduce((a, b) => a + b); // 15
```

---

## ⚛️ React Essentials
### Functional Component
```javascript
import React from 'react';

const MyComponent = () => {
  return <h1>Hello, React!</h1>;
};

export default MyComponent;
```

### Hooks
```javascript
import React, { useState, useEffect } from 'react';

const App = () => {
  const [count, setCount] = useState(0);

  useEffect(() => {
    console.log('Component mounted');
  }, []);

  return <button onClick={() => setCount(count + 1)}>Count: {count}</button>;
};
```

---

## 💻 Command Line Shortcuts
```bash
# Navigate Directories
cd folder_name        # Enter a folder
cd ..                 # Go up one level

# File Management
touch file.txt        # Create a file
mkdir folder_name     # Create a folder
rm -r folder_name     # Delete a folder

# System Info
top                   # View running processes
df -h                 # Disk usage
```

---

## 🖥️ VS Code Shortcuts
```plaintext
Ctrl + P             # Quick file open
Ctrl + Shift + F     # Global search
Ctrl + `             # Open terminal
Alt + Click          # Multi-cursor editing
Ctrl + /             # Toggle comment
```

---

## 🐳 Docker Basics
```bash
# Common Commands
docker build -t my-app .       # Build an image
docker run -p 8080:80 my-app   # Run a container
docker ps                      # List running containers
docker stop container_id       # Stop a container
docker rm container_id         # Remove a container
docker rmi image_id            # Remove an image
```

---

## 🗄️ SQL Queries
```sql
-- Select
SELECT * FROM users WHERE age > 25;

-- Insert
INSERT INTO users (name, age) VALUES ('John', 30);

-- Update
UPDATE users SET age = 31 WHERE name = 'John';

-- Delete
DELETE FROM users WHERE name = 'John';
```

---

## 📝 Markdown Syntax
```markdown
# Header 1
## Header 2
### Header 3

**Bold** and _Italic_

[Link](https://example.com)

- List item
1. Ordered item
```

---

## 🚀 Bonus: API Status Codes
| Status Code | Meaning                  |
|-------------|--------------------------|
| 200         | OK                      |
| 201         | Created                 |
| 400         | Bad Request             |
| 401         | Unauthorized            |
| 404         | Not Found               |
| 500         | Internal Server Error   |

---

### 🙌 Contribute
Found something missing? Feel free to [open an issue](https://github.com/PHCoder05/DevCheats-Ultimate-Developer-Toolkit/issues) or submit a pull request.

---

### 🌟 Star this Repo
If you found this cheat sheet helpful, give it a star ⭐ and share it with others!
