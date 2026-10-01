# Xavier Nursing Recruiting Experience

## Purpose
A deliberately small prototype to answer one question:

> Could the Xavier College of Nursing dean imagine using an interactive experience like this to recruit prospective students?

## Includes
- Browser camera access
- TensorFlow.js + BlazeFace face detection
- Smoothed face tracking
- Canvas-based visual treatment
- One guided recruiting question
- Four simple outcome messages
- No backend, database, generative AI API, CRM integration, or student-data collection

## Intentionally not copied from viking-helmet-AI
- NKU branding and teaching copy
- Griffin Hall / BodyPix flow
- Filter selector
- Glasses or helmet assets
- Selfie download
- Instructor-email flow

## Success criterion
Stop building when the dean can react to this question: **Could I imagine using this to recruit students?**

## Run locally
Camera access usually requires HTTPS or localhost. From this folder:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Suggested repo name
`xavier-nursing-recruiting-experience`
