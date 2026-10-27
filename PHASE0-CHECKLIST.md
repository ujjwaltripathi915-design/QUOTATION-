# Phase 0 — Preparation Checklist
**Project:** Quotation ERP — Khandelwal Plastic Industries + Satyam Polymers  
**Specification:** *Master Build Prompt: Quotation ERP (Khandelwal Plastic Industries + Satyam Polymers).pdf*  
**Status key:** `[ ]` not checked · `[x]` verified · `[!]` needs attention

> This checklist is a preparation document. Do not enter passwords, recovery codes, secret keys, or full bank credentials into chat. Store sensitive details only in the appropriate secure account/settings page.

## 1. Development environment — needed now

- [ ] Open **Cursor** and open the existing Quotation ERP project folder (do not create a second project folder if one already exists).
- [ ] Open **Terminal → New Terminal** in Cursor.
- [ ] Run `node -v`; record the exact output.
- [ ] Run `npm -v`; record the exact output.
- [ ] Run `git --version`; record the exact output or the full error.
- [ ] Confirm whether the project folder already contains files. Do not overwrite or replace existing work before inspecting it.
- [ ] Confirm whether Git is available. If unavailable, local development can still be inspected; version history and phase commits will remain unavailable until Git is installed/configured or another approved version-control route is set up.
- [ ] Do not start Phase 1 until Phase 0 is reviewed and the owner explicitly approves continuation.

## 2. Accounts — needed now

Create or confirm these accounts and enable two-step verification (2FA) on each:

- [ ] **GitHub** — repository and source history. The free plan is generally suitable for a personal project; check current limits and private-repository features before launch.
- [ ] **Supabase** — PostgreSQL database, authentication and private file storage. Select the **Mumbai region (ap-south-1)** for the development project. A free tier may be suitable for development; review current limits, backups, pausing and production requirements before launch.
- [ ] **Vercel** — application hosting and deployment. A free/Hobby plan may suit personal development, but check current plan terms, commercial-use eligibility, function limits and production needs before launch.

Never share account passwords, recovery codes, database passwords, or secret keys in chat.

## 3. Company details

### Khandelwal Plastic Industries

**Needed now to prepare accurate production documents; placeholders may be used during development.**

- [ ] Full legal/display name confirmed.
- [ ] Registered/business address, city, state, PIN.
- [ ] GSTIN and PAN.
- [ ] Phone number(s), email, website (if any).
- [ ] Bank name, account name, account number, IFSC and branch.
- [ ] Logo, seal and signature as PNG files with transparent backgrounds.
- [ ] 7–8 actual approved Terms and Conditions.
- [ ] One old quotation with customer-identifying information removed, as a formatting sample.
- [ ] Confirm quotation prefix `KPI`.

### Satyam Polymers

**Needed now to prepare accurate production documents; placeholders may be used during development.**

- [ ] Full legal/display name confirmed.
- [ ] Registered/business address, city, state, PIN.
- [ ] GSTIN and PAN.
- [ ] Phone number(s), email, website (if any).
- [ ] Bank name, account name, account number, IFSC and branch.
- [ ] Logo, seal and signature as PNG files with transparent backgrounds.
- [ ] 7–8 actual approved Terms and Conditions.
- [ ] One old quotation with customer-identifying information removed, as a formatting sample.
- [ ] Confirm quotation prefix `SP`.

**Can be added later in Settings:** branding files and company profile details may be entered later while building/testing with clearly marked placeholders. A non-Draft/final PDF must remain blocked until the company profile has the required verified details.

## 4. Shared setup information

- [ ] Choose the owner's Login ID.
- [ ] Confirm a recovery email (do not post it publicly in project files).
- [ ] Prepare a list of 20–30 main items and their rates **for each company separately**, including units and any known specifications.
- [ ] Prepare a list of around 10 main customers. Avoid importing real customer data until security and access policies have been tested.
- [ ] Confirm that `KPI` and `SP` are the intended prefixes. The PDF specifies these as the defaults.

## 5. Questions for the Chartered Accountant (CA)

Do not guess these values in the application. Keep them as unconfirmed until the CA advises:

- [ ] Applicable GST rates for the actual products.
- [ ] Applicable HSN codes.
- [ ] GST treatment of freight and packing charges.
- [ ] Whether the proposed round-off treatment is appropriate.
- [ ] Whether e-invoicing may apply in the future.

## 6. Design requirements to retain for Phase 1

- [ ] Ocean Aurora theme for Khandelwal Plastic Industries (blue, teal and green).
- [ ] Rose Silk theme for Satyam Polymers (light red and cream).
- [ ] Neutral accent for All Companies view.
- [ ] Working company switcher and collapsible sidebar, including `Ctrl+B`.
- [ ] Light and dark modes.
- [ ] Distinct Design A and Design B A4 quotation previews.
- [ ] Responsive previews for desktop, tablet and phone.
- [ ] Animation timings: status-chip colour cross-fade 250 ms; button press scale to 0.97 for 100 ms; sidebar width 250 ms; company theme transition 300 ms; illustration floating loops 6–10 seconds using transform only.
- [ ] Respect `prefers-reduced-motion`; do not animate in print/PDF.
- [ ] No real database or real business/customer data in the design-only Phase 1.
- [ ] Confirm ₹ rendering in every used font and record gradient-text contrast results.

## 7. Safety and project handling

- [ ] Never put secrets in chat, source control, browser code, or `NEXT_PUBLIC_` variables.
- [ ] `.env.local` must stay out of Git; `.env.example` must contain placeholders only.
- [ ] Do not deploy with real business data before required security and testing gates pass.
- [ ] Inspect existing files before changing architecture or replacing anything.
- [ ] Keep the two companies' branding, quotation numbers, bank details, generated PDFs, filenames and metadata isolated.
- [ ] Do not invent company/legal details or legal/commercial T&C wording.
- [ ] Use visibly marked `[PLACEHOLDER]` company values and `[SAMPLE]` T&C only where the specification permits them; warn before printing.

## 8. Phase 0 verification record

| Check | Result / evidence |
|---|---|
| Original 50-page PDF reviewed | Reviewed for the phase plan, stack, core rules, database/security, business logic, UI, PDF, tests and deployment requirements |
| Existing project folder inspected | Pending — local Cursor workspace is not directly accessible from this chat |
| `node -v` | Pending owner output |
| `npm -v` | Pending owner output |
| `git --version` | Pending owner output |
| GitHub / Supabase / Vercel account and 2FA check | Owner confirmation pending |
| Checklist file | Created in the provided preparation workspace; must be copied into the actual project at `docs/PHASE0-CHECKLIST.md` if that folder is not this workspace |

## 9. Owner's next action

In Cursor, open **Terminal → New Terminal**. Copy and run these commands **one at a time**, pressing Enter after each:

```powershell
node -v
npm -v
git --version
```

Copy the exact three outputs back. If a command errors, copy the complete error message instead. Do not install or change anything yet; first review the actual result.
