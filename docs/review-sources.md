# E101–E160 primary-reference and material audit

Audit date: 2026-10-25. Status: pass for the factual reference models and citation-only material boundary. Runtime, numerical, mobile, localization, tag collection and public deployment checks are separate release gates.

The audit covers all 60 fixed plan IDs and slugs. The recommended reference set contains 67 unique official URLs. Fourteen calculators require a source replacement or addition listed in `source-proposals.json`. The integrator must apply those recommendations to the assembled catalog, generated tool metadata and per-app SOURCES before release.

## Scientific scope

All 60 formulas were compared with the stated primary-source model and reviewed with their dimensional conventions and approximations. Each record in `source-audit.json` includes the formula, review note, reference URL, observed transport status, web verification flag and material-reuse boundary.

Points requiring explicit conventions include the local Euclidean Einstein-lens distance model; the fluid Roche coefficient 2.44; Jeans mass defined using half the Jeans wavelength; static exterior Schwarzschild observers; finite nuclear mass in the hydrogen Rydberg coefficient; consistent atomic/nuclear mass bookkeeping; slow gyroscope precession; exact pitch-line belt geometry; hydraulic mean depth A/T; rapid initial Joukowsky pressure rise; clockwise-positive circulation; equivalent noise bandwidth; uniform ADC rounding error; dB power ratios; passive-load infinite VSWR; Hall polarity; insulated-tip fin efficiency; slab half-thickness; distinct-species ideal mixing; constant welding power; and the bend angle measured from flat.

## Repaired references

- E106: use the original University of Maryland point-mass lens lecture rather than relying on a specialized black-hole-ring article.
- E107: the MSU PDF URL returned an HTML interstitial. The MIT original teaching note states the opacity-based Eddington balance directly.
- E117: add the stable NIST complete table to support the atomic mass conversion. The bare `?u` endpoint works directly, but one web parser rewrites it as an invalid query.
- E121: add the MIT collision lecture that explicitly defines the coefficient of restitution.
- E124: follow the Purdue moved-content link to the official interactive Coriolis page.
- E131: use TxDOT’s exact Froude equation page instead of its broad chapter navigation.
- E132–E133: add the detailed original MIT surface-tension notes.
- E134: replace an unconfirmed PAP file with the official USBR F-3 cavitation-index definition.
- E135: use the reachable FHWA HEC-14 primary hydraulic-jump guide.
- E136: the AFT PDF returned HTTP 404. Use Joseph E. Shepherd’s Caltech lecture with the Joukowsky relation.
- E148: use the MIT coaxial TEM impedance problems instead of the generic distributed-model section.
- E151: the old fifth-edition PDF returned HTTP 404. The current author-hosted sixth-edition PDF is reachable.
- E154: replace the timed-out Kiel endpoint with Brian Cantwell’s original Stanford ideal-mixture chapter.

## Constants

The current official NIST table remains the 2022 CODATA release. Verified atomic mass constant: 1.66053906892×10⁻²⁷ kg. G, vacuum permittivity, vacuum permeability and atomic mass constant are measured values. h, c, e, kB and NA are exact SI defining constants. R and F follow exact products of defining constants and are rounded in binary64; hbar is computed as h/(2π). Standard gravity 9.80665 m/s² is conventional and must not be described as the local measured gravity.

E113 uses an explicitly labeled educational hydrogen coefficient 1.096776×10⁷ m⁻¹. This differs from the current infinite-nucleus Rydberg constant 10973731.568157 m⁻¹ and does not claim precision spectroscopy.

## Material and rights boundary

External textbooks, university notes, vendor documentation and government documents supply factual model references only. No external prose, diagrams, tables, datasets, code, font files or images are imported, republished or relicensed. The model-author modules contain original elementary JavaScript and no third-party imports. Application explanations, examples and graphics are independently authored. Final artifact-inventory verification remains with the integrator.

A source being available online is not treated as a commercial reuse license. `reuse_allowed: false` grants no right to copy its expression. Restricted noncommercial or no-derivatives material, including teaching sources with such terms, is excluded from the distributed app material. Source links and factual formulas do not transfer those source licenses to the original app code.

## Transport exceptions

Six recommended endpoints could not be fetched directly in the shell during the final pass: Harvard Faraday rotation (403), USBR cavitation F-3 (connection closed), three Analog Devices pages (DNS/timeout), and INL BISON verification (403). Their exact official pages or indexed official documents were independently verified through the web tool, including the relevant equations and scope. The audit retains the observed status instead of claiming HTTP 200. A temporary transport failure is distinct from the 404 references that were replaced.

The full source metadata is in `source-audit.json`; complete third-party content is not stored in the workspace by this audit.
