# FusionAuth Engagement: Handover

Last updated: November 25, 2026. Paste this file (or its path) into a new chat to pick up where this one left off.

## Standing rules (apply to every reply and every draft)

1. **No em dashes, ever**, in chat or in any message, email or document drafted for Cam. Use commas, periods, colons or "to" instead.
2. **FusionAuth's internal reference PDFs are confidential.** They were shared only as a visual style reference. Never save them, or anything from them, to memory, and never reproduce their contents.
3. Cam's personal email address is private. Never send it to an outside service without asking first.

## Engagement snapshot

| | |
|---|---|
| Client | FusionAuth |
| Contact | Ben Hoehn, Sr. Director, Demand Gen |
| Provider | Camilo "Cam" Gonzalez, Automate305 (independent contractor, 1099) |
| Start | Monday, November 23, 2026 (live) |
| Commitment | 3 to 4 hours a day: calling, multi-channel outreach (email, phone, LinkedIn) and admin |
| Stack | A305 SEP (Outbox), A305 Dialer, GetLeads (sourcing), ColdIQ (scoring and signals) |
| Retainer | $3,500 per month, invoiced monthly or semi-monthly, Net 7 |
| Per qualified meeting | $300, billed on the invoice alongside the retainer |
| Billing address | ap@fusionauth.io, Ben CC'd |
| Termination | 30 days' written notice, either side |
| Confidentiality | Mutual: pricing, strategy and target account data stay confidential during and after |

**Qualified meeting** (what earns the $300): a decision-maker persona at an ICP-fit account, booked on a real trigger rather than a favor, and accepted and held. A reschedule within 14 days still counts. A confirmed no-show earns partial credit or a free re-book.

**Full proposal** (signature block, activity targets, what FusionAuth provides): private artifact at https://claude.ai/artifact/LPGXk4i2Rr4ZA1EP9zavtZ. It is kept out of this repo on purpose, because it includes FusionAuth's internal goals and is covered by the confidentiality clause. Open it with the Artifact tool's `read` action.

## Invoicing

### Status

| Invoice | Dated | Period | Meetings | Amount | Due | Status |
|---|---|---|---|---|---|---|
| A305-001 | Nov 23, 2026 | Nov 23 to Dec 22, 2026 | 0 | $3,500.00 | Dec 1, 2026 | Sent to ap@fusionauth.io with W-9 and direct deposit form, Ben CC'd |
| A305-002 | Dec 23, 2026 | Dec 23, 2026 to Jan 22, 2027 | held Nov 23 to Dec 22 | $3,500 + $300 per meeting | Dec 30, 2026 | Next up |

How billing works: the retainer is billed at the **start** of each period. Meetings are billed on the **following** invoice, for meetings held during the previous period. The W-9 and direct deposit form went out with A305-001 and do not need to be resent.

### Invoice generator (the tool to use)

**Link:** https://claude.ai/artifact/YXHEj7yHajg9worYpjqq4D (private to Cam; pin it in the claude.ai sidebar for quick access)
**Source backup:** `gtm-outbound/fusionauth/invoice-generator.html`

How to use it:

1. Open the link. The next invoice number, dates and meeting window fill in automatically from the last invoice in history.
2. Enter the number of qualified meetings held. The total and notes update on their own. Notes can be edited, one line per paragraph.
3. Click **Download PDF**. Once the download is accepted, the invoice is saved to history and the form moves on to the next number.

Behavior worth knowing:

- **Numbering comes from the history.** The next number is always the highest number in history plus one. Nothing is used up until a PDF download is accepted, so clicking around or cancelling never skips a number.
- **Reissuing a corrected invoice:** type the earlier number (for example A305-002) into the number field, fix the details and download. That replaces the record in history.
- **Re-downloading an old invoice:** each history row has a PDF button. It rebuilds that invoice exactly as recorded and changes nothing.
- **Data:** invoice records live in the artifact's database (`invoices` collection, one document per invoice number, e.g. `invoices/A305-001`). A new chat can read or fix them with the ArtifactData tool.
- **Running it locally is not recommended.** The artifact is already a hosted, private app with saved history, so there is nothing to deploy. A downloaded copy of the HTML opened in a browser can still make PDFs, but it has no history and does not track numbers.

Older files: `gtm-outbound/templates/invoice-template.html` is the static placeholder template from before the generator existed. The generator replaces it.

## Skills

- **fusionauth-getleads-list-builder** (account skill, call it with the Skill tool): builds an ICP-graded, phone-first prospect list for FusionAuth outbound from GetLeads, output in CloudTalk's contacts-template format. Use it whenever Cam asks to find, compile or grade FusionAuth prospects.
- `gtm-outbound/SKILL.md` in this repo is a different campaign (Automate305's own HVAC outbound in South Florida). Do not mix it up with FusionAuth work.

## Not covered here

Interview prep and the FusionAuth outbound sequence work are kept in another chat and on Cam's computer.
