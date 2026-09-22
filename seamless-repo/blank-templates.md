# Blank Templates

One per chapter, fields only, no worked example, no prose. Copy the one you need. See the matching chapter in Part Two for what each field means and how it tends to go wrong.

---

## Ch.1 — Decommission Record
- System name / inventory ID:
- Decommission trigger (dated):
- Data disposition (kept / deleted / migrated), confirmed by:
- Downstream dependents notified (name + date, each):
- Inventory removal confirmed (date):
- Open retention conflicts (owner + target date, or "none"):

## Ch.2 — Human Participation Tier
- System:
- Tier(s) assigned (1 Evaluative / 2 Bounded / 3 Procedural / 4 None / 5 Shared-ambiguous):
- Note (why each tier applies, what's real vs. formal):

## Ch.3 — Reviewer Competence Record
- System and use:
- Named reviewer(s):
- Known failure mode (specific, not "AI can be wrong"):
- Evidence reviewer was shown this failure mode (dated):
- Last caught incident (date, or "none yet"):

## Ch.4 — AUP Tier
- Tool:
- Tier (Approved / Conditional / Prohibited):
- Data permitted:
- Evidence of actual training (dated, not a click):
- Last reviewed (tied to a ToS/data-handling change):
- Escalation contact:

## Ch.5 — Draws Strongly Test
- System:
- Downstream party:
- Draws strongly test (real sample, real percentage):
- Conclusion (does the SCHUFA logic apply):
- Named owner of providing an explanation on request:
- Explanation actually available (yes / partial / no):

## Ch.6 — Merged Clock Table (one row per incident type)
- Incident type:
- Regimes that apply (tick: AI Act / NIS2 / GDPR / DORA / sector-specific / contractual):
- Shortest applicable deadline:
- First-alert role:

## Ch.7 — Authority Ladder
Pre-authorised actions (one row each):
- Action (specific, bounded):
- Trigger:
- Pre-authorised by (name + date):
- Execution authority:

Escalation triggers (answer each for your own context):
- Critical business function down — threshold:
- Critical customer impact — threshold:
- Existential threat — threshold:
- Personal data breach — which clock applies, named starter:
- Other regulatory breach — which regimes:

## Ch.8 — Seam Inventory
- Seam description:
- Direction (agent-to-agent / agent-to-tool):
- Last reviewed:
- Named contact:
- Backup contact:
- Trust basis (the real reason, not the comfortable one):

## Ch.9 — Label Chain of Custody (one row per hop)
- Hop:
- Label survives by default? (yes / no / untested):
- Responsible:
- Last tested:

## Ch.10 — Bias Testing Allocation
- System:
- Vendor-level testing commitment (contractual, cadenced):
- Deployer-level testing commitment (your own data):
- Named owner, vendor-level:
- Named owner, deployer-level:
- Gap identified (what neither level covers):

## Ch.11 — Provider Status Check
- Change:
- Own branding applied? (Y/N):
- Substantial modification? (Y/N):
- New intended purpose? (Y/N):
- Resulting classification:
- Decision made by (name + date):

## Ch.12 — Vendor Continuity Register
- Vendor / product:
- Export/portability tested (date, result):
- Estimated full migration time if discontinued:
- Named migration-trigger owner:
- Trigger condition (tied to announcement, not shutdown date):

## Ch.13 — Insurance Coverage Check
- Policy:
- AI-specific exclusion present (Y/N, form number if known):
- What this excludes (plain language):
- Alternative coverage in place (Y/N):
- Named owner of closing the gap:
- Last checked:

## Ch.14 — Ghost-Finding Run
- Run date:
- Method used (OAuth/SSO review / extension audit / expense scan / DNS-egress check):
- Finding:
- Action taken:

## Ch.15 — Switch Map
- Control being disabled:
- Intended effect:
- Other things bundled with this flag (discovered on inspection):
- Verified still active before the run (Y/N):
- Action taken:

## Ch.16 — Shared Resource Audit
- Shared resource:
- Why it's shared:
- Could it carry an unintended signal (Y/N/untested):
- Isolation assumed or verified:
- Action taken:

## Ch.17 — System Synthesis
- System:
- Status pulled from Ch.1 through Ch.16 (one line each, "not applicable" or "not started" where true):
- Could you explain what happened here if someone asked tomorrow? (yes / partial, with what's still open / no):
