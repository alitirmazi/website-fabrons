# Fabrons Accounting Ltd. website

This is a small, static, single-page website. It uses only `index.html` and `styles.css`; there is no build step, JavaScript dependency, backend, database, external font, analytics, or embedded map.

## Preview and edit

Open `index.html` in a browser to preview the page. Edit the HTML to change copy, links, or package information, and `styles.css` to change presentation. The page uses system fonts and has no external assets to install.

## Hosting and deployment

The site is hosted at <https://alitirmazi.github.io/website-fabrons/> using GitHub Pages. The workflow in `.github/workflows/pages.yml` publishes `index.html` and `styles.css` whenever a change is pushed to `main`; it can also be started manually from the repository's Actions tab. GitHub Pages serves the site over HTTPS. No build step, custom domain, or DNS change is required.

The repository is public to support GitHub Pages on its current plan. If changing hosting or DNS in the future, preserve any existing mail settings and back up the current configuration first.

## Legacy URL redirects

These are the desired destinations for legacy links:

| Legacy URL | Destination |
| --- | --- |
| `/default.aspx` | `/` |
| `/services.aspx` | `/#services` |
| `/packages.aspx` | `/#packages` |
| `/contact.aspx` | `/#contact` |
| `/partners.aspx` | Retire the page; return a not-found response or redirect to `/` rather than implying partner relationships |

The current Pages workflow deploys only the two site files above and does not implement legacy `.aspx` redirects. GitHub Pages does not provide server-side rewrite rules; decide how to handle these old URLs before retiring the previous host. URL fragments are handled by the browser and are not sent to the server.

## Pre-launch confirmation gates

Do not treat legacy copy or prices as approved public information. Before launch, confirm:

- The service scope and current descriptions.
- Every legacy package price, monthly billing interval, inclusion, condition, and tax treatment. The package cards reproduce the old GIF artwork and the legacy page's terms, including its statement about providing Xero software and training; they are reference material only until confirmed.
- Whether Xero is still a required record-keeping assumption, and the turnover threshold and payroll terms.
- The company's registered name, jurisdiction, registered-office disclosure, and company number. The old site displayed number `09141314`, which has not been verified and is intentionally omitted here. The supplied Bolton address is shown as a contact address, not represented as a registered office.
- Privacy wording and any additional disclosures appropriate to the final service and contact process. The in-page privacy note is a placeholder, not a legal determination.
- Contact details, including the supplied phone number, email, and address.

No opening hours, qualifications, accreditations, testimonials, or partner relationships have been asserted.
