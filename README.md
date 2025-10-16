# Markdown to HTML Converter

## 1. Summary/Overview

This single-page web application converts Markdown content to HTML using the Marked.js library and applies syntax highlighting to code blocks using Highlight.js. It processes embedded base64-encoded Markdown content and renders the resulting HTML in the browser.

Key features:
- Converts Markdown to semantic HTML
- Automatic syntax highlighting for code blocks
- Responsive design
- Client-side processing only

## 2. Setup Instructions

1. Save the provided HTML code as an `.html` file (e.g., `index.html`)
2. Open the file in any modern web browser
3. No server or additional dependencies required

## 3. Usage Guide

The application will automatically:
1. Decode the embedded base64-encoded Markdown content
2. Convert the Markdown to HTML using Marked.js
3. Apply syntax highlighting to code blocks using Highlight.js
4. Display the rendered content in the `#markdown-output` element

Example Markdown features included:
- Headers (#, ##, ###)
- Lists (ordered and unordered)
- Links and images
- Code blocks with language specification
- Horizontal rules

## 4. Code Explanation and Architecture

### Architecture
The application is a single HTML file containing:
- HTML structure with output container
- CSS for basic styling
- JavaScript for processing and rendering

### Key Components

1. **CDN Libraries**:
   - Marked.js (v4.0.2) for Markdown parsing
   - Highlight.js (v11.5.1) for code syntax highlighting

2. **Processing Flow**:
   - Base64 content decoded at runtime
   - Marked.js converts Markdown to HTML
   - Highlight.js applies syntax highlighting
   - Rendered output displayed in DOM element with ID `markdown-output`

3. **Security Features**:
   - Client-side processing eliminates server dependencies
   - No external requests after initial library loading

## 5. License Information

MIT License

Copyright (c) 2023

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.