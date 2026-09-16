# Naming Who Tests for Bias, at Which Level

*Companion to "Screened Out, Together"*

## Worked example

**System:** Third-party applicant-screening tool Inês Duarte adopted once hiring passed twenty people, used to rank candidates before she reviews them herself
**Vendor-level testing (aggregate, across the vendor's full customer base):** Unknown. Inês asked; the vendor pointed to a generic marketing page claiming "bias-audited AI" with no methodology, no date, and no offer to share actual results
**Deployer-level testing (Ondas's own specific configuration and applicant pool):** None yet, run for the first time as part of this exercise, on the last twelve months of Ondas's own hiring outcomes, twenty-two hires reviewed
**Named owner, vendor-level:** Unresolved, see "when the vendor won't agree" below
**Named owner, deployer-level:** Inês Duarte
**Gap identified:** Ondas has no aggregate-level visibility at all, and, being a twenty-four person company, no realistic way to get it. The deployer-level check at least confirms nothing alarming showed up in Ondas's own small sample, which is honest but not the same as knowing the tool is fair

Two tests were supposed to run here. Only one did, and the record says so plainly rather than pretending otherwise. That honesty, not a clean pair of green checkmarks, is the actual deliverable of this chapter.

## Building the allocation

**System and vendor**
Named specifically, including which underlying model or product line it uses, since a vendor may have acquired or rebranded components with different histories.

**Vendor-level testing commitment**
What the vendor has contractually agreed to test, at what cadence, and whether results are actually shared or just asserted. "The vendor tests for bias" without a contractual commitment and a delivery cadence is not evidence, it's a marketing claim.

**Deployer-level testing commitment**
What your organisation tests, using your own actual outcomes data, not the vendor's aggregate figures, which cannot see your specific applicant pool or job criteria.

**Named owner, each level**
One person per level who is accountable for the test actually happening on schedule, not just for reviewing results if someone remembers to run them.

**Gap identified**
An explicit statement of what neither level's testing covers. If this field is blank, the allocation hasn't been thought through, it's been assumed complete.

## Who fills this in, and when

Negotiated between the organisation's HR/legal function and the vendor before signing or renewing any contract for a high-risk employment AI system, not discovered for the first time during litigation discovery. Reviewed whenever the vendor changes the underlying model, acquires a component (as happened in the Workday case with an acquired product later folded into the same collective action), or your organisation's applicant pool changes materially.

The failure mode specific to this chapter: treating a vendor's marketing claim of "bias-tested" as equivalent to a contractual, cadenced, aggregate-level testing commitment with results your organisation can actually see. The two are not the same, and a five-year gap between what was tested and what actually happened is not a compliance record. It's the thing a plaintiff's discovery request goes looking for first.

## When the vendor won't agree

A ten-person company has essentially no leverage to extract a bespoke testing commitment from a vendor the size of Workday, and it would be dishonest to present this chapter as though negotiating one is realistic for most readers. Where that's the case, the deliverable changes but doesn't disappear: put the request in writing, keep the vendor's response, whether that's a refusal, silence, or a pointer to a generic public disclosure that doesn't actually answer the question asked. That correspondence is worth less than a real contractual commitment, but it's worth considerably more than nothing, it establishes that your organisation identified the gap and asked, rather than never having thought to. In litigation, the difference between those two positions is not small.
