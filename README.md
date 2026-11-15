# HTML Notes

> Transcription of the screenshots available from the referenced conversation. The attachment data provided pages 7–16 only; pages 1–6 were not available to transcribe.

## Pages 1–6

**Not available in the referenced conversation's attachment data.** These pages are omitted rather than reconstructed.

## Page 7

### Table caption

```html
<!-- Table caption →
<table>
  <caption>Table Title</caption>
  <!-- table content →
</table>
```

### Forms

#### Form Structure

```html
<form action="/submit" method="POST">
  <fieldset>
    <legend>Personal Information</legend>

    <!-- Text input →
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <!-- Email input →
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>

    <!-- Password input →
    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required>

    <!-- Number input →
    <label for="age">Age:</label>
    <input type="number" id="age" name="age" min="1" max="120">

    <!-- Date input →
    <label for="birthdate">Birthdate:</label>
    <input type="date" id="birthdate" name="birthdate">

    <!-- Radio buttons →
    <fieldset>
      <legend>Gender:</legend>
```

**Screenshot cutoff:** the page ends mid-example; the opening `<fieldset>` and the rest of the form continue on page 8.

## Page 8

Continuation of the form example from page 7:

```html
      <input type="radio" id="male" name="gender" value="male">
      <label for="male">Male</label>

      <input type="radio" id="female" name="gender" value="female">
      <label for="female">Female</label>
    </fieldset>

    <!-- Checkboxes →
    <input type="checkbox" id="newsletter" name="newsletter" value="yes">
    <label for="newsletter">Subscribe to newsletter</label>

    <!-- Dropdown select →
    <label for="country">Country:</label>
    <select id="country" name="country">
      <option value="">Select a country</option>
      <option value="us">United States</option>
      <option value="uk">United Kingdom</option>
      <option value="ca">Canada</option>
    </select>

    <!-- Textarea →
    <label for="comments">Comments:</label>
    <textarea id="comments" name="comments" rows="4" cols="50"></textarea>

    <!-- File upload →
    <label for="file">Upload file:</label>
    <input type="file" id="file" name="file" accept=".pdf,.doc,.docx">

    <!-- Submit button →
    <input type="submit" value="Submit">
    <button type="submit">Submit Form</button>
    <button type="reset">Reset Form</button>
  </fieldset>
</form>
```

### Input Types

## Page 9

### Input Types

```html
<input type="text">          <!-- Text input →
<input type="email">         <!-- Email validation →
<input type="password">      <!-- Hidden text →
<input type="number">        <!-- Numeric input →
<input type="tel">           <!-- Telephone →
<input type="url">           <!-- URL validation →
<input type="search">        <!-- Search box →
<input type="date">          <!-- Date picker →
<input type="time">          <!-- Time picker →
<input type="datetime-local"> <!-- Date and time →
<input type="month">         <!-- Month picker →
<input type="week">          <!-- Week picker →
<input type="color">         <!-- Color picker →
<input type="range">         <!-- Slider →
<input type="file">          <!-- File upload →
<input type="hidden">        <!-- Hidden field →
<input type="checkbox">      <!-- Checkbox →
<input type="radio">         <!-- Radio button →
<input type="submit">        <!-- Submit button →
<input type="reset">         <!-- Reset button →
<input type="button">        <!-- Generic button →
```

### Semantic HTML5 Elements

#### Layout Elements

```html
<header>
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<main>
```

**Screenshot cutoff:** the visible example ends after `<main>` and continues on page 10.

## Page 10

Continuation of the semantic layout example:

```html
  <article>
    <header>
      <h1>Article Title</h1>
      <time datetime="2024-01-01">January 1, 2024</time>
    </header>

    <section>
      <h2>Section Heading</h2>
      <p>Section content...</p>
    </section>

    <aside>
      <h3>Related Links</h3>
      <ul>
        <li><a href="#">Link 1</a></li>
        <li><a href="#">Link 2</a></li>
      </ul>
    </aside>
  </article>
</main>

<footer>
  <p>&copy; 2024 Your Website. All rights reserved.</p>
</footer>
```

### Content Elements

```html
<figure>
  <img src="image.jpg" alt="Description">
  <figcaption>Image caption</figcaption>
</figure>

<details>
  <summary>Click to expand</summary>
  <p>Hidden content that can be toggled</p>
</details>

<progress value="70" max="100">70%</progress>
```

## Page 11

Continuation of the content elements example:

```html
<meter value="6" min="0" max="10">6 out of 10</meter>

<address>
  Contact: <a href="mailto:email@example.com">email@example.com</a>
</address>
```

### Meta Tags and Head Elements

#### Essential Meta Tags

```html
<head>
  <!-- Character encoding →
  <meta charset="UTF-8">

  <!-- Viewport for responsive design →
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Page description →
  <meta name="description" content="Page description for search engines">

  <!-- Keywords →
  <meta name="keywords" content="html, web development, tutorial">

  <!-- Author →
  <meta name="author" content="Your Name">

  <!-- Refresh page →
  <meta http-equiv="refresh" content="30">

  <!-- CSS link →
  <link rel="stylesheet" href="styles.css">

  <!-- Favicon →
  <link rel="icon" type="image/x-icon" href="favicon.ico">
```

**Screenshot cutoff:** the head example continues at the top of page 12.

## Page 12

Continuation of Essential Meta Tags:

```html
  <!-- External fonts →
  <link rel="preconnect" href="https://fonts.googleapis.com">

  <!-- JavaScript →
  <script src="script.js"></script>
</head>
```

### HTML Entities

#### Common Entities

```html
&lt;     <!-- < (less than) →
&gt;     <!-- > (greater than) →
&amp;    <!-- & (ampersand) →
&quot;   <!-- " (quotation mark) →
&apos;   <!-- ' (apostrophe) →
&nbsp;   <!-- Non-breaking space →
&copy;   <!-- © (copyright) →
&reg;    <!-- ® (registered) →
&trade;  <!-- ™ (trademark) →
&euro;   <!-- € (euro) →
&pound;  <!-- £ (pound) →
&yen;    <!-- ¥ (yen) →
&sect;   <!-- § (section) →
&para;   <!-- ¶ (paragraph) →
```

### Best Practices

#### Do's

- Always use proper DOCTYPE declaration
- Use semantic HTML5 elements
- Include alt attributes for images
- Use proper heading hierarchy (h1 → h2 → h3)
- Validate your HTML code

## Page 13

Continuation of Best Practices — Do's:

- Use lowercase for element names and attributes
- Quote attribute values
- Close all tags properly
- Use meaningful class and ID names
- Optimize for accessibility

#### Don'ts

- Don't use deprecated elements (`<font>`, `<center>`, etc.)
- Don't skip heading levels
- Don't use tables for layout
- Don't use inline styles (use CSS instead)
- Don't forget to escape special characters
- Don't use non-semantic elements when semantic ones exist
- Don't ignore validation errors

### HTML5 APIs and Features

#### New Input Attributes

```html
<input type="text" placeholder="Enter your name" required>
<input type="email" pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$">
<input type="number" min="1" max="100" step="5">
<input type="text" autocomplete="name">
<input type="text" autofocus>
<input type="text" readonly>
<input type="text" disabled>
```

#### Data Attributes

```html
<div data-user-id="123" data-role="admin">User Info</div>
<button data-action="delete" data-confirm="Are you sure?">Delete</button>
```

## Page 14

### Accessibility Features

#### ARIA Attributes

```html
<button aria-label="Close dialog">×</button>
<div role="button" tabindex="0">Custom button</div>
<img src="chart.png" alt="Sales increased 25% this quarter" aria-describedby="chart-desc">
<p id="chart-desc">Detailed description of the chart...</p>

<!-- Skip link for screen readers →
<a href="#main-content" class="skip-link">Skip to main content</a>
```

#### Form Accessibility

```html
<label for="username">Username:</label>
<input type="text" id="username" name="username" aria-required="true" aria-describedby="username-help">
<div id="username-help">Must be 3-20 characters long</div>

<fieldset>
  <legend>Preferred contact method</legend>
  <input type="radio" id="email-contact" name="contact" value="email">
  <label for="email-contact">Email</label>
  <input type="radio" id="phone-contact" name="contact" value="phone">
  <label for="phone-contact">Phone</label>
</fieldset>
```

### Advanced HTML Concepts

#### Custom Elements

```html
<!-- Custom elements (requires JavaScript) →
<my-custom-element attribute="value">Content</my-custom-element>
```

#### Web Components

## Page 15

Continuation of Web Components:

```html
<template id="my-template">
  <style>
    /* Scoped styles */
  </style>
  <div>Template content</div>
</template>
```

### Microdata

```html
<div itemscope itemtype="http://schema.org/Person">
  <h1 itemprop="name">John Doe</h1>
  <p itemprop="jobTitle">Software Developer</p>
  <a itemprop="url" href="https://johndoe.com">Website</a>
</div>
```

### Quick Reference

#### Essential Tags Checklist

- [ ] `< !DOCTYPE html>`
- [ ] `<html lang="en">`
- [ ] `<head>` with meta tags
- [ ] `<title>`
- [ ] `<body>`
- [ ] Semantic elements (`<header>`, `<main>`, `<footer>`)
- [ ] Proper heading structure
- [ ] Alt text for images
- [ ] Form labels and validation
- [ ] Valid and accessible markup

#### Useful Resources

- **W3C HTML Validator:** https://validator.w3.org/

## Page 16

Continuation of Useful Resources:

- **MDN HTML Reference:** https://developer.mozilla.org/en-US/docs/Web/HTML
- **HTML5 Specification:** https://html.spec.whatwg.org/
- **Accessibility Guidelines:** https://www.w3.org/WAI/WCAG21/quickref/

---

*Happy coding! 🎉 Remember to always write semantic, accessible, and valid HTML!*

---

## Transcription notes

- The available screenshots are numbered 7–16; pages 1–6 were not included in the referenced thread's accessible attachments.
- Several HTML comments visibly use an arrow glyph (`→`) where a closing comment delimiter would normally appear. They are transcribed as shown.
- On page 15, the checklist's first tag is rendered as `< !DOCTYPE html>` in the screenshot and is transcribed as displayed.
