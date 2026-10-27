# Work, Well — Job Satisfaction & Workplace Wellbeing

A multi-page, editorial + interactive static website for an educational assignment inspired by the Times of India article *“When the Pay Was Terrible, But the Friendships Priceless.”*

## Pages

- `index.html` — landing page and routes through the project
- `story.html` — article-inspired summary and reflection
- `model.html` — four-factor model
- `issues.html` — workplace challenges and organizational good practices
- `framework.html` — guided reflection
- `assessment.html` — interactive 12-item self-check and personalized report

Every page is a separate HTML document. Navigation links connect pages; shared presentation is in `css/styles.css`. The original V1 editorial visual system is retained, including its paper/forest-green/rust palette, serif headlines, spacing, card treatments, and local workplace illustrations. Guided reflection is linked from the primary navigation.

## Run locally

**Option A:** Extract the archive and open `index.html` in a modern browser.

**Option B (recommended):** From this folder run `python -m http.server 8000`, then visit `http://localhost:8000`. No build, dependency installation, backend, account or network connection is required.

## Assessment

- 12 prompts, three per factor; response scale 1–5 plus “prefer not to answer / not applicable.”
- Four dimensions: what you do; how much you earn; where you work; who you work with.
- Factor-level scoring, relative patterns, explanation of possible assets and gaps, practical actions and optional conversation starters.
- Skipped items are excluded from the scored denominator. The report explains its descriptive bands and limitations.
- Back navigation retains current-page answers. Retake restarts the check-in.
- Responses remain in page memory; they are not transmitted or saved persistently. Navigating away or reloading clears them.

## Interpretation limits

This is an educational reflection aid, not a validated psychometric instrument, clinical assessment, formal employee survey, workplace investigation, safety certification, legal/financial advice, or substitute for professional support. The factors are a practical lens, not exhaustive or universally weighted. Scores do not diagnose a person or employer and must not dictate resignation. A positive average cannot cancel out specific harassment, retaliation, discrimination or safety concerns.

## Primary issues and policy lens

1. Workplace culture, trust, power-play, respect and psychological safety.
2. Adequate/fair compensation, transparency and equity.
3. Early-career job evaluation beyond prestige or title—considering actual tasks, conditions and relationships.

Organizations can support wellbeing through fair and transparent pay practices, accountable leadership, safe voice routes, reasonable workload and job design. These are proposed good practices, not claims about universal legal requirements.

## Scope

**Included:** article brief summary; four-factor explainer; issue context; guided reflection; 12-prompt assessment; personalized factor-level report; actions; responsive editorial presentation; documentation.

**Excluded:** user accounts, server/backend, persistent answer storage, telemetry/analytics, employer ratings or comparisons, scientific validation, diagnosis, formal legal-compliance audit, automated resignation advice, or collecting sensitive workplace details.

## Design and engineering principles

- **Editorial + interactive:** narrative-led pages paired with a practical check-in.
- **Multi-page focus:** each page has a distinct task; navigation keeps the journey coherent.
- **DRY / separation of concerns:** shared CSS; assessment logic isolated from page markup.
- **Orthogonality:** story, model, issue context, reflection and assessment each have a clear purpose.
- **KISS:** plain HTML, CSS and JavaScript without dependency setup.
- **Accessibility:** semantic page landmarks, skip links where supplied, native rating controls, progress semantics, and responsive styles.
- **Privacy by design:** no accounts, analytics, remote submission or persistent response storage.
- **Small iterations / change control:** preserve the agreed content model and visual direction; make targeted fixes rather than unrequested redesign.

## Content attribution

The story page paraphrases the assignment/article brief, not the full article. It avoids presenting invented direct quotations.

## Verification

Run through each page link and complete the assessment end-to-end. Check back/forward behavior, skip behavior, factor scoring, result explanations, retake, keyboard operation and narrow-screen layout in the target browser.
