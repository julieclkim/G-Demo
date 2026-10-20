# Genesys Interaction Detail Demo v3

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

Upload `index.html` and the `assets` folder to the root of a GitHub Pages repository.
