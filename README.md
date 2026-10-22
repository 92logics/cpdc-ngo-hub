# NGO management hub (prototype)

Prototype by [92 Logics](https://www.92logics.com), prepared as a sample for the Caribbean Policy Development Centre (CPDC) call for the technical build-out of an AI-enabled institutional management software package for Caribbean NGOs. It is not an official CPDC system. Fictional sample data only. Scripted AI drafts only.

Live demo: https://92logics.github.io/cpdc-ngo-hub/

## What it shows

A public, clickable sample of a multi-organisation hub for small and medium-sized NGOs. Four fictional NGOs share one application, and each sees only its own users, projects, finances, documents and reports.

- **Sign-in with roles:** choose an organisation and a role (Admin, Programme Officer, Finance, Viewer), then pass a mock MFA code step. Permissions change what each role can edit, post, approve or see.
- **Dashboard:** projects, open and overdue tasks, budget spent, indicators on track, and a "needs attention" check for missing or overdue information.
- **M&E indicators:** baseline, target, actual, progress and status, with logged progress updates.
- **Project plans and tasks:** workplan tasks with owners, due dates and status, plus a timeline by project.
- **Budget and general ledger:** budget lines, budget versus actual, and a ledger with vouchers, invoices and receipts linked to each posting.
- **Document library:** contracts, consultant outputs, vouchers, invoices, receipts and verification evidence, linked to projects.
- **Reports and exports:** project progress, M&E, budget versus actual, general ledger and workplan reports, downloaded as PDF, Excel or CSV. The files are built in the browser.
- **AI drafting with human review:** narrative reports, M&E updates, workplans, budget notes and proposal sections drafted from the organisation's records. A person edits the draft, then approves it or requests changes. Every step goes into the review history and the audit trail.
- **Audit trail:** sign-ins, exports, postings, indicator updates and draft reviews, exportable to CSV.

The AI drafts are scripted templates filled from the sample records. Nothing calls a live AI API, nothing is uploaded, and nothing leaves the browser. There are no API keys and no real personal data.

## How it maps to the TOR deliverables

| TOR deliverable | What this prototype shows |
| --- | --- |
| 1. Inception Report | Not a document here. The sample shows our reading of the scope before inception. |
| 2. Technical Requirements Validation | Multi-organisation separation, the role and permission model, sign-in with MFA, document types and the AI functions, in a form CPDC can click through. |
| 3. Technical Specifications and Working Test Version | A working sample of the core modules. The real test version would be built from CPDC's approved functional flow and interface requirements. |
| 4. Integrated Capacity-Building Hub | M&E, project and workplan, budgeting, general ledger, documents, narrative reporting, dashboards, downloads and AI-assisted drafting, all in one hub. |
| 5. Testing and User Acceptance | Role switching, data separation between organisations, financial totals, exports and the draft review flow can all be tried here. |
| 6. Fully Functional Hub, Training and Manual | Out of scope for the sample. The production hub would come with training and a user and administrator manual. |
| 7. Technical Handover and Final Completion Report | Out of scope for the sample. The production build would hand over source, database, configuration, backups and third-party service details. |

## Intended production stack

- **Application:** ASP.NET Core with Blazor or React.
- **Database:** SQL Server, with each organisation's data separated in the data model and enforced on every query.
- **Identity:** password rules, account recovery, session management, multi-factor sign-in, role-based permissions and audit logs for sensitive administrative and financial actions.
- **Documents:** secure file storage linked to projects and ledger entries.
- **Reports:** server-side PDF and Excel generation.
- **AI:** an AI service approved by CPDC in advance, with its costs stated, and a human review and approval step on every draft.
- **Hosting:** Azure or any cloud, with test and production environments and backups in place before go-live.

## Run it

Open `index.html` in a browser, or use the GitHub Pages copy. No install and no build step.

## Disclaimer

This is a 92 Logics prototype. It is not an official CPDC system and is not connected to any CPDC or NGO system. All organisations, people, projects and amounts are fictional. The AI drafts are scripted templates, not output from a live AI service.

## Contact

92 Logics · cowork@92logics.com · https://www.92logics.com
