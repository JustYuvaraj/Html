
# Markup Language 
A **markup language** is like a set of instructions that tells a computer how to display text or content.   
For example, it can say things like:  
- "make this text bold"  
- "create a list"   
This is done by using special codes (like `<strong>` or `<ul>` in HTML).   
It’s like adding invisible instructions to plain text to make it look nicer or more organized!

## What is HTML?
- **HTML** stands for **HyperText Markup Language**.
- It is the language used to create web pages.
- Originally designed for sharing scientific documents.
- Now used to describe various types of documents displayed as web pages.

## HTML Elements
- **Elements** are the building blocks of an HTML page.
- Content is labeled with tags like:
  - Paragraph (`<p>`)
  - List (`<ul>`, `<ol>`)
  - Table (`<table>`)
- Browsers use tags to render(process and generate visual representation) content but do not display the tags themselves.

## Evolution of HTML  
- HTML started in the early 1990s by **CERN** and **IETF**.  
- The **W3C** (World Wide Web Consortium) created rules for HTML.  
- The **WHATWG** (Web Hypertext Application Technology Working Group) also helped with HTML.  
- In 2007, W3C and WHATWG worked together to create **HTML5**.

## HTML5 Objectives
- Can be written in **HTML** or **XML** syntax.
- Works with earlier HTML versions.
- Improves document markup.
- Includes markup for:
  - Web storage
  - Video
  - Audio content
## HTML5 Features
- **Categorizes web pages** into different sections.
- Includes tools for:
  - **Data management**
  - **Drawing**
  - **Video and audio** 
- **Works smoothly on all browsers and devices**:  
  Whether you use Chrome, Safari, or your phone, HTML5 helps your app work great everywhere.  
- **Makes websites more interactive**:  
  Add cool features like games, animations, and forms without needing extra plugins.  
- **Feels like a desktop app**:  
  Websites can act more like apps you’d use on your computer, right in your browser.  
- **Build once, use everywhere**:  
  Create apps and websites that work on phones, tablets, and computers—all from one codebase.  
- **Looks the same on all devices**:  
  Whether you’re on a phone, tablet, or desktop, your website looks consistent.

## HTML5 Document Example
- **`<!DOCTYPE>`**: Declares the HTML version (not an HTML tag).
- **`<html>`**: Root element containing all other elements.
- **`<head>`**: Contains metadata like:
  - **`<title>`**: Page title.
  - Scripts, styles, and links.
- **`<body>`**: Contains content displayed on the webpage.

## Document Object Model (DOM)
-represents the structure of a web document, such as an HTML page, in a tree-like data structure(tree of objects).
-**DOM Tree**: A hierarchical representation of an HTML document, structured as a tree of nodes. The tree is stored in the computer's RAM and constructed by the browser when the HTML document is loaded.
- **nodes** : represents a part of the document, such as elements, text, or comments.)
- **Types of Nodes** in the DOM tree :
  - **DOCTYPE node** 
  - **Element nodes** (e.g., headers, paragraphs) - 
  - **Text nodes** 
  - **Comment nodes** 

## XML Syntax in HTML5
- **XML Declaration and MIME Type:** HTML5 documents using XML syntax start with `<?xml version="1.0" encoding="UTF-8"?>` and use MIME type `application/xml`. **XML parsers** enforce strict syntax rules, causing errors if not followed.

## HTML vs. XHTML
- **HTML:** Tags are case-insensitive, and syntax is flexible, allowing unclosed tags.
- **XHTML:** Tags must be lowercase, elements must be well-formed, and parsing stops on errors.
  # HTML Scripting

## What is Scripting?
- **Scripting** writing small programs or scripts that add interactivity and dynamic behavior to a website.
- Often done using **JavaScript**.
- Can be added:
  - Directly in HTML using `<script>` tags.
  - Or in a separate file linked to the HTML.

## Uses of Scripting
- **Form validation**
- **Dynamic content changes**
- **Image manipulation**
- **Interactive user experiences**

## HTML5 Sandbox
- **Sandboxed browsing context**:  A Secure Environment for Untrusted Content
  - Adds extra content restrictions.
  - Can be applied to the entire page or specific elements like iframes, offering flexibility in security management.(e.g., `<iframe>`).
- **Sandbox attribute**:
  - Prevents embedded objects from gaining implicit permissions.
  - Avoids granting third-party scripts the same permissions as your page.

## Document Object Model (DOM)
- Each HTML document loaded in a browser becomes a **Document object**.
- Provides access to all HTML elements on the page.
- Accessed via **DOM tree accessors** (prefixed with `document`).

## Common DOM Accessors
- **`document.head`**: Returns the `<head>` element (or `null` if none).
- **`document.images`**: Returns an `HTMLCollection` of all `<img>` elements.
- **`document.scripts`**: Returns an `HTMLCollection` of all `<script>` elements.

## DOM Methods
- **`document.getElementById('id')`**:
  - Accesses an element by its `id` attribute.
- **`document.getElementsByTagName('tag')`**:
  - Returns a `NodeList` of all elements with the specified tag.
## Checking Browser Support with JavaScript
- **Steps**:
  1. Create a DOM element using `document.createElement()`.
  2. Set the element type (e.g., `input type="date"`).
  3. Test for a known property or method of the element.
- **Result**:
  - If the property/method exists, the browser supports the element.
  - If not, the browser does not support the element.
- **Fallback Behavior**:
  - Unsupported elements revert to default behavior (e.g., displaying as a text field).
    ```markdown
# HTML Elements and Examples

| **Element**          | **Description**                                                                 | **Example**                                                                 |
|----------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| `<!--  -->`          | Denotes a comment in HTML, not displayed by the browser.                        | `<!-- This is a comment -->`                                                |
| `<!DOCTYPE html>`    | Declares the document type. Must be the first line in an HTML document.         | ```html <!DOCTYPE html> <html> <head>...</head> <body>...</body> </html> ```|
| `<a href="path">`    | Creates a hyperlink using the `href` attribute.                                 | `<a href="https://www.ibm.com">IBM</a>`                                     |
| `<body>`             | Contains the content of the HTML document.                                      | ```html <body> <!-- Document Body Here --> </body> ```                      |
| `<div>`              | Used to separate sections for styling with CSS.                                 | ```html <div> This element is used for styling purposes. </div> ```         |
| `<h1>`               | Adds a level 1 heading.                                                         | `<h1>Thomas J. Watson</h1>`                                                 |
| `<head>`             | Contains metadata and is placed after `<html>` and before `<body>`.             | ```html <head> <!-- Metadata Here --> </head> ```                           |
| `<html>`             | The root element of an HTML document.                                           | ```html <html> <head>...</head> <body>...</body> </html> ```                |
| `<img src="path">`   | Inserts an image. `src` specifies the image path. Optional: `width`, `height`.  | `<img src="image.jpg" width="300" height="300"/>`                           |
| `<li>`               | Creates bulleted or numbered list items. Used with `<ul>` or `<ol>`.            | ```html <ul> <li>Bullet point 1</li> <li>Bullet point 2</li> </ul> ```      |
| `<link>`             | Links external documents like CSS files.                                        | ```html <head> <link rel="stylesheet" href="styles.css"> </head> ```        |
| `<meta>`             | Provides metadata about the HTML document.                                      | ```html <head> <meta name="author" content="Christopher Moore"> </head> ``` |
| `<ol>`               | Creates an ordered (numbered) list. Used with `<li>`.                           | ```html <ol> <li>Numbered bullet point 1</li> <li>Numbered bullet point 2</li> </ol> ``` 
| `<p>`                | Defines a paragraph. Adds a line break after the text.                          | `<p>This is a paragraph of text.</p>`                                       |
| `<script>`           | Embeds JavaScript in an HTML document.                                          | ```html <script> alert("Hello World"); </script> ```                        |
| `<table>`            | Defines a table. Used with `<tr>`, `<td>`, and `<th>`.                          | ```html <table> <tr> <th>Header cell 1</th> <th>Header cell 2</th> </tr> <tr> <td>First row first cell</td> <td>First row second cell</td> </tr> </table> ``` |
| `<td>`               | Defines a cell within a table row.                                              | `<td>Cell Content</td>`                                                     |
| `<th>`               | Defines a header cell within a table row.                                       | `<th>Header cell 1</th>`                                                    |
| `<title>`            | Defines the title of the HTML document (displayed in the browser tab).          | ```html <head> <title>Document Title</title> </head> ```                    |
| `<tr>`               | Defines a row within a table.                                                   | ```html <tr> <td>First row first cell</td> <td>First row second cell</td> </tr> ``` 
| `<ul>`               | Creates an unordered (bulleted) list. Used with `<li>`.                         | ```html <ul> <li>Bullet point 1</li> <li>Bullet point 2</li> </ul> ```      |
```
