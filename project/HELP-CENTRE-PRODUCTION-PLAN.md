# Seama Help Centre production plan

This file tracks the Help Centre from product mapping through publication. It is the operational source of truth for content production; `docs.json` remains the source of truth for published navigation.

## What finished means

The Help Centre is complete for launch when:

- every P0 article is published;
- every supported end-to-end workflow has been reproduced in the current product;
- all customer-facing steps use exact interface labels;
- screenshots use synthetic data and match the current interface;
- every article explains the expected result and how to verify it;
- unsupported or unresolved behaviour is not presented as normal;
- navigation, search, related links and mobile layout work;
- Mintlify validation, broken-link and accessibility checks pass;
- a named product owner approves each product area;
- a review date and revalidation process are in place.

P1 and P2 content can continue after launch. The launch has a defined end; routine updates then become maintenance.

## Status key

| Status | Meaning |
| --- | --- |
| Not started | No current workflow map or article |
| Mapping | Intended workflow and dependencies are being defined |
| Testing | Current product behaviour is being reproduced |
| Decision needed | Product owner must confirm the intended rule |
| Drafting | Customer-facing MDX is being written |
| Screenshots | Synthetic screenshots are being captured |
| Review | Content and product accuracy are being checked |
| Ready | Approved and technically validated |
| Published | Live and included in navigation |
| Revalidate | Product changed or verification is out of date |

## Required article fields

Every article must include:

- title and search description;
- audience and permissions;
- prerequisites;
- exact steps;
- decision points and state changes;
- expected result;
- verification step;
- warnings where an action cannot be safely reversed;
- troubleshooting;
- related articles;
- `lastVerified`, `reviewDate` and product-area owner.

## End-to-end workflow coverage

| Workflow | Starts with | Ends with | Launch priority | Status |
| --- | --- | --- | ---: | --- |
| Account setup | New company | Controlled test-ready account | P0 | Mapping |
| Customer setup | New client | Usable client, site, contact and billing record | P0 | Mapping |
| Quote to Workorder | Quote | Accepted and converted Workorder | P0 | Mapping |
| Direct Workorder | Client/site | Active scheduled Workorder | P0 | Mapping |
| Dispatch and field work | Active Workorder | Reviewed completed work | P0 | Mapping |
| Job to invoice | Completed work | Correct customer invoice | P0 | Mapping |
| Invoice to payment | Reviewed invoice | Sent, synced and reconciled payment state | P0 | Mapping |
| Supplier bill | Source document | Reviewed accounting record | P0 | Mapping |
| Bill to inventory/job | Reviewed bill | Correct stock or job-cost allocation | P0 | Mapping |
| Bill to Xero | Reviewed bill | Verified accounting-system result | P0 | Mapping |
| Inventory lifecycle | Item master | Reconciled quantity by location | P0 | Mapping |
| Composite item | Components | Correct bundle and component movement | P0 | Mapping |
| Reporting | Confirmed records | Traceable report result | P0 | Not started |
| Access control | Staff member | Correct role and permissions | P0 | Mapping |
| Templates and communications | Approved template | Delivered message/document | P1 | Mapping |

## Phase 1 — Foundation and product model

Exit condition: the information architecture, terminology, state model and article template are approved.

| Deliverable | Priority | Status |
| --- | ---: | --- |
| Help Centre home and navigation | P0 | Existing; review |
| End-to-end workflow overview | P0 | Existing; expand |
| Setup order | P0 | Existing; review |
| First controlled workflow | P0 | Existing; review |
| Go-live checklist | P0 | Existing; review |
| Product glossary | P0 | Existing; expand |
| Status and state glossary | P0 | Not started |
| Data ownership and inheritance map | P0 | Mapping |
| Article template and editorial rules | P0 | Existing; review |
| Screenshot and synthetic-data standard | P0 | Existing; review |

## Phase 2 — Customer and job operations

Exit condition: a user can create the customer context, quote work, convert or create a Workorder, schedule it and complete operational activity using the Help Centre alone.

### Clients, sites and contacts

| Article | Priority | Status |
| --- | ---: | --- |
| Understand clients, sites and contacts | P0 | Existing overview |
| Add a client | P0 | Split from existing article |
| Add and validate a site | P0 | Split from existing article |
| Add client and site contacts | P0 | Mapping |
| Choose a billing contact | P0 | Mapping |
| Set customer payment terms | P0 | Mapping |
| Edit and archive customer records | P1 | Not started |
| Import customers safely | P1 | Not started |

### Quotes and Workorders

| Article | Priority | Status |
| --- | ---: | --- |
| Understand job types and statuses | P0 | Mapping |
| Create a Quote | P0 | Mapping |
| Add and price Quote lines | P0 | Mapping |
| Preview and send a Quote | P0 | Mapping |
| Record Quote acceptance or rejection | P0 | Mapping |
| Convert a Quote to a Workorder | P0 | Existing; review |
| Create a Workorder directly | P0 | Split from existing article |
| Understand the job card | P0 | Mapping |
| Change job status, type and priority | P0 | Mapping |
| Complete or cancel a Workorder | P0 | Mapping |
| Create work from a job template | P1 | Not started |

### Dispatch, tasks and field work

| Article | Priority | Status |
| --- | ---: | --- |
| Assign a job versus book staff | P0 | Existing; review |
| Create a booking | P0 | Split from existing article |
| Reschedule, reassign or cancel a booking | P0 | Mapping |
| Use the Dispatch Board | P0 | Mapping |
| Add and complete a task | P0 | Mapping |
| Add a reminder | P1 | Mapping |
| Use queues and queue stages | P0 | Mapping |
| Add notes and attachments | P0 | Mapping |
| Record job and travel time | P0 | Existing; review |
| Correct a time entry | P1 | Not started |
| Email or SMS from a job | P0 | Existing; review |
| Review activity and communication history | P1 | Not started |

## Phase 3 — Job-to-cash and Xero

Exit condition: an accounts user can turn completed work into a correct invoice, send it through the supported accounting workflow and reconcile payment without relying on undocumented assumptions.

### Invoices and payments

| Article | Priority | Status |
| --- | ---: | --- |
| Understand the invoice lifecycle | P0 | Existing; expand |
| Create an invoice from completed work | P0 | Mapping |
| Confirm customer and billing contact | P0 | Mapping |
| Check invoice lines, descriptions, tax and total | P0 | Mapping |
| Apply payment terms and due date | P0 | Mapping |
| Preview an invoice | P0 | Mapping |
| Approve and send an invoice | P0 | Existing; review |
| Understand invoice statuses | P0 | Mapping |
| Record a full or partial payment | P0 | Existing; review |
| Edit an invoice before sync | P0 | Not started |
| Correct an invoice after sync | P0 | Decision needed |
| Cancel, void or credit an invoice | P0 | Decision needed |
| Resolve a failed customer delivery | P1 | Not started |

### Tax, accounts and Xero

| Article | Priority | Status |
| --- | ---: | --- |
| Understand sales and purchase tax in Seama | P0 | Decision needed |
| Configure tax settings | P0 | Testing |
| Connect Seama to Xero | P0 | Testing |
| Map Seama accounts to Xero | P0 | Testing |
| Map Seama tax rates to Xero | P0 | Testing |
| Understand Seama and Xero states | P0 | Existing; review |
| Send an invoice to Xero | P0 | Existing; review |
| Verify an invoice in Xero | P0 | Testing |
| Resolve an invoice sync error safely | P0 | Testing |
| Disconnect or reconnect Xero | P1 | Decision needed |

## Phase 4 — Purchasing and inventory

Exit condition: a user can process a supplier bill once, allocate it correctly, manage stock by location and trace every resulting movement.

### Suppliers and bills

| Article | Priority | Status |
| --- | ---: | --- |
| Add and maintain a supplier | P0 | Mapping |
| Upload or email a supplier bill | P0 | Existing; review |
| Review and correct extracted bill data | P0 | Existing; expand |
| Map bill accounts and tax | P0 | Mapping |
| Allocate bill lines to inventory | P0 | Existing; review |
| Allocate bill lines to a job | P0 | Mapping |
| Mark a bill ready | P0 | Mapping |
| Send and verify a bill in Xero | P0 | Existing; review |
| Correct a bill after sync | P0 | Decision needed |
| Prevent duplicate imports and retries | P0 | Testing |

### Items, stock locations and composites

| Article | Priority | Status |
| --- | ---: | --- |
| Understand goods, services and composite items | P0 | Existing overview |
| Create an item | P0 | Mapping |
| Use one item across stock locations | P0 | Decision needed |
| Set opening stock by location | P0 | Testing |
| Understand stock quantities | P0 | Existing; review |
| Transfer stock | P0 | Existing; review |
| Adjust stock with a reason | P0 | Existing; review |
| Add or remove an item from a job | P0 | Testing |
| Understand stock commitment and consumption | P0 | Decision needed |
| Create a composite item | P0 | Testing |
| Add, remove and reverse composite components | P0 | Testing |
| Reconcile stock by location and history | P0 | Not started |
| Configure reorder points | P1 | Not started |
| Import item records | P1 | Not started |

## Phase 5 — Administration, reports and launch

Exit condition: administrators can control access and defaults, users can interpret reports, and the complete P0 Help Centre passes editorial and technical release gates.

### Administration

| Article | Priority | Status |
| --- | ---: | --- |
| Add a staff member | P0 | Existing; review |
| Create and assign a role | P0 | Existing; review |
| Understand the permissions matrix | P0 | Existing; expand |
| Configure job defaults and job types | P0 | Mapping |
| Configure queues | P1 | Mapping |
| Configure payment terms | P0 | Mapping |
| Configure markup | P1 | Mapping |
| Configure document templates | P0 | Mapping |
| Configure email and SMS templates | P1 | Existing partial |
| Manage profile and preferences | P1 | Not started |
| Manage company plan and billing | P1 | Not started |

### Reports and troubleshooting

| Article | Priority | Status |
| --- | ---: | --- |
| Understand report dates and filters | P0 | Not started |
| Review job and Quote performance | P1 | Not started |
| Review revenue, paid and outstanding | P0 | Not started |
| Reconcile inventory reports | P0 | Not started |
| Review integration exceptions | P0 | Capability review |
| Refresh and identify stale state | P0 | Existing partial |
| A button or action is missing | P0 | Mapping |
| A total or tax is unexpected | P0 | Decision needed |
| A Xero record did not sync | P0 | Testing |
| A stock quantity is unexpected | P0 | Testing |
| Contact Seama support effectively | P1 | Not started |

## Release gates

### Product gate

- All P0 workflows have a confirmed intended design.
- Any unresolved product decision is excluded from launch instructions or clearly constrained.
- No article describes a known defect as the normal workflow.

### Content gate

- Every P0 article is complete and reviewed.
- Terminology is consistent across articles.
- Cross-links cover both the next step and recovery path.
- Search keywords include common customer language.

### Visual gate

- Screenshots use synthetic records only.
- Desktop images are current, legible and consistently cropped.
- Mobile steps are included only where verified.
- Images have useful alternative text.

### Technical gate

Run from the repository:

```sh
mint validate
mint broken-links
mint a11y
mint dev --no-open
```

All checks must pass. Navigation and search must be tested in the preview.

### Approval gate

Each area needs approval from its nominated product owner:

- Customers and jobs
- Dispatch and field work
- Invoices, tax and Xero
- Suppliers and bills
- Inventory
- Administration and security
- Reports

## Maintenance after launch

- Revalidate an article whenever its interface or underlying rule changes.
- Review P0 content at least every three months.
- Set changed articles to **Revalidate** before editing.
- Keep product fixes and Help Centre content changes in separate pull requests.
- Update `lastVerified` only after reproducing the workflow.
- Archive instructions for removed features instead of leaving stale search results.

## Current definition of the end

**Launch end:** all P0 rows are **Published**, all release gates pass, and the full controlled workflow can be completed from company setup through customer payment and supplier accounting verification using only the Help Centre.

**Project end:** after launch, all agreed P1 articles are published and ownership has moved to the maintenance cycle. P2 remains an optional improvement backlog.
