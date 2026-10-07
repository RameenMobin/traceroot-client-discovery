# TraceRoot client discovery form

Standalone inbound discovery questionnaire for TraceRoot onboarding.

Clients fill the form in the browser. Dropdowns for roles, stage triggers/capabilities, and document metadata. Tables start short with **Add row**. Progress saves on-device under an optional draft name (Save progress + autosave). When finished they download answers and email them to TraceRoot.

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
2. Fill the form (optional draft name so they can return later on the same device).
3. **Download my answers** → email TraceRoot.
4. Optional: **Print** for a paper/PDF snapshot.

## Admin (TraceRoot)

In the workflows app → **Onboarding** → **Import discovery JSON**. Pick the client’s download. That seeds a draft tenant/profile (identity, parties, suppliers, stages, docs, failures, packs, case-wide). Review Stages / Failures (soft-draft failure codes), then **Save draft**.

Progress is stored in the browser (`localStorage`) under the draft name. Concurrent clients each use their own device (or distinct draft names on a shared computer).

