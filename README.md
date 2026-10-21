# Genesys Interaction Demo Workspace

Static GitHub Pages demo replica for Interaction Detail.

## Default behavior
- Opens on Transcript with AI Insights selected.
- AI outline is off by default.
- AI Insights and Events are clickable tabs.
- Quality Summary opens the scenario-matched Auto Evaluation.
- Scenario edits are stored in `sessionStorage`, so they survive refresh/navigation in the same browser session and clear when the session ends.
- Reset Demo restores the selected template.
- Presentation mode hides demo-authoring controls. Press Ctrl+Shift+E to return to edit mode.

## Patient Access Center templates
1. Referral appointment and specialty scheduling
2. New patient scheduling
3. Appointment reschedule with transportation barrier
4. Prior authorization status before imaging
5. Symptom call routed to nurse triage

Upload `index.html`, `summary.html`, `live.html`, and the `assets` folder to the root of a GitHub Pages repository.

## Archive fidelity audit

This build uses the supplied SingleFile exports as the visual source of truth for the interaction-detail experience.

- Default view opens Transcript with AI Insights selected.
- Events uses the captured right-side panel proportions, filters, event colors, spacing, and timestamps.
- Quality uses the captured 60/40 layout: evaluation summary/table on the left and the active evaluation form on the right.
- All five patient-access templates include a Virtual Agent exchange by default. Use **Hide virtual agent** in Demo Builder when presenting without the bot portion.
- Quality forms and scores remain scenario-specific.
- Demo Builder changes persist in session storage until Reset Demo or the browser session ends.


## Multi-page demo workspace update

- `index.html` is now a home screen with tiles for **Interaction Summary** and **Live Voice Interaction**.
- `summary.html` contains the historical Interaction Detail experience.
- `live.html` recreates the supplied active voice interaction layout and uses CSS grid for the Conversations, Call Interaction, Profile, Copilot, and Tools regions.
- Scenario selection is shared across pages with `localStorage`.
- Caller name and phone are universally editable for the selected scenario and are shared between the live and historical pages.
- Live Voice Interaction uses JavaScript for the upward-running call timer, end-call pause behavior, scenario switching, profile synchronization, and Copilot search states.
- Clicking the Copilot search field auto-types the scenario-specific knowledge query, shows the supplied loading pattern, then surfaces scenario-specific knowledge results. The first result opens an article detail state.
- Post-call behavior remains intentionally deferred for the next build.

## v5 fidelity pass

- Restored the Genesys typography hierarchy using Noto Sans for body text and Urbanist for headings.
- Removed an accidental duplicate live Call Interaction header.
- Refined top navigation sizing, spacing, badges, queue controls, AI button, and agent avatar/info cluster against the supplied SingleFile captures.
- Quality remains docked at the captured 60/40 split, with a 220 px participant rail and a compact scenario-specific evaluation title.
- The external sentiment indicator is constrained to its participant card and no longer overflows.
- Browser QA covers all five scenarios, 13+ transcript turns per template, Copilot loading/results/article states, shared caller profile edits, timer behavior, Quality close/reopen behavior, and home-page routing.
