# MF Data Solutions

Mauricio Forneron’s personal professional website. Plain HTML and one shared CSS file, with no build step, JavaScript, external fonts, analytics scripts or third-party assets.

- `index.html`: English page, including metadata and Person structured data.
- `de/index.html`: German page. Keep content changes in sync with the English version.
- `impressum.html` / `de/impressum.html`: Bilingual operator notice drafts.
- `privacy.html` / `de/datenschutz.html`: Bilingual privacy notice drafts.
- `style.css`: Shared styles, responsive layouts, reduced-motion and print rules.
- `favicon.svg`: Small text monogram.
- `CNAME`: Existing custom domain, `mf-datasolutions.com`.

## Preview

From the repository root, run `python3 -m http.server 8000` and open `http://localhost:8000`. The German version is at `/de/`.

## Updating

Edit the HTML directly. Contact links currently use `info@mf-datasolutions.com`; update every `mailto:` link and its displayed address in both pages if that changes. The LinkedIn profile is `https://www.linkedin.com/in/mauricio-forneron`; it is a plain outbound link and is also listed in Person structured data.

The existing `logo.svg` is retained but is not loaded by the pages. The design uses a lightweight text identity instead.

## Publishing

There is no build output to generate. Publish the repository’s static files using the existing hosting setup. GitHub Pages is configured to publish the root of `main` at `https://mf-datasolutions.com/`; pushing to `main` triggers publication. Local edits alone do not publish the website. Legal pages are drafts with visible placeholders and `noindex` metadata. They remain incomplete public drafts after a push; replace all placeholders and review them before treating them as finalized legal notices. Remove `noindex` once finalized. Footer links are present on both homepages and all legal pages.


## Legal/privacy details still needed

The operator is Mauricio Forneron personally in Germany. There is no registered company, Handelsregister entry or VAT ID associated with this website. The legal pages do not imply a paid consulting business.

Replace matching placeholders in both languages:

- `[PUBLIC_POSTAL_ADDRESS]`: complete address suitable for the public operator notice.
- `[PUBLIC_EMAIL]`: confirmed public contact address; reconcile with the current homepage email links.
- Hosting confirmed on 7 October 2026 through the GitHub Pages API, live `server: GitHub.com` response and DNS. The privacy pages name GitHub Pages and give GitHub, Inc.’s published contact address.
- GitHub documents IP logging for Pages security. `[HOSTING_ADDITIONAL_LOG_DATA]` remains for any additional log fields; these have not been established.
- `[HOSTING_LOG_RETENTION]`: actual retention/deletion period.
- `[HOSTING_PROCESSING_AND_TRANSFER_DETAILS]`: processing locations, recipients/provider role, any transfers outside the EEA, and applicable transfer safeguards. Confirm relevant data-processing arrangements; do not assume a processor agreement or safeguards exist.
- `[EMAIL_PROVIDER]`: actual provider’s legal name, including forwarding services if used.
- `[EMAIL_PROVIDER_ADDRESS/COUNTRY if required]`: relevant provider address and country.
- `[EMAIL_PROCESSING_AND_TRANSFER_DETAILS]`: processing locations, recipients/provider role, any transfers outside the EEA, and applicable safeguards.
- `[EMAIL_RETENTION_DETAILS]`: provider-side mailbox, deletion and backup retention. The operator’s inquiry-handling/deletion practice must also match the notice.

Before finalizing, confirm that the host adds no analytics, nonessential cookies, injected resources or other consent-requiring behavior. The source inspection cannot establish server-side behavior. Do not automatically install a consent platform if anything is found; report it first.

Legal references: [GDPR (especially Articles 6, 13, 15–21 and 77)](https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng), [§25 TDDDG](https://www.gesetze-im-internet.de/ttdsg/__25.html). Only verified GitHub hosting details have been filled. Retention and account-specific arrangements remain unconfirmed; email-provider wording is unfilled.

## Source privacy inspection

All HTML, CSS and SVG assets were inspected. The only script blocks are inert Person JSON-LD metadata. There are no executable scripts, event handlers, analytics integrations, pixels, browser storage APIs, social embeds, remote font downloads, CSS imports or external runtime resources. Fonts are system fonts. CSS and the favicon are local. The retained, unused `logo.svg` contains an embedded image, not a remote image. LinkedIn is an ordinary outbound hyperlink with `rel="noreferrer"`; no widget or preconnect is used. No cookie banner was added.
