# HTML - HyperText Markup Language

**HTML** stands for **HyperText Markup Language**.

- **HyperText**: Refers to text that is linked to other documents or web pages.
- **Markup**: Means structuring content using tags.

---

## Headings

HTML provides six heading tags: `h1` to `h6`.

- `h1` is the most important for SEO and is the largest in size.
- `h6` is the least important and the smallest.

Example:

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
...
<h6>Smallest Heading</h6>
```

---

## Paragraphs

Use the `<p>` tag to add paragraphs.  
Always close tags properly:

```html
<p>This is a paragraph.</p>
```

---

## Line Breaks

The `<br>` tag creates a line break.  
It is a self-closing tag:

```html
Line one.<br>
Line two.
```

---

## Lists

- **Ordered List**: Use `<ol>` for numbered lists.
- **Unordered List**: Use `<ul>` for bulleted lists.
- **List Items**: Use `<li>` for each item.

Example:

```html
<ol>
    <li>First item</li>
    <li>Second item</li>
</ol>

<ul>
    <li>Bullet one</li>
    <li>Bullet two</li>
</ul>
```

---

## Links

Use the `<a>` tag to create hyperlinks:

```html
<a href="https://www.google.com/maps/?entry=wc">Google Maps</a>
```

By default, links open in the same tab.  
To open in a new tab, add the `target="_blank"` attribute:

```html
<a href="https://www.google.com/maps/?entry=wc" target="_blank">Google Maps</a>
```

---

**Tip:** Always close your HTML tags properly for well-structured pages!