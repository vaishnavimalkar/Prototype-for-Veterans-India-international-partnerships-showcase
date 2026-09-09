# QA Note — International Partnerships Showcase (Prototype)

Manual test pass, performed in Chrome (desktop, 1440px width) and via
Chrome DevTools device emulation (mobile, 375px width — iPhone SE profile).

## 1. Layout (desktop)
- **Steps:** Open `index.html` at full desktop width (≥1200px).
- **Expected:** Masthead, purpose panel, category grid (5 across),
  partner card grid (multi-column), form panel, and CTA banner all render
  within a centred 1080px max-width column with consistent spacing.
- **Result:** Pass. All sections render in order with no overlapping
  elements or broken grids.

## 2. Mobile view
- **Steps:** Resize viewport to 375px width (or use DevTools device
  toolbar set to a small phone).
- **Expected:** Masthead stacks vertically, nav links wrap, category and
  partner card grids collapse to a single column, CTA banner stacks
  text above the button, no horizontal scroll.
- **Result:** Pass. Layout reflows to single column at the 640px
  breakpoint; no horizontal scrollbar appears.

## 3. Required-field validation
- **Steps:** Click "Submit enquiry" on the form with all fields empty.
- **Expected:** Name, organisation, country, email, proposed
  collaboration, and consent checkbox are all flagged invalid; each
  shows a visible, field-specific error message; focus moves to the
  first invalid field (Name); no acknowledgement message appears.
- **Result:** Pass.

## 4. Invalid email handling
- **Steps:** Fill in all required fields, but enter `not-an-email` in the
  Email field, then submit.
- **Expected:** Email field is flagged invalid with the message "Please
  enter a valid email address (e.g. name@example.org)"; form does not
  submit; acknowledgement message does not appear.
- **Result:** Pass. Re-entering a valid address (e.g.
  `demo@example.org`) and resubmitting clears the error and shows the
  acknowledgement message.

## 5. Keyboard navigation
- **Steps:** Using only the Tab / Shift+Tab / Enter / Space keys, navigate
  from the "Skip to main content" link through the nav links, category
  filter buttons, partner card evidence links, form fields (including the
  consent checkbox via Space), and the submit button.
- **Expected:** A visible focus outline appears on every interactive
  element in a logical order; the skip link is reachable as the very
  first Tab stop; the consent checkbox toggles with Space; the form can
  be fully completed and submitted without a mouse.
- **Result:** Pass. Focus order follows visual/DOM order; all
  interactive elements show a visible focus ring (brass-coloured
  outline); filter buttons and evidence links are reachable and operable
  by keyboard.

## Notes
- No automated test suite included (out of scope for a static prototype);
  all tests above were performed manually.
- Screenshots/recording referenced in the evidence package were captured
  during this same session.
