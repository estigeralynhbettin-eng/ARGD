# ARGD research materials

Research companion for **ARGD: Requirement-Linked Neighboring-Scenario Validation for Vulnerability Patches**, by Yi Lv and Cheng Wang.

Version 1.0.0 supplies the public companion to the R38 manuscript's Supplementary Materials S1 to S7. Each package records its sources, protocols and evidence boundaries.

The archived release has the persistent identifier [10.5281/zenodo.24048682](https://doi.org/10.5281/zenodo.24048682).

## Materials

| File | Contents |
| --- | --- |
| [ARGD_S1_catalog.zip](supplementary/ARGD_S1_catalog.zip) | Source-catalog metadata, checking questions and source-to-scenario mappings |
| [ARGD_S2_matrix.csv](supplementary/ARGD_S2_matrix.csv) | Four requirement-linked VUL4J-32 repair-coverage matrix rows |
| [ARGD_S3_execution.zip](supplementary/ARGD_S3_execution.zip) | Archived execution reports, native candidate revalidation, the single-XML control and test-input identities |
| [ARGD_S4_evaluator.zip](supplementary/ARGD_S4_evaluator.zip) | Preserved evaluator records, supplied test metrics and an offline audit program |
| [ARGD_S5_context.zip](supplementary/ARGD_S5_context.zip) | AntiSamy, Pillow, libtiff and source-screening observations and result summaries |
| [ARGD_S6_figure_data.zip](supplementary/ARGD_S6_figure_data.zip) | Figure data, plotting programs and editable diagrams |
| [ARGD_S7_reproduction_metadata.zip](supplementary/ARGD_S7_reproduction_metadata.zip) | Source identities, recorded commands, fixture signatures and reproduction metadata |

## Reading and checking the archive

Start with the README inside each package. For the matrix, inspect S2 together with the execution records in S3 and the fixture identities in S7. The earlier adapter and native validation protocols have separate recorded results.

To recompute the saved evaluator-record analysis, extract S4 and run the following command from its extracted directory with Python 3.10 or newer.

```text
python verify_evaluator.py --output evaluator_audit_output
```

To verify the retained legacy execution companion, extract the nested legacy ZIP in S3 and run the following command from its extracted directory.

```text
python verify_package.py
```

Both commands use the Python standard library to inspect archived records. The original vulnerability executions and model generations are documented by their retained evidence and source identities.

## Public-copy provenance

S1, S2 and S4 preserve the submission-file bytes. S3, S5, S6 and S7 contain public-copy transformations of historical machine-local path strings. Two internal review documents are omitted from S3. The published numerical results, testcase outcomes, matrix assertions and Java/fixture sources have been checked against the submission copies.

[PUBLICATION_PROVENANCE.md](PUBLICATION_PROVENANCE.md) explains the transformations. [PUBLICATION_CHANGES.csv](PUBLICATION_CHANGES.csv) identifies affected members and their hashes. [SUPPLEMENTARY_SHA256.csv](SUPPLEMENTARY_SHA256.csv) provides the submission and public package identities.

## License and attribution

The author-created S2 matrix and the new repository documentation use CC BY 4.0. Other archived materials retain their applicable terms, as detailed in [LICENSE.md](LICENSE.md) and the notices supplied with each package. Source catalog entries link to their original third-party sources. S3 and S4 retain the applicable Apache and MIT license and attribution files.

## Citation

Use [CITATION.cff](CITATION.cff) for this repository's author, version and DOI metadata. The archived v1.0.0 record corresponds to the GitHub v1.0.0 tag.

## Funding

This work was supported by the Discipline Breakthrough Pioneer Program of the Ministry of Education of China, Grant No. JYB2025XDXM122.
