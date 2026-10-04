# ATAOGO Operations Hub — Concept Demonstration

Built by **Vecora Technologies**.

An interactive frontend demonstration of a potential custom operations/workflow platform. It uses **fictional/sample data** and does not represent Ataogo's actual internal systems, actual projects or confirmed requirements. It is not an official Ataogo product.

## Technology and running locally

HTML5, CSS3 and vanilla JavaScript. No libraries, CDN, build command, API, server or environment variables are required. Extract the ZIP and open `ataogo-operations-hub/index.html` in a modern browser. Internet access is unnecessary for the application. The public-source reference link needs internet access.

Files:

- `index.html` — intro and application shell
- `css/style.css` — desktop, tablet, mobile and print styles
- `js/data.js` — interconnected fictional records
- `js/app.js` — views, workflow actions, filters, reports and persistence
- `assets/favicon.svg` — original concept monogram, not an Ataogo logo
- `RESEARCH.md` — public-source basis and limits
- `QA.md` — verification and known limitations

## Two-minute demonstration

1. Enter Demo. The default role is Management.
2. Projects → Delta Flowline Integrity & Maintenance Project → Overview. Explore the connected workflow and tabs.
3. Procurement → PR-2026-014 → Approve request → Confirm.
4. See the changed status and recorded activity. Dashboard counts update immediately.
5. Materials → MAT-011. The request needs two inspection probe kits.
6. Equipment → EQ-003. Explore assignment, maintenance, inspections and documents.
7. Field Operations → FO-001. View the resource dependencies and timeline.
8. HSE → HSE-2026-034. Review findings and corrective action. HSE-2026-033 is the linked Delta Flowline inspection.
9. Document Control → DOC-001 → Preview document.
10. Reporting → choose Delta Flowline → Generate Report. Review project, procurement, equipment, HSE and field records together; Export CSV or Print report.

## Complete the connected sample workflow

1. After approval, change the role menu to Procurement Officer. In PR-2026-014 select a fictional vendor, enter a rationale and create a sample purchase order.
2. Switch to Store/Materials Officer. Record a delivery reference and quantity. Partial receipts are supported; excess or duplicate full receipts are blocked by workflow state. Full receipt completes the request and adds two probe kits to MAT-011.
3. Switch to Equipment/Asset Officer. EQ-003 → Inspections → record sample clearance. This updates the fictional certificate revision. Overview → Change assignment/status → Assigned to Delta Flowline. Include a change note.
4. Switch to HSE Officer. HSE-2026-033 → Resolve with closure evidence.
5. Switch to Project Manager. FO-001 → Update status → Completed. This illustrative survey requires full receipt, assigned/cleared EQ-003 and closed HSE-ACT-019 first.
6. Generate the integrated report again. Activity Log records your browser-local changes.

Role selector controls available actions; all six roles can explore all sample modules. This is frontend simulation, **not secure access control**. Production roles and department access would be discovered and enforced on a backend.

## Persistence and resetting

Changes are stored under `ataogo-concept-v1` in browser localStorage. Activity Log → Reset sample data restores the initial dataset. Different devices, browsers and origins have independent copies. Some browsers restrict storage for local files; changes then remain in memory for that session. The intro appears each visit. Do not enter confidential information.

The initial dataset uses a fixed 4 October 2026 snapshot. Action timestamps use the current browser clock. Reporting filters use record dates, not historical status reconstruction. Receipts use their actual browser action timestamp. All records and amounts are fictional.

## GitHub Pages: exact setup

1. Sign in to GitHub and create a **public** repository named `ataogo-operations-hub`. Add a README if GitHub needs an initial commit.
2. Extract this ZIP on your computer.
3. Open the extracted `ataogo-operations-hub` folder. Upload its **contents**, not the enclosing folder, so `index.html` is at the repository root.
4. In the repository select **Add file → Upload files**. Drag in `index.html`, `css`, `js`, `assets` and the Markdown files together. If your browser does not upload folders, use GitHub Desktop or Git to preserve those directories. Do not upload only the ZIP.
5. Select **Commit changes** to the `main` branch.
6. Open **Settings → Pages**.
7. Under **Build and deployment**, choose **Deploy from a branch**.
8. Choose branch **main**, folder **/ (root)**, then **Save**.
9. Wait for the deployment to finish (check the Actions tab if needed). Return to Settings → Pages → **Visit site**.
10. Test the link on your phone before sharing. If there is a 404, confirm `index.html` is at the repository root and the Pages deployment succeeded.

Expected URL: `https://USERNAME.github.io/ataogo-operations-hub/`.

All asset paths are relative; no routing rewrites are required. Filenames and paths are case-sensitive on GitHub Pages.

## Suggested WhatsApp message

Good afternoon sir. As discussed, here is a short interactive concept demo prepared by Vecora Technologies: [DEMO LINK]. It shows how a custom platform could connect a project’s procurement, materials, equipment, field activities and safety reporting. All information is sample data, and the concept is not based on confirmed Ataogo requirements. Please tap “Enter Demo”; it works on your phone. I would appreciate your feedback when convenient.

## Production scope

There is no authentication, shared database, real document repository, real purchase order transmission or real certification. The browser activity log is editable browser data, not an immutable audit trail. Server-enforced role/department permissions, approval policies, protected audit history, real version control, integrations and secure validation are potential production capabilities subject to discovery. No payroll or financial accounting is implemented. Material reservations and receipts are shown; consumption is not fabricated from those quantities.
