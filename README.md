# TraceRoot client discovery form

Standalone inbound discovery questionnaire for TraceRoot onboarding.

Clients fill the form in the browser. Dropdowns for roles, stage triggers/capabilities, and document metadata. Tables start short with **Add row**. Progress saves under a workspace name in `localStorage` (Save progress + autosave). Download answers as JSON when done.

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

## Save / continue & multiple clients

- Progress is stored in the browser (`localStorage`) under a **workspace name**.
- Click **Save progress** (also auto-saves a moment after you type).
- Come back later on the **same device and browser** to continue.
- **Multiple clients at once:** yes — each person uses their own browser/device. On a shared computer, use a distinct workspace name per client.
- When done, **Download answers (JSON)** and email it to your TraceRoot contact.

