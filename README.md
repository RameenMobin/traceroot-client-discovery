# TraceRoot client discovery form

Standalone inbound discovery questionnaire for TraceRoot onboarding.

Clients fill the form in the browser. Progress auto-saves in `localStorage`. They download answers as JSON and email them to TraceRoot.

## Local preview

```bash
npx serve .
```

## Deploy to Vercel (this repo only)

```bash
npx vercel --prod
```

Or: Vercel → **Add New Project** → import **this** repository → Deploy  
(no framework, no build command — static `index.html`).

Do **not** connect the SilverBirch-FE monorepo.

## Client workflow

1. Open the Vercel URL.
2. Fill the form.
3. **Download answers (JSON)** → email TraceRoot.
4. Optional: **Print** for a paper/PDF snapshot.
