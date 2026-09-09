# Veterans India — International Partnerships Showcase (Prototype)

Prototype for the "International Partnerships Showcase" assignment. Built as a
single self-contained HTML file (HTML + CSS + vanilla JavaScript, no build
step, no backend, no dependencies).

## How to run it

1. Download / clone this folder.
2. Open `index.html` directly in any modern browser (double-click it, or
   right-click → Open With → your browser).
3. No server, install step, or API key is required — everything runs
   client-side.

Optional, if you prefer serving it locally:
then visit `http://localhost:8000/index.html`.

## What's included

- **Purpose statement** — short paragraph on why Veterans India runs
  international partnerships.
- **Partner categories** — five categories (veterans' organisations,
  universities/HEIs, CSR/foundations, diaspora/community organisations,
  knowledge partners) with demo counts.
- **Partnership cards** — each card shows organisation, country, contact
  status (Active/Pending/Lapsed), focus area, next action, owner, and an
  evidence link. A category filter lets you narrow the list.
- **Collaboration enquiry form** — name, organisation, country, email,
  proposed collaboration, consent checkbox, and an on-screen submission
  acknowledgement. The form does not send data anywhere; it only validates
  and displays a confirmation message client-side.
- **Opportunities / completed collaborations / contact CTA** — three
  dedicated sections as specified.
- **Responsiveness & accessibility** — single breakpoint at 640px for
  mobile; skip-to-content link; labelled form fields with `aria-describedby`
  error messages; visible keyboard focus states; `role="alert"` /
  `role="status"` for dynamic messages.

## Design assumptions

- No real partner list, branding guide, or copy was supplied, so all
  organisation names, countries, and figures are placeholder/demo data,
  clearly marked as such in a banner at the top of the page.
- No backend, database, or email service was requested — the enquiry form
  is a functional *front-end* prototype only (validates input, shows an
  acknowledgement, does not persist or transmit data).
- Visual direction: a restrained navy/cream/brass palette with a serif
  display face for headings, meant to read as an institutional registry
  page rather than a marketing site — appropriate to a veterans' welfare
  organisation rather than a consumer product.
- Built as a single HTML file for easy review and portability; this can be
  split into components/framework code later if the organisation adopts a
  particular tech stack.

