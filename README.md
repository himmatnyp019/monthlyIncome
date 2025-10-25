# Project: Fair Pay — Work Hours & Income Calculator

This project is created to calculate the work hours & income for weeks and months
by taking daily attendance and evaluating expenses.

A simple and basic site. Straightforward and focused on the main task — let you
track daily start/end times, mark holidays, calculate weekly totals, and get a
monthly income summary after expenses and taxes.

Because this is open source, anyone can use and contribute to it. Please read
the sections below before using, modifying, or redistributing this code.

## Quick summary

* Purpose: Calculate daily, weekly, and monthly worked hours and estimate income.
* Main features: time entry (12/24h), holiday marking, weekly totals, expenses,
  tax calculation, print and screenshot export.
* Theme: clean green (dollar-like) theme, Roboto font, lightweight frontend.
* License & contribution: open-source — see LICENSE and Contribution section.

## Why this exists

Many wage-earners manually calculate their worked hours and wages every month.
This tool automates that process and helps you see the real income after daily
expenses (travel, food, other) and taxes. It’s intentionally simple so it can be
used by non-technical people and extended by developers.

## Features

* Select month from the current year (calendar-driven day rows).
* Toggle between 12-hour and 24-hour time formats.
* Start and end time per day; automatic calculation of hours/minutes worked.
* Automatic handling of overnight shifts (end time earlier than start time).
* Mark / unmark a day as Holiday (visually highlighted and excluded from pay).
* Weekly totals shown after each 7-day block.
* Monthly summary: total hours, worked days, gross pay, tax, total expenses,
  and final income after expenses and tax.
* Per-minute salary calculated automatically from hourly rate.
* Optional daily expenses: travel, food, other.
* Print the salary sheet and save a screenshot (watermark included).
* Designed to be easy to modify and style.

## Getting started (for developers)

1. Clone the repository:
   git clone <your-repo-url>

2. Open the project folder and serve the `index.html` file in a browser:

   * Option A: Open `index.html` directly in your browser (works for demo).
   * Option B (recommended for development): use a simple HTTP server.
     Example (Python 3):
     cd <project-folder>
     python -m http.server 8000
     Then open: [http://localhost:8000](http://localhost:8000)

3. No build tools required. All code is plain HTML/CSS/JS. One optional CDN:

   * `html2canvas` is used for screenshot export and is included via CDN in the
     HTML file. If you prefer offline, download and serve it locally.

## Configuration

* Edit the colour palette and typography in `style.css` (root CSS variables).
* The currency symbol is user-provided at runtime in the app.
* Per-hour rate, tax percentage, and daily expenses are entered in the UI.
* Time mode (12/24) can be switched while the sheet is open.

## Usage

1. Go to the Settings section.
2. Select the month (current year), enter your hourly rate and currency.
3. Optionally enter daily travel, food, and other expenses and tax percentage.
4. Click **Start calculation** — the sheet will be generated for that month.
5. Enter start and end times for each working day. Mark holidays if applicable.
6. See weekly totals appear automatically. View monthly summary at the bottom.
7. Use **Print Sheet** to print or **Save Screenshot** to download an image.
8. The watermark "Fair pay for your day" will appear in prints/screenshots.

## Contribution & Code of Conduct

This project welcomes contributions from the community. If you'd like to help:

* Fork the repository.
* Create a new branch for your feature or fix: `feature/your-feature`.
* Make changes, test locally, and create a pull request with a clear description.
* Write tests or usage examples where appropriate.

Please follow a respectful code of conduct:

* Be kind, constructive, and patient.
* Do not harass or threaten maintainers or contributors.
* Use clear commit messages and document breaking changes.

## Security & Responsible Use

This software is a client-side calculator tool. It does not collect data by
default. If you adapt it to store data (localStorage, server backend, or cloud),
please follow security best-practices (encryption, authentication, input
validation, and privacy policies).

## DISCLAMER & IMPORTANT LEGAL NOTE (READ CAREFULLY)

Publishing, redistributing, or repackaging this project is allowed under the
project license (see LICENSE), but the following actions are strictly forbidden:

* Publishing the project under another person's name or claiming ownership.
* Using this project as a tool for fraudulent or illegal activities.
* Modifying this source to spread misinformation or to impersonate public or
  private services.
* Republishing, selling, or distributing the project in a way that hides the
  original authorship or violates the license terms.

Any misuse of this source code for illegal, fraudulent, or deceptive purposes
is a violation of the terms and may be subject to legal action. By using this
project you agree to use it responsibly and ethically.

## License

This project is open-source. See the included `LICENSE` file for details. If a
specific license is not included, please contact the repository owner before
reusing the code in a commercial product.

## Acknowledgements & Credits

* Original design and implementation by the project authors.
* Icons and visual elements: Brave icons and open-source emoji (as noted in the
  footer/credits in the site).
* Screenshot feature powered by `html2canvas` (included via CDN).

## Contact & Support

For bugs, feature requests, or questions:

* Open an issue in the repository.
* Submit a pull request for improvements.
* If you need to contact the author directly, include a contact method in your
  pull request or issue (do not post private data publicly).

## Roadmap (ideas for future work)

* CSV and PDF export of the salary sheet.
* Local storage / user profiles for persistence.
* Multi-month and year comparison reports.
* Paid time-off / sick leave handling and accrual tracking.
* Localization and multi-currency formatting.
* Mobile-first responsive refinements and accessibility improvements.

## Changelog

v1.0 — Basic UI, monthly sheet generator, weekly totals, print & screenshot export.
(Keep an ongoing CHANGELOG.md in the repo for subsequent releases.)

## Final note

This is intentionally a simple, transparent, and modifiable tool for individuals
and small teams to track work hours and estimate true income after basic
expenses. If you build something cool from it, consider contributing back!

–––––––––––––––––––––––––––––––––––––––––––––––––
END OF README
––––––––––––––––––––––––––––––––––
