# Downloadable supervisor demo

26 October 2026. This package contains a working local reference verifier built from `ExecCoDhe/Final-research` commit `0213390b304baab56dee73a0e43ade60374fa309`. The prepared changes are commit `447dc72` in the local implementation checkout. The connected GitHub integration cannot push to that repository or create a fork, so this separate branch of the already connected Research-Work repository hosts the download and integration patch. Neither repository's main branch is changed by this package branch.

- [Download the standalone demo ZIP](https://raw.githubusercontent.com/Shreya732-debug/Research-Work/codex/supervisor-demo-package/supervisor_demo/supervisor_demo_bundle.zip)
- [Read the walkthrough](WALKTHROUGH.md)
- [Download the patch for Final-research](https://raw.githubusercontent.com/Shreya732-debug/Research-Work/codex/supervisor-demo-package/supervisor_demo/Final-research-demo.patch)

## Run without Git

Extract the ZIP. Open its `code` folder and double-click `4_SUPERVISOR_DEMO.bat` on Windows. Python 3.11+ is required; no API key or third-party Python packages are needed. The browser opens a localhost interface. Keep the terminal open. Use the guided buttons to show the same SunPower claim under different disclosure policies and cutoff dates. The walkthrough includes other platforms and troubleshooting.

The prototype is deterministic and operates on prepared pilot evidence. It is not a newly trained model, a raw-document extractor or independently validated financial-verification accuracy. Eleven contract/regression checks and local HTTP S/C/U checks passed. The original automatic-dataset issues and bare/full experiment confound remain pending.

## Integrate into Final-research later

Someone with write access to `ExecCoDhe/Final-research` can apply the patch. This is optional for running the downloaded demo. In a clean local checkout of that repository, using Git:

```
git switch -c supervisor-verifier-demo
git am /path/to/Final-research-demo.patch
python -m unittest discover -s code/tests -v
git push -u origin supervisor-verifier-demo
```

Replace `/path/to/Final-research-demo.patch` with the downloaded file's actual path; quote it if it contains spaces. The patch is based on `0213390`. If it does not apply because the project changed, stop and provide the conflict details; do not overwrite newer work. The owner can then review and merge the branch through GitHub.
