[README.md](https://github.com/user-attachments/files/33624032/README.md)
# Real Estate Cinematic Video Workflow — Video Media World

A reusable adaptation of the browser-based VideoExpress documentary workflow for real estate property tours.

## What this repository is

This repository is a **prompt and operating-instructions package**, not a standalone executable application. It guides a browser-capable AI agent through preparing ten short property-video scenes in VideoExpress 3.5. The user reviews the generated assets and assembles the final video manually.

## Production defaults

- Brand: Video Media World
- Tool: VideoExpress 3.5
- Aspect ratio: Landscape 16:9
- Scene count: exactly 10
- Target clip duration: 8–10 seconds per scene; final edited clips must be no longer than 10 seconds
- Presenter: user's supplied portrait, used as a consistent identity reference
- Presenter presence: all ten scenes
- Dialogue: Romanian, presenter speaks directly to camera
- Lip sync: use the supported native speech or audio-driven lip-sync workflow; verify results rather than assuming success
- Editing: manual assembly by the user
- Property fidelity: preserve the source photos' real architecture, furniture, materials and layout

## Repository files

- `SYSTEM_PROMPT.md` — main instructions for the browser-capable agent.
- `SCENE_TEMPLATE.md` — copy-ready template for each of the ten scenes.
- `QUALITY_CHECKLIST.md` — review checklist for visual fidelity, presenter identity, dialogue, timing and editing.
- `PROJECT_INPUT_TEMPLATE.md` — intake sheet for each new property.

## Prerequisites

- Access to VideoExpress 3.5 and its supported generation features.
- A browser-capable AI agent that can follow a system prompt and interact with the visible interface.
- Ten property photographs, numbered in intended presentation order.
- The user's presenter portrait available as a reference image.
- Verified property facts and an approved Romanian call to action.
- A video editor for manual assembly.

Sign in yourself when the interface requests it. Never put passwords, API keys, or recovery codes into prompts or repository files.

## Start a new project

1. Open `PROJECT_INPUT_TEMPLATE.md` and fill in the facts for the property.
2. Prepare ten photographs and label them `01` through `10`.
3. Load `SYSTEM_PROMPT.md` as the browser agent's instructions.
4. Ask the agent to produce all ten scene prompt sets before generation.
5. Generate and inspect a pilot scene before making the remaining nine.
6. Generate each scene using the matching property image and presenter reference.
7. Check each clip's actual duration and spoken dialogue.
8. Assemble the ten clips manually in the intended order, balancing audio and adding restrained transitions.
9. Export only after the final quality checklist passes.

## Important limitations

- A prompt cannot guarantee that VideoExpress supports simultaneous use of both references, native dialogue generation, or a particular lip-sync mode. Confirm the current interface's available controls.
- A requested duration is not proof of the rendered duration. Check the actual clip and trim in the editor without cutting off dialogue.
- The ten photographs are source-of-truth references. Never invent features, room layouts, measurements, legal status, views, prices or amenities.
- If the presenter or room becomes visibly distorted, repair or regenerate that scene rather than accepting the defect.
- This workflow does not automatically publish, share publicly, or claim to have exported a video.

## Suggested GitHub fork workflow

1. Fork `ai-playbooks/historical-documentary-video-workflow` to your account.
2. Create a branch such as `real-estate-adaptation`.
3. Replace the original `README.md` and `SYSTEM_PROMPT.md` with the versions in this package.
4. Add `SCENE_TEMPLATE.md`, `QUALITY_CHECKLIST.md`, and `PROJECT_INPUT_TEMPLATE.md`.
5. Review the original repository's license and attribution requirements before publishing your modified fork.
6. Commit your changes and test the prompt on one property before scaling up.

The package is prepared locally for review. It has not been pushed to GitHub, and no fork is claimed to have been created by this package.
