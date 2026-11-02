# T-Decomp: Experimental Data and Reproducibility Records

Supporting experimental output records and available code snapshots for **T-Decomp: Time-Aware State Decoupling for Mixed-Precision Quantization of Recurrent Language Models**.

## Download
Download `TDecomp_Experimental_Records.zip` from this repository and extract it. The archive contains its own README, data dictionary, file manifest with SHA-256 hashes, validation script and validation report.

## Included evidence
- Five complete downstream tasks, four configurations each (82,324 question evaluations).
- Complete 1K–16K retrieval grid: 100 cells, 10,000 model-case evaluations.
- Native recurrent-controller and loaded-7.2B experiments with per-token losses.
- Natural-document trajectories, matched routing seeds, Mamba and cross-corpus controls.
- Physical packed-state quality, storage accounting, and complete-model timing records.
- Completed official Quamba W4A16 comparison and diagnostic records.
- Summary tables, plotting inputs, and available execution/code snapshots.

## Verification
After extraction, run `python3 validate_records.py`. The supplied report records 305 successful checks, including task item counts and correctness, retrieval successes, packed quality PPL, and timing medians.

## Scope and access
Historical table cells, including Smooth operating points, are source-reported and separated from newly executed raw records. Missing historical execution logs are not claimed to have been recovered. The available code snapshots are not a turnkey model environment. Model weights, raw third-party corpora, authentication helpers and confidential project identifiers are not included. Machine-specific paths are generalized. Obtain external models/datasets under their original terms and replace redacted paths before rerunning inference.

No DOI or new software license is asserted. Third-party code remains subject to its original rights and licensing. Nominal payload bits, total persistent buffers and full-model latency are distinct metrics; the packed prototype does not establish a speedup or total-storage advantage over the plain FP16-state reference.
