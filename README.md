# Movenpick

The official front-end website for Mövenpick Café, independently designed and developed by myself. This project is a multi-page static website that simulates the full information architecture of a real restaurant, covering menu categories, set meals, business lunches, a reservation entry point, and brand introduction pages.

---

## Overview

The website is built around the Mövenpick Café brand using only the three core front-end technologies (HTML / CSS / JavaScript), with no front-end framework dependencies. The design goal is to present the full information structure that a real restaurant needs for external operations, while maintaining a consistent visual style and user flow.

- A pure static website that can be opened directly in any browser via `index.html`.
- Built with semantic HTML and standalone CSS files for easy long-term maintenance and extension.
- All image assets are organized under the `images/` directory.

---

## Tech Stack

- HTML5
- CSS3
- JavaScript (Vanilla)

---

## Project Structure

| File / Folder | Description |
| --- | --- |
| `index.html` | Home page and main entry point, aggregating business lunches, set meals, and ice cream flavor sections. |
| `15.reservation.html` | Reservation form page where users can enter name, phone, email, reservation date, party size, and special requests. |
| `2.two person set` / `3.two person set(1)` | Two-person set meals (five-course and six-course deluxe). |
| `4.three person set` / `5.three person set(1)` | Three-person set meals (seven-course and nine-course deluxe). |
| `6.appetizer` ~ `9.steak` | Category pages for appetizers, main courses, deluxe main courses, and steaks. |
| `10.dessert side` ~ `12.ice cream` | Pages for baked desserts, ice cream plates, and ice cream flavors. |
| `13.business` / `14.business(1)` | Business lunch menus (Mon / Tue / Wed and Thu / Fri groupings). |
| `16.about.html` | Brand introduction and "About Us" page. |
| `basic1.html` ~ `basic10.html` | Early layout drafts and structural prototypes that document the design iteration process. |
| `images/` | Image assets for menus, set meals, and other visual elements. |

---

## How to Run

Since this project is a pure static website, it can be opened in any browser:

1. Download the entire project folder to your local machine.
2. Open `index.html` directly in a browser.
3. Use the navigation bar to access menu categories, set meal pages, and the reservation form.

To run with a local server (recommended for the full experience):

```bash
# Pick either command
python3 -m http.server 8000
# or
npx serve .
```

Then open `http://localhost:8000` in your browser.

---

## Companion Project — Full-Stack Backend Integration

This front-end is also used as the source for an independent full-stack project, paired with Node.js and SQLite to deliver a complete end-to-end reservation system:

- Backend repository: [brianlab999/Web-Application-with-SQLite-Back-End](https://github.com/brianlab999/Web-Application-with-SQLite-Back-End)
- The backend uses Express to receive reservation form submissions and persist them to a SQLite database, and exposes an `/api/bookings` endpoint so the front-end can fetch the reservation list.
- The `views/` directory of that project directly reuses all pages and styles from this Movenpick front-end.
