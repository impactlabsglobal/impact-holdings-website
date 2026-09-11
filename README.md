# Impact Holdings LLC Website

Official landing page for Impact Holdings LLC, a tax preparation and LLC formation business based in Perth Amboy, New Jersey.

## About The Business

Impact Holdings LLC helps individuals, contractors, and small business owners with professional tax preparation and business setup services in English and Spanish.

Services include:

- W-2 tax return preparation
- 1099 and self-employed tax preparation
- Mileage and business expense deduction support
- LLC formation packages
- EIN / Tax ID assistance
- Registered agent support
- Business domain and professional email setup

## Website

This project is a single-page HTML website built with:

- HTML
- CSS
- Vanilla JavaScript
- Responsive design for desktop, tablet, and mobile
- English / Spanish language toggle
- Light / dark theme toggle
- Contact form powered by FormSubmit
- Public service-milestone counter loaded from `service-progress.json`

Main file:

```text
index.html
```

## Live Website

The public website is available through GitHub Pages:

```text
https://impactlabsglobal.github.io/impact-holdings-website/
```

## Contact Form

The contact form currently sends inquiries to:

```text
founder@impactholdingsllc.com
```

The form uses FormSubmit:

```html
https://formsubmit.co/founder@impactholdingsllc.com
```

## Local Preview

To preview the website locally, open `index.html` in a browser.

You can also run a simple local server:

```bash
python3 -m http.server 4173
```

Then visit:

```text
http://localhost:4173
```

## Updating Completed-Service Counts

Edit only the `completed` values in `service-progress.json` after reconciling them with internal paid-and-completed service records. Do not count form submissions, estimates, canceled work, or unpaid requests. The public counter contains aggregate totals only and must never include client names or tax information.

The current public milestones are:

- W-2 tax returns: 1,000
- Uber/Lyft 1099 with driver-organized mileage: 1,000
- Uber/Lyft 1099 with driver-organized expenses: 1,000
- LLC formation packages: 700

Do not announce an active drawing until official rules define the prize, eligibility period, entry method, geographic restrictions, odds, privacy terms, and applicable legal requirements.

## Repository

GitHub repository:

```text
https://github.com/impactlabsglobal/impact-holdings-website
```

## Notes

Tax preparation and business formation services are not legal or financial advice. Clients should consult a qualified professional for advice specific to their situation.
