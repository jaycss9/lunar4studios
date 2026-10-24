# Lunar4

Static multipage music website inspired by https://7clouds.org/.

## Editing
- `dist/config.js`: form endpoint, business email, release catalogue, channel links.
- `build.py`: page content and shared layouts. Run `python build.py` after editing.
- `dist/style.css`: responsive styling.
- `dist/app.js`: navigation, article filters, form delivery and catalogue rendering.
- `/setup`: complete form setup guide on the site.

All original page categories are represented; article details use three original starter stories, not the source site's article archive. Artist rosters, subscriber counts and partnerships are not copied as Lunar4 claims.

## Form setup
1. Create a form at https://formspree.io/ and verify your notification email.
2. Copy its `https://formspree.io/f/...` endpoint into `formEndpoint` in `dist/config.js`.
3. Add your real email and complete/review the legal pages in `build.py` with your operator and data practices.
4. Set `legalApproved: true`, regenerate if content changed, then redeploy.
5. Send a test, confirm receipt in Formspree and email, and delete the test.

The form sends listening links, not uploaded audio. Formspree stores records and delivers notifications. No API secret belongs in config.js. The endpoint is public. Blank configuration disables sending and never reports fake success.

## Assets
The reference music video poster is used for this private design preview. Source: https://7clouds.org/. Replace with your own licensed media before public launch. No reference branding or staff identities are included.

## Verification
JavaScript syntax and all local page/asset references checked. Browser QA was not requested. Formspree delivery cannot be tested until an endpoint is supplied. WebMCP form staging is feature-detected; live WebMCP validation was unavailable.
