# Fabrons Accounting Ltd. website

This is a small, static, single-page website. It uses only `index.html` and `styles.css`; there is no build step, JavaScript dependency, backend, database, external font, analytics, or embedded map.

## Preview and edit

Open `index.html` in a browser to preview the page. Edit the HTML to change copy, links, or package information, and `styles.css` to change presentation. The page uses system fonts and has no external assets to install.

## Basic hosting

Upload `index.html` and `styles.css` to the website's document root. Configure the hosting plan to serve `index.html` as its default document and enable HTTPS. The exact redirect/configuration syntax depends on the hosting provider and server; do not install IIS-, Apache-, or other host-specific rules until the host is known. Back up the current site and hosting configuration before changing files.

If the domain also handles email, preserve its existing mail and DNS settings when updating website hosting or DNS. Do not make domain or deployment changes without confirming the provider and current configuration.

## Legacy URL redirects

Configure permanent redirects at the hosting provider, where supported. The provider/server is not known, so these are destination mappings only:

| Legacy URL | Destination |
| --- | --- |
| `/default.aspx` | `/` |
| `/services.aspx` | `/#services` |
| `/packages.aspx` | `/#packages` |
| `/contact.aspx` | `/#contact` |
| `/partners.aspx` | Retire the page; return a not-found response or redirect to `/` rather than implying partner relationships |

Confirm that the host preserves the fragment destinations as needed; URL fragments are normally handled by the browser and are not sent to the server.

## Pre-launch confirmation gates

Do not treat legacy copy or prices as approved public information. Before launch, confirm:

- The service scope and current descriptions.
- Every legacy package price, monthly billing interval, inclusion, condition, and tax treatment. The package cards reproduce the old GIF artwork and the legacy page's terms, including its statement about providing Xero software and training; they are reference material only until confirmed.
- Whether Xero is still a required record-keeping assumption, and the turnover threshold and payroll terms.
- The company's registered name, jurisdiction, registered-office disclosure, and company number. The old site displayed number `09141314`, which has not been verified and is intentionally omitted here. The supplied Bolton address is shown as a contact address, not represented as a registered office.
- Privacy wording and any additional disclosures appropriate to the final service and contact process. The in-page privacy note is a placeholder, not a legal determination.
- Contact details, including the supplied phone number, email, and address.

No opening hours, qualifications, accreditations, testimonials, or partner relationships have been asserted.
