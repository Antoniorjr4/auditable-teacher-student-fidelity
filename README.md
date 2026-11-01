# Auditable Teacher–Student Fidelity

Commitment-Based Teacher-Student Fidelity Auditing with Public Randomness and Finite-Population Certification.

**Antonio Rufino · Independent Researcher, Brazil · [ORCID](https://orcid.org/0009-0004-1767-8165)**

This is the dedicated repository for the completed fidelity audit on **2,048 maintenance reports**. The prespecified sample of 768 reports contained 64 disagreements, giving a one-sided 95% exact hypergeometric upper bound of **9.765625%**, below the registered 10% target. The later census found **158/2,048 (7.71484375%)** disagreements.

- [Paper (PDF)](finite-population-audit/paper/manuscript_en.pdf)
- [Full package and reproduction instructions](finite-population-audit/README.md)
- [Release](https://github.com/Antoniorjr4/auditable-teacher-student-fidelity/releases/tag/audit-large-v1.0.0)
- [Offline verifier](finite-population-audit/verification/reproduce.py)
- [Licenses and third-party notices](finite-population-audit/LICENSES.md)

The certificate concerns a fixed finite disagreement table under the stated sampling and reference assumptions. No API key or model execution is needed for documentary replay.

## Reproduce

```bash
python -m pip install -r finite-population-audit/requirements-replay.txt
cd finite-population-audit
sha256sum --check SHA256SUMS
python verification/reproduce.py --output /tmp/audit-replay
```

## Relation to earlier work

The earlier [commitment-based knowledge-distillation project](https://github.com/Antoniorjr4/commitment-based-knowledge-distillation) addresses a related but distinct question. This study now has its own repository. Its initial publication there is preserved as part of the history; the raw evidence and registered results are unchanged. See [release notes](finite-population-audit/RELEASE_NOTES.md).

## Citation and archive

Use [CITATION.cff](CITATION.cff). The independent preprint and supplementary reproduction package are archived at **[10.5281/zenodo.23851318](https://doi.org/10.5281/zenodo.23851318)**. The earlier baseline DOI is not this study's DOI. See [PUBLICATION.md](PUBLICATION.md) for the archive history and exact file hashes.
