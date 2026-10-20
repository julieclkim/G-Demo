# Interaction Details Demo Builder

Static, GitHub Pages-ready demo replica focused on the Genesys Interaction Details transcript experience.

## Included

- High-fidelity top Genesys navigation with supplied Genesys mark and profile image
- Roboto typography
- Clickable Internal participant control with the participant popover
- High-fidelity External participant block with name, phone, sentiment score, and trend treatment
- Clickable AI Insights and Events tabs
- Five patient access center scenario templates
- Editable transcript lines, timestamps, speaker roles, participant details, sentiment score, AI insights, and events
- Topic, positive, negative, empathetic, and unhelpful events
- Click an event or timeline marker to jump to the related transcript line
- Drag timeline markers in Edit mode to change event timing
- Searchable transcript
- Two-page simulated recording timeline and playback simulation
- Annotation markers
- AI outline toggle, OFF by default, with scenario-specific outline templates and expandable sections
- Presentation mode that hides the demo editing toolbar
- Browser-local save plus JSON export/import

## Scenario templates

1. Referral appointment
2. New patient scheduling
3. Reschedule / cancel appointment
4. Insurance / prior authorization
5. Billing / payment question

These are practical demo scenarios, not a statistically ranked list of patient access contact reasons.

## Publish with GitHub Pages

1. Create or open the GitHub repository you want to use.
2. Upload the **contents** of this folder to the repository root, including the `assets` folder.
3. Commit the files.
4. In GitHub, open **Settings > Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select your main branch and `/ (root)`.
7. Save.

No backend or build step is required.

## Editing and presenting

- Use the dark Demo Builder toolbar to choose a scenario and edit content.
- Transcript and AI insight text can be edited directly while Edit mode is active.
- Event labels, categories, and timestamps can be edited in the Events panel.
- Drag a marker on the recording timeline to move that event.
- Click **INTERNAL** or **Multiple** to open the internal participant popover.
- Toggle **AI outline** on to switch the transcript into scenario-specific outline sections. It starts off by default.
- Choose **Presentation mode** before showing the screen.
- Press `Ctrl+Shift+E` to return to Edit mode while the toolbar is hidden.
- Save locally to persist changes in that browser.
- Export JSON to move a scenario to another browser or machine.

## Important

This is a standalone demo simulator. It does not connect to Genesys Cloud or pull real interaction data.
