## 📁 File Path System: How Websites Find Their Files

### 1️⃣ The First Principle

A website is **not** a single file—it's a collection of files (HTML, CSS, JavaScript, images, etc.) organized in folders, just like your computer.

### 2️⃣ The Core Problem

If your `index.html` needs to show an image called `logo.png`, how does it tell the browser **where to find it**?  
You need a **file path**—an exact address for the browser.

---

### 🔗 Relative File Paths (Most Important!)

A **relative path** gives directions to a file **starting from the location of your current file**.  
You’ll use these almost always for your own files.

#### Example Project Structure

```
my-website/
├── index.html
├── about.html
├── images/
│   ├── logo.png
│   └── hero.jpg
└── pages/
  ├── contact.html
  └── terms.html
```

#### Common Scenarios

**1. Same Folder**

```html
<!-- Inside index.html -->
<a href="about.html">About Us</a>
```

**2. Sub-Folder (Going Down)**

```html
<!-- Inside index.html -->
<img src="images/logo.png" alt="Logo" />
```

**3. Parent Folder (Going Up)**

```html
<!-- Inside pages/contact.html -->
<img src="../images/logo.png" alt="Logo" />
```
- `../` means "go up one folder"

---

### 🌐 Absolute File Paths

An **absolute path** is a full URL (starts with `http://` or `https://`).  
Use these **only** for resources **not on your own website**.

**Examples:**

```html
<a href="https://www.google.com">Google</a>
<img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/Html5_logo_and_wordmark.svg" alt="HTML5 Logo">
```

**Never use your computer’s file path (like `C:/Users/...`) for web images!**  
It only works on your computer, not on the web.

---

### 🖥️ Absolute Paths: Windows vs. macOS/Linux

| Feature                  | Windows Example                           | macOS/Linux Example                  |
|--------------------------|-------------------------------------------|--------------------------------------|
| **Root**                 | `C:\` (drive letter)                      | `/` (single slash)                   |
| **Separator**            | `\` (backslash)                           | `/` (forward slash)                  |
| **Example**              | `C:\Users\JohnDoe\Documents\report.docx`  | `/Users/johndoe/Documents/report.docx` |

---

## 🏗️ HTML Boilerplate: The Foundation of Every Page

### Why Do We Need It?

Browsers need **clear instructions**:  
- What version of HTML?
- What language?
- How to display on mobile?
- What’s the tab title?

### The Modern HTML5 Boilerplate

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>

</body>
</html>
```

#### What Each Line Means

- `<!DOCTYPE html>`: Tells browser to use modern HTML rules.
- `<html lang="en">`: Sets the language for accessibility and SEO.
- `<meta charset="UTF-8">`: Ensures all characters display correctly.
- `<meta name="viewport" ...>`: Makes your site look good on mobile.
- `<title>`: Sets the browser tab name.
- `<body>`: Where your visible content goes.

---

### ❓ Why Not Skip the Boilerplate?

Browsers are **forgiving**—they’ll try to guess missing info.  
But skipping boilerplate can cause:
- Unpredictable layouts (“quirks mode”)
- Broken characters
- Bad mobile experience
- Poor SEO and accessibility

**Always use the boilerplate for professional, reliable websites!**

---

## 🌍 Multipage Websites: Organizing Your Content

Big topics need separate pages (like chapters in a book).  
A multipage site connects these with a **navigation menu**.

### How?

1. **Consistent Structure:**  
   Every page shares the same header, footer, and style.

2. **Navigation System:**  
   Use `<a>` tags for links between pages.

---

## 📦 Grouping & Labeling Content: div, class, id, span

### 1. `<div>`: The Generic Container

Wrap related elements together:

```html
<div>
  <img src="avatar.png">
  <h2>Arjun Kumar</h2>
  <p>Loves to code and teach HTML.</p>
</div>
```

### 2. `class` & `id`: Targeting Elements

- **id**: Unique label for one element.
- **class**: Reusable label for many elements.

```html
<div id="main-header">...</div>
<div id="featured-profile" class="profile-card">...</div>
<div class="profile-card">...</div>
```

**CSS Example:**

```css
#main-header { ... }
.profile-card { ... }
#featured-profile { ... }
```

### 3. `<span>`: Inline Highlighter

Highlight part of a sentence:

```html
<p>This is very <span class="highlight">important</span> information.</p>
```

---

## 🏷️ Semantic Layout Tags

- `<header>`: Top section (logo, navigation)
- `<footer>`: Bottom section (copyright, contact)
- `<main>`: Unique content for each page (only one per page)

---

**Summary:**  
- Use **relative paths** for your own files, **absolute paths** for external resources.
- Always start with the **HTML boilerplate**.
- Organize content with `<div>`, label with `class` and `id`, highlight with `<span>`.
- Use semantic tags for clear structure.

---

*Build your websites on a solid foundation—your future self (and your users) will thank you!*
