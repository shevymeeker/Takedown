# Takedown

Questions for Daviess County candidates 2026

## Overview

This is a single-page web application designed to help voters hold candidates accountable during the 2026 Daviess County elections. The app presents important questions for both Commissioner and Judge-Executive candidates in an interactive, easy-to-use format.

## Features

- **Interactive flip cards** - Click or tap cards to reveal analysis of potential answers
- **Candidate filtering** - Switch between Commissioner and Judge-Executive questions
- **Fully accessible** - Keyboard navigation, ARIA labels, and screen reader support
- **Responsive design** - Works on desktop, tablet, and mobile devices
- **Dark mode support** - Automatically adapts to user's system preferences
- **Modern codebase** - Clean, well-documented JavaScript with security best practices

## How to Use

1. Open `Index.html` in any modern web browser
2. Click the tabs to filter between Commissioner and Judge-Executive questions
3. Click any card to flip it and see what to watch for in candidate responses
4. Navigate with keyboard using Tab and Enter/Space keys

## For Developers

### Adding New Questions

To add a new question card:

1. Open `Index.html` in a text editor
2. Find the `data` array in the `<script>` section
3. Copy the template at the bottom of the data array
4. Fill in the required fields:
   - `role`: Either 'commissioner' or 'judge'
   - `topic`: Category name (e.g., 'Budget & Funding')
   - `question`: The question to ask candidates
   - `redFlag`: What would be a concerning answer
   - `goodSign`: What would be a positive answer
5. Save the file and refresh your browser

### Code Structure

- **CSS Variables**: Theme colors and styling defined in `:root`
- **Responsive Grid**: Auto-adjusting card layout
- **Data-Driven**: All questions stored in a single data array
- **XSS Protection**: HTML sanitization on all user-facing content
- **Validation**: Built-in data validation on page load

### Testing

Run the test suite by opening `test.html` in your browser. This validates:
- HTML structure and syntax
- JavaScript modernization (no `var`, uses `const`/`let`)
- Accessibility attributes (ARIA labels, semantic HTML)
- Security features (XSS protection)
- Responsive design implementation
- Dark mode support

### Tech Stack

- Pure HTML5 (no frameworks required)
- Modern CSS3 with custom properties
- Vanilla JavaScript (ES6+)
- Semantic HTML for accessibility
- Progressive enhancement

## Browser Support

Works in all modern browsers:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Security

- Input sanitization to prevent XSS attacks
- No external dependencies or CDN requirements
- Can be run entirely offline

## License

Public domain - use freely for civic engagement

## Contributing

To contribute:
1. Fork the repository
2. Make your changes
3. Test thoroughly (run test.html)
4. Submit a pull request

---

Made for the citizens of Daviess County
