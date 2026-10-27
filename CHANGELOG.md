# Change log

## Multi-page integrity and delivery correction
- Preserved the agreed editorial + interactive visual direction and core content model.
- Kept six separate pages: home, story, model, workplace issues, reflection framework and assessment.
- Corrected homepage CTAs that pointed to missing in-page anchors so they navigate to the corresponding separate pages.
- Standardized primary navigation by exposing the workplace issues page alongside story, model and assessment.
- Removed unused duplicate assessment app/data scripts to reduce confusion; the assessment page loads the single active `js/assessment.js` implementation.
- Expanded documentation to record objective, audience, use cases, factors, assessment behavior, scope boundaries, privacy, limitations, policy framing and design/engineering principles.

## Design baseline (locked unless requested)
- Editorial + interactive experience.
- Multi-page structure; do not consolidate into a one-page document.
- Core audience: students and early-career workers.
- Objective: understand the workplace wellbeing issue and help users reflect on job experience with explanations and possible actions.
- Four-factor model: what you do; how much you earn; where you work; who you work with.
- Assessment: 3 prompts per factor (12 total), 1–5 responses, optional skip, factor-level interpretation and action plan.
- Privacy: session/page memory only, no remote submission or persistent storage.
- Targeted content: culture/trust, compensation fairness, early-career job evaluation, and organizational responsibility.
- Change control: only necessary changes unless the user authorizes a broader revision.

## V1 styling preservation and navigation pass

- Restored the V1 editorial design baseline rather than applying a new visual redesign.
- Kept the local SVG workplace illustrations and the four-factor editorial artwork.
- Kept the assessment as a separate HTML page with its interactive 12-prompt flow.
- Added a consistent Guided reflection link to the main navigation on each page.
- Retained the project boundaries: browser-only processing, no account/backend, and no persistent assessment storage.
- Package verification covers file structure, local references, script syntax, and ZIP integrity. This does not constitute exhaustive real-browser testing.

## Assessment interaction and sizing fix

- Preserved the reader's current viewport position when moving between questions; removed heading focus that could contribute to scroll jumps.
- Applied a short fade/translate transition between question states.
- Reduced quiz response tile padding, text size, progress spacing and question heading size.
- Used a compact two-column response layout on larger viewports and one-column compact tiles on narrow mobile screens; the skip option spans the row on wider layouts.
- Existing reduced-motion handling remains in place.

## Quiz navigation and results readability fix

- Stabilized question changes by removing focus from the submitted control, temporarily disabling smooth-scroll behavior, and restoring the quiz panel's viewport anchor after its fade transition.
- Kept question fade-out/fade-in transitions and reduced response option padding and typography, with tighter mobile sizing.
- Rebuilt the initial results view as a compact summary: overall answered-point percentage, four-factor score cards, and priority actions.
- Moved extended assets/gaps/action detail and remaining factor interpretations into native expandable disclosures, preserving the detailed result content with substantially less initial scrolling.
- Added responsive styling for the summary, factor cards, action prompts, and disclosures.
- Verification: JavaScript syntax check passed; local references passed; ZIP integrity passed. Browser-specific interaction QA remains recommended.

## Interior-page visual refinement

- Reduced oversized page titles, section spacing, prose type scale, card padding and vertical margins across story, model, issues and guided-reflection pages.
- Reduced editorial illustration maximum heights and adjusted crop/radius for more balanced reading proportions.
- Improved page content measure and responsive rules, with denser but readable card and issue layouts.
- Retained the V1 typography, palette, shapes, local illustrations and quiz-specific interaction/report refinements.
- Verification: JavaScript syntax checks passed; local page/assets references passed; ZIP integrity passed. Visual browser QA is still recommended.


## Results layout adjustment
- Updated the remaining-dimensions section to display three cards in one row on wide screens.
- Prevented collapsed cards from stretching to match expanded cards; added tablet and mobile responsive layouts.
