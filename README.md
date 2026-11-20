# CityHealth — Hospital & Clinic Information Page

A responsive, static single-page website for **CityHealth**, a modern medical clinic, built with semantic HTML5 and CSS3. The page presents core medical services, specialist schedules, clinic hours, contact information, and a styled appointment request form without relying on JavaScript frameworks or build tooling.

**Repository:** [EklavyaTyagi6/hospital-clinic-information-page](https://github.com/EklavyaTyagi6/hospital-clinic-information-page)

## Features

- **Sticky Navigation Bar:** Fixed top navigation (`.navbar`) with smooth anchor scrolling (`scroll-behavior: smooth`) and responsive `scroll-padding-top` offsets (`120px` on desktop, `170px` on narrow mobile screens) linking to Home, Services, Our Specialists, and Book Now.
- **Hero Banner:** Full-width header section featuring a linear-gradient overlay over a background image and the headline *"Modern Medicine. Compassionate Care."*
- **Services Showcase:** Three overlapping floating cards highlighting core clinic offerings:
  - **24/7 Emergency Care** — Round-the-clock immediate medical attention for critical and urgent conditions.
  - **Advanced Labs** — Diagnostic imaging and laboratory services for accurate results.
  - **Primary Care** — Comprehensive health check-ups and preventative care for the whole family.
- **Medical Team Schedule:** Responsive table (`.doctor-table`) listing clinic specialists, departments, and visiting hours:
  - **Dr. Alice Smith** — Cardiology (`Mon - Wed 9:00 AM - 1:00 PM`)
  - **Dr. Robert Jones** — Pediatrics (`Tue - Thu 10:00 AM - 3:00 PM`)
  - **Dr. Emily Davis** — Dermatology (`Fri - Sat 11:00 AM - 4:00 PM`)
- **Appointment Request Form:** Glassmorphism-styled booking card (`.glass-card`) with client-side HTML5 validation:
  - Patient Name (required text field)
  - Contact Number (10-digit telephone input with `pattern="[0-9]{10}"`)
  - Department selector (Cardiology, Pediatrics, Dermatology)
  - *Confirm Booking* submit button
- **Informative Footer:** Displays clinic overview (*serving since 2010*), Quick Links, Clinic Hours (`Mon - Fri: 8:00 AM - 8:00 PM`, `Saturday: 9:00 AM - 5:00 PM`, `Sunday: Emergency Only`), and Contact details (`123 Wellness Way, Medical District`, `(555) 123-4567`, `care@cityhealth.com`).

## Tech Stack

| Technology | Share | Role |
| :--- | :--- | :--- |
| **CSS3** | 51.9% | Layout, typography, glassmorphism styling, smooth scrolling, and responsive media queries |
| **HTML5** | 48.1% | Semantic page structure, specialist schedule table, and HTML5 form validation |
| **Google Fonts** | External | `Outfit` typeface (weights 300–700) |

## Project Structure

| File | Description |
| :--- | :--- |
| [index.html](https://github.com/EklavyaTyagi6/hospital-clinic-information-page/blob/main/index.html) | Main HTML document containing the navigation bar, hero section, service cards, medical team table, appointment form, and footer (163 lines). |
| [style.css](https://github.com/EklavyaTyagi6/hospital-clinic-information-page/blob/main/style.css) | Complete stylesheet defining the `#f8fafc` / `#334155` / `#0ea5e9` palette, sticky navbar, hero overlay, glass card form, and responsive breakpoints (486 lines). |
| `README.md` | Project documentation. |

## Getting Started

Because this is a pure HTML/CSS static site, no package installation or build step is required.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/EklavyaTyagi6/hospital-clinic-information-page.git
   cd hospital-clinic-information-page
   ```

2. **Open the page:**
   - Open `index.html` directly in any modern web browser, **or**
   - Serve it locally (for example, with VS Code Live Server or Python's built-in HTTP server):
     ```bash
     python3 -m http.server 8000
     ```
     Then visit `http://localhost:8000` in your browser.

## Responsive Breakpoints

`style.css` adapts the layout across five screen-width breakpoints:

| Breakpoint | Layout Adjustments |
| :--- | :--- |
| `<= 1199px` | Scales main container spacing, padding, and typography for smaller desktop and laptop screens. |
| `<= 1100px` | Reflows the footer into a 2x2 grid while preserving the three-column service cards row. |
| `<= 900px` | Stacks the medical team schedule table and appointment form vertically (`flex-direction: column`). |
| `<= 768px` | Stacks service cards into a single column and adjusts navigation bar sizing. |
| `<= 600px` | Stacks the navbar vertically with an increased `170px` scroll offset, enables horizontal scrolling for `.doctor-table` (`min-width: 460px`), and collapses the footer into a single column. |

## Notes

- **Static Form Handling:** The appointment form (`action="#"`, `method="POST"`) is currently a frontend-only prototype with HTML5 input validation. Connecting it to a backend endpoint or form service is required to process live bookings.
- **External Assets:** An internet connection is needed to load the `Outfit` font from Google Fonts and the Unsplash hero background image.

## Contributors

- **Mahathi Gowri** (`mahathigowri-oss`)
- **EklavyaTyagi6**
- **surajshakya9569**
