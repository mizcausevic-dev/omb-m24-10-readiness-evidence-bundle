# omb-m24-10-readiness-evidence-bundle

> **Historical draft, not current federal AI readiness guidance (reviewed 2026-10-30).** [OMB M-25-21](https://www.whitehouse.gov/wp-content/uploads/2025/02/M-25-21-Accelerating-Federal-Use-of-AI-through-Innovation-Governance-and-Public-Trust.pdf) expressly rescinded and replaced M-24-10, and [OMB M-25-22](https://www.whitehouse.gov/wp-content/uploads/2025/02/M-25-22-Driving-Efficient-Acquisition-of-Artificial-Intelligence-in-Government.pdf) expressly rescinded and replaced M-24-18 on April 3, 2025. This repository preserves a 2024-memorandum profile for historical comparison. Its `profile.json`, examples, cadence values, and referral language have **not** been remapped to the replacement memoranda. Do not use it to assert current federal readiness, required reporting, or conformance. Check the [OMB memoranda index](https://www.whitehouse.gov/omb/information-resources/guidance/memoranda/) for later changes.

> **OMB M-24-10 Readiness Evidence Bundle v0.1 draft.** Profile of the [Evidence Bundle spec](https://github.com/mizcausevic-dev/evidence-bundle-spec) scoped to evidence a federal agency's program toward **OMB M-24-10** (March 2024) "Advancing Governance, Innovation, and Risk Management for Agency Use of Artificial Intelligence", plus the AI Bill of Rights blueprint, Section 508 + WCAG 2.1 AA, Privacy Act of 1974 + FOIA, NIST AI RMF 1.0 + GenAI Profile, OMB M-24-18 (AI procurement), and residual obligations carried forward from EO 14110 + state-government-AI statutes. Names 8 obligation families covering agency AI governance, the Federal AI Use Case Inventory, rights-impacting minimum practices, safety-impacting minimum practices, AI procurement, Section 508 accessibility, Privacy Act + FOIA, and NIST AI RMF application.

Part of the [Kinetic Gain Protocol Suite](https://suite.kineticgain.com).

> Status: v0.1 draft. Profile at [`profile.json`](./profile.json), canonical example at [`examples/prfsa-omb-2026q4/`](./examples/prfsa-omb-2026q4/).

## Obligation families (8)

| Code | Citation | Required evidence kinds |
| --- | --- | --- |
| **ai-governance** | OMB M-24-10 §2 | agency-ai-policy-officer-designation · agency-ai-strategy-document · agency-ai-governance-committee-charter · agency-ai-risk-register |
| **federal-ai-use-case-inventory** | OMB M-24-10 §3(a) | federal-ai-use-case-inventory-snapshot · per-use-case-entry-with-tool-card-link · annual-inventory-update-attestation |
| **rights-impacting-ai-minimum-practices** | OMB M-24-10 §5(d) | rights-impacting-pre-deployment-impact-assessment · rights-impacting-ongoing-monitoring-report · rights-impacting-human-review-pathway-documentation · rights-impacting-consumer-notice-template · rights-impacting-opt-out-pathway-documentation |
| **safety-impacting-ai-minimum-practices** | OMB M-24-10 §5(c) | safety-impacting-pre-deployment-safety-evaluation · safety-impacting-real-world-testing-report · safety-impacting-ongoing-safety-monitoring-report · safety-impacting-safety-officer-designation |
| **ai-procurement-omb-m24-18** | OMB M-24-18 | ai-procurement-contract-clause-template · vendor-ai-disclosure-requirement · far-ai-reference-attestation |
| **accessibility-section-508** | Section 508 + 36 CFR Part 1194 + WCAG 2.1 AA | section-508-conformance-attestation · wcag-2-1-aa-audit-report · ai-output-accessibility-test-evidence |
| **privacy-act-foia** | Privacy Act 5 USC §552a + FOIA 5 USC §552 | privacy-act-system-of-records-notice-for-ai-system · privacy-act-accounting-of-disclosures-extract · foia-processing-impact-assessment |
| **nist-ai-rmf** | NIST AI 100-1 + GenAI Profile (2024) | nist-ai-rmf-govern-function-attestation · nist-ai-rmf-map-function-output · nist-ai-rmf-measure-function-output · nist-ai-rmf-manage-function-output · nist-genai-profile-application-attestation |

## Historical profile cadence examples

| Family | Window |
| --- | --- |
| agency_strategy | P365D |
| inventory_update | P365D (annual minimum per M-24-10) |
| rights_impacting_monitoring | P90D |
| safety_impacting_monitoring | P30D (highest cadence — safety is critical) |
| wcag_audit | P365D |
| nist_rmf_iteration | P180D |

## Historical synthetic example

[`examples/prfsa-omb-2026q4/`](./examples/prfsa-omb-2026q4/) — Pacific Region Federal Services Agency 2026 Q4 OMB M-24-10 readiness bundle covering two in-scope AI systems (VendorG GovDecide v3.x + PRFSA internal chatbot v2.1), 12 evidence items across the eight families.

## Composes with

| Repo | Role |
| --- | --- |
| [`evidence-bundle-spec`](https://github.com/mizcausevic-dev/evidence-bundle-spec) | Base spec |
| [`government-decision-record-audit-stream`](https://github.com/mizcausevic-dev/government-decision-record-audit-stream) | Audit-stream extracts feed ai-governance + nist-ai-rmf families |
| [`state-government-ai-disclosure-tracker`](https://github.com/mizcausevic-dev/state-government-ai-disclosure-tracker) | Identifies which federal + state overlays apply |
| Sibling readiness bundles (hipaa / ferpa / respa / naic / eeoc / cfpb) across the 6 prior verticals | Same architecture, different per-vertical regulatory anchors |

## Historical posture

This draft shows how the 2024 OMB M-24-10 and M-24-18 text was mapped into evidence-bundle fields. It does not support a present-day federal AI readiness or compliance claim. A replacement profile requires a field-by-field review against M-25-21 and M-25-22 and verification of other applicable sources. The Federal AI Use Case Inventory listing is a separate agency publication process. Per the standing public-language guardrail: *readiness · evidence · posture · controls · scaffolding* — never "OMB-M-24-10-compliant" or "AI-Bill-of-Rights-attested" without an external attestation.

## License

MIT — see [`LICENSE`](./LICENSE).
