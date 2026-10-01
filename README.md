# Xavier Nursing Recruiting Experience

A deliberately small recruiting prototype designed to answer one question:

> Could the Xavier College of Nursing dean imagine using an interactive experience like this to recruit prospective students?

## Current design

The experience is intentionally reduced to **two meaningful taps**:

1. **See My Future** — opens the user's camera for a short future-self moment.
2. **Choose what pulls you toward nursing** — immediately reveals a personalized Xavier Nursing message and program proof point.

The camera moment advances automatically after a few seconds. There is no face tracking, no TensorFlow.js, no Continue button, and no dependency on AI model loading.

## Why the architecture changed

The earlier prototype used BlazeFace/TensorFlow face tracking. That introduced unnecessary load time and glitch risk without clearly improving the recruiting value.

The current build prioritizes:

- identity
- purpose
- personalization
- speed
- mobile reliability
- Xavier Nursing differentiation

## Technical architecture

- Static HTML/CSS/JavaScript
- `getUserMedia()` for the camera moment
- No backend
- No database
- No AI model dependency
- No image upload or storage
- Camera denial gracefully falls back to the recruiting question
- Final CTA links to Xavier's public nursing page

## Recruiting flow

```text
What kind of nurse will you become?
        ↓
See My Future
        ↓
2–3 second live camera moment
        ↓
automatic transition
        ↓
What pulls you toward nursing?
        ↓
one choice
        ↓
personalized Xavier result
        ↓
Explore Xavier Nursing
```

## Success criterion

The prototype is successful when the dean can answer:

> "Could I imagine using this to recruit students?"

Do not expand into CRM, analytics, lead capture, admissions integrations, chatbots, or complex AI until Xavier validates the recruiting use case.

## Live testing

When GitHub Pages is enabled from `main` / `(root)`, the expected URL is:

`https://brandinealnku.github.io/xavier-nursing/`
