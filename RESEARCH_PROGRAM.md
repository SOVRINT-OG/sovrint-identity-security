# Research Program: Identity Security

**Status:** Proposed agenda for a documented security-framework draft. This document does not claim standards compliance, production deployment, or independent security validation. See [RESEARCH_STATUS.yaml](./RESEARCH_STATUS.yaml).

## Scope

The README identifies public framework topics including identity assurance, consent, delegation, revocation, recovery, and audit. Research will keep identity claims, proofing, authentication, authorization, and credential exchange distinct. Public diagrams and synthetic examples must not expose credentials, personal records, private topology, or operational secrets.

## Questions

1. Which actors, claims, credentials, and trust relationships are represented in each proposed flow?
2. What threats apply to issuance, presentation, verification, delegation, recovery, and revocation?
3. Which data are strictly necessary for a stated operation, and what retention or deletion conditions apply?
4. How are issuer, holder, and verifier responsibilities represented without implying that a credential proves more than its defined claims?
5. Which assertions can be checked with synthetic test cases, and which require independent security review?

## Planned work

- Create a public threat-model template naming assets, trust boundaries, attacker capabilities, mitigations, assumptions, and residual risks.
- Map public flows to relevant NIST SP 800-63-4 sections only where scope matches; record differences and avoid unsupported compliance labels.
- If credential examples are added, use synthetic identities and identify issuer, holder, verifier, claims, and verification assumptions.
- Test validation and revocation edge cases with synthetic fixtures; retain test results, versions, and limits.
- Keep a separate review record for privacy, accessibility, consent, and recovery risks.

## Security and evidence boundaries

Do not publish real identity data, credentials, secrets, access tokens, private keys, exploitable operational details, or private system topology. A specification crosswalk is not certification. Automated tests cover only their fixtures and assertions; they do not establish that a deployed system is secure.

## References

- Temoshok, D. et al. (2025). [NIST SP 800-63-4, Digital Identity Guidelines](https://doi.org/10.6028/NIST.SP.800-63-4). NIST guidance on identity proofing, authentication, and federation; use only for matching scope.
- W3C, [Verifiable Credentials Data Model v2.0](https://www.w3.org/TR/2025/REC-vc-data-model-2.0-20250515/) (W3C Recommendation, 15 May 2025). Defines a data model and issuer-holder-verifier ecosystem; it does not establish the security of a SOVRINT implementation.
- [Repository README](./README.md) for the framework's stated scope and protected-material boundaries.
