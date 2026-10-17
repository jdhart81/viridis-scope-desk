# Evidence and decision rules for Scope Desk

Use this reference for both skills. It adapts the literal citation format used
by Delivery Desk 0.1.4; it does not require that plugin to be installed.

## Source register and literal evidence

Assign S1, S2, etc. to selected source texts; retain supplied source IDs when
present. Record title, supplied date/revision, source-stated/owner-supplied
status and reviewed scope. An unread link is a gap, not evidence. For embedded
JSON text, count its decoded text lines starting at 1. Register the original
raw bundle as B1 for bundle-level fields and count its actual physical lines.
Do not pretty-print the bundle and cite those new line numbers. State the line
spaces used. If raw text is unavailable, mark citations unverified; never guess
line numbers or invent a quote that describes an absent fact.

Provenance fields are claims too. Retain the supplied filename/title and full
revision/hash, record type, issuer and date/version where supplied; otherwise
mark unknown. Each supplied metadata value needs an E entry containing that
value, cited beside the register field/row. For JSON metadata use the original
B1 field line; for metadata within an embedded document use its original S
header/date line. A decoded requirements paragraph does not establish its
document's filename, issuer, date or hash. Do not abbreviate supplied hashes.
An attachment name observed in the host may be labeled as that observation;
do not manufacture a source line containing it.

Complete the literal evidence index first, then compose source-based assertions
only from those entries. Keep positive source facts and explicit absences
distinct. Check value, subject, qualification and context, not just topical
similarity. Register entries, introductory prose and copyable handoffs must
carry the matching E IDs too. Optional details unsupported by the index are
omitted/unknown, not supported by an absence entry. A source's price/buyer
hypothesis still needs positive evidence for its actual wording or amount.

For each selected complete original source line, create one evidence entry:

E1 — S1 L3
Supports: one concise factual claim.
~~~
<one complete original source line, with indentation stripped>
~~~

Each entry has one source ID, one 1-based line number and one plain-text block.
Use a tilde fence of at least three characters, longer than every tilde run in
the source line, with no language label. Never put quotes in tables or inline
code. Preserve literal backticks, bold markers, links, pipes, backslashes,
punctuation and case; do not add escapes, entities, ellipses or joined snippets.
Extract `source_lines[line_number - 1].strip()` when file/code access is
available. Check the displayed block text against that exact line. All later
source-based claims cite E IDs, without adding new quotes. Proposed choices
and current conversation observations are labeled separately, not given
manufactured source quotes.

Exact text alone is insufficient: verify that the quote supports the claim
in context. A physical line may begin or end mid-sentence. If a negation,
condition, quantity, attribution or limit is on an adjacent line, create a
separate literal E entry for each necessary adjacent line and cite those
entries together. Do not isolate a continuation that drops `No`, `not`,
`only`, `unless`, or another qualification and changes the apparent meaning.
Keep each block one complete original line; sufficient context may require
several blocks. Never repair the quote by joining or rewriting source lines.

For missing facts explicitly listed in a bundle, cite each relevant original
item under B1. If absent from the reviewed records, say `not supplied within
the reviewed scope`, naming that scope. A null, blank or absent value is
unknown; explicit zero is known. An old record of an unrun test does not prove
the test remains unrun today. Keep dated record claims, current observations
and unknown current state separate.

Before returning, reconcile the explicit missing_facts array with the evidence
list and gap section one item at a time: every item retained, every original
physical line quoted, every gap linked to its E ID. Likewise, for each factual
deliverable/criterion attribute, confirm that the cited entries contain that
attribute and its necessary sentence context. If it is a proposed choice,
label it proposed instead of attaching an incomplete factual citation.

## Exact baseline and acceptance

For any scope or acceptance claim, identify subject, exact revision,
environment, approver role and action. A source can report acceptance without
independent authentication. Acceptance of a quote, payment terms, permission
to test and acceptance of a delivered revision are different events. Acceptance
of one revision never automatically covers later changes. Preserve unresolved
conflicts; do not choose the newest file without an explicit superseding or
selected-baseline designation. A proposed reviewer or deadline is not an
approved owner or schedule.

Tests, local package checks, tool discovery, synthetic examples and internal
payments are not client delivery, adoption, verified sales or profit. A scoped
source-stated test result cannot qualify a different revision/environment.
This skill prepares review drafts only. It cannot promise market outcomes,
approve pricing, interpret legal enforceability or create customer agreement.

## Change categories

- **Addition:** requested behavior/output exceeds or changes an explicit
  baseline requirement/boundary. State exactly which baseline item changes.
- **Clarification:** resolves wording without an evidenced change to behavior,
  output, quantity, authority, acceptance or effort. If unchanged impact cannot
  be established, classify unknown rather than quietly call it clarification.
- **Correction:** requested implementation/output would meet an explicit
  existing criterion it currently fails in supplied evidence. Require both
  the original criterion and the evidenced deviation; a complaint alone does
  not prove a defect, fault or who should pay.
- **Unknown:** baseline revision, current behavior, request meaning or authority
  is insufficient/conflicting. Name the exact missing input and offer a
  provisional comparison; do not infer an agreed billable change.

Split mixed requests into separate items. Record category and pricing treatment
separately. None of these categories decides blame, contractual responsibility,
billability, price or acceptance.
