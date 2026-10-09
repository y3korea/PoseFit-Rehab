# PoseFit Rehab reproducibility release

This folder is a GitHub-ready release package for the manuscript *Functional Verification of a Local-First Browser Prototype for Markerless Home Knee Exercise Monitoring*.

## Scope

The static browser demo and synthetic functional tests are research/educational artifacts. They are not a medical device, do not diagnose or prescribe treatment, and have not been clinically validated. The repository must not be presented as evidence of clinical accuracy, safety, usability, or effectiveness.

## Contents

- `prototype/index.html`: static prototype reviewed by the manuscript, including a one-line correction so a reported visibility value of zero is handled as low quality
- `PoseFit-Rehab-v0.1.1.zip`: complete version-fixed source archive containing `prototype/`, `reproducibility/`, the deterministic test harness, and release metadata
- `SOURCE_MANIFEST_SHA256.txt`: file hashes for the prototype snapshot inside the version-fixed archive

## Reproduce the functional checks

```bash
unzip PoseFit-Rehab-v0.1.1.zip
cd PoseFit-Rehab-public-v0.1.1/reproducibility
python3 run_functional_verification.py
```

Expected result: `11/11 deterministic functional checks passed`.

## Release record

- Public repository: https://github.com/y3korea/PoseFit-Rehab
- Initial release version: `v0.1.1`
- Archive DOI: pending Zenodo archival after the GitHub release is published.
- License: no open-source license has been selected. Public access does not grant reuse rights; see `LICENSE_TO_SELECT.md`.

Do not commit secrets, personal recordings, participant data, API keys, or credentials.
