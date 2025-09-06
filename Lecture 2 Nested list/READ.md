# Lecture 2: Nested Lists and Tables

This lecture covers two important Markdown features: **nested lists** and **tables**. Below is a detailed explanation with examples, including equivalent HTML snippets for better understanding.

---

## 1. Nested Lists

Nested lists allow you to organize information hierarchically. You can nest both ordered and unordered lists.

### Unordered Nested List

**Markdown Example:**
```markdown
- Item 1
    - Subitem 1.1
        - Subitem 1.1.1
    - Subitem 1.2
- Item 2
```

**Rendered Output:**
- Item 1
    - Subitem 1.1
        - Subitem 1.1.1
    - Subitem 1.2
- Item 2

**HTML Equivalent:**
```html
<ul>
  <li>Item 1
    <ul>
      <li>Subitem 1.1
        <ul>
          <li>Subitem 1.1.1</li>
        </ul>
      </li>
      <li>Subitem 1.2</li>
    </ul>
  </li>
  <li>Item 2</li>
</ul>
```

### Ordered Nested List

**Markdown Example:**
```markdown
1. First
     1. First - Subitem
            1. First - Subsubitem
     2. Second - Subitem
2. Second
```

**Rendered Output:**
1. First
     1. First - Subitem
            1. First - Subsubitem
     2. Second - Subitem
2. Second

**HTML Equivalent:**
```html
<ol>
  <li>First
    <ol>
      <li>First - Subitem
        <ol>
          <li>First - Subsubitem</li>
        </ol>
      </li>
      <li>Second - Subitem</li>
    </ol>
  </li>
  <li>Second</li>
</ol>
```

---

## 2. Tables

Tables are used to display data in rows and columns.

### Basic Table

**Markdown Example:**
```markdown
| Name   | Age | City      |
|--------|-----|-----------|
| Alice  | 24  | New York  |
| Bob    | 30  | London    |
| Carol  | 28  | Paris     |
```

**Rendered Output:**

| Name   | Age | City      |
|--------|-----|-----------|
| Alice  | 24  | New York  |
| Bob    | 30  | London    |
| Carol  | 28  | Paris     |

**HTML Equivalent:**
```html
<table>
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>24</td>
    <td>New York</td>
  </tr>
  <tr>
    <td>Bob</td>
    <td>30</td>
    <td>London</td>
  </tr>
  <tr>
    <td>Carol</td>
    <td>28</td>
    <td>Paris</td>
  </tr>
</table>
```

### Table with Alignment

**Markdown Example:**
```markdown
| Name   | Age | City      |
|:-------|:---:|----------:|
| Alice  |  24 | New York  |
| Bob    |  30 | London    |
| Carol  |  28 | Paris     |
```

- `:---` aligns left
- `:---:` centers
- `---:` aligns right

**HTML Equivalent:**
```html
<table>
  <tr>
    <th style="text-align:left;">Name</th>
    <th style="text-align:center;">Age</th>
    <th style="text-align:right;">City</th>
  </tr>
  <tr>
    <td style="text-align:left;">Alice</td>
    <td style="text-align:center;">24</td>
    <td style="text-align:right;">New York</td>
  </tr>
  <tr>
    <td style="text-align:left;">Bob</td>
    <td style="text-align:center;">30</td>
    <td style="text-align:right;">London</td>
  </tr>
  <tr>
    <td style="text-align:left;">Carol</td>
    <td style="text-align:center;">28</td>
    <td style="text-align:right;">Paris</td>
  </tr>
</table>
```

---

## Summary

- **Nested lists** help structure content hierarchically.
- **Tables** organize data for easy comparison.
- Both features improve readability and presentation in Markdown documents.
- HTML snippets show how Markdown translates to web content.

