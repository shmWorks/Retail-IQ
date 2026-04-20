# 🧠 Retail-IQ Core Wisdom (Compacted)

<syn id="ARTIFACT-ERR" date="2026-04-20" type="FIX">
OBJ: Document creation safety.
CAUSE: `IsArtifact:true` on project paths fails.
RULE: Use `IsArtifact:true` ONLY for internal brain/knowledge paths. Project files = `IsArtifact:false`.
</syn>

<syn id="DEP-SYNC" date="2026-04-20" type="ARCH">
OBJ: Env consistency.
CAUSE: Plan vs. requirements drift.
RULE: Sync `requirements.txt` & `pyproject.toml` with `README` tech-stack before execution.
</syn>

<syn id="MODULAR-ML" date="2026-04-20" type="ARCH">
OBJ: Reduce agent cognitive load.
CAUSE: Large notebooks cause context poisoning.
RULE: Decouple logic from `.ipynb` to `src/retail_iq/`. Use notebooks only as clean drivers.
</syn>

<syn id="API-SHORTCUT" date="2026-04-20" type="OPT">
OBJ: 100x turn acceleration.
CAUSE: `view_file` is expensive.
RULE: Maintain `[API_MANIFEST]` in `docs/project_summary.md`. Use signatures there to code without reading source.
</syn>

<syn id="PATH-CENTRAL" date="2026-04-20" type="ARCH">
OBJ: Cross-platform robustness.
CAUSE: Relative paths break during restructuring.
RULE: ALWAYS use `config.py` constants (`RAW_DATA_DIR`, etc.) for I/O.
</syn>

<syn id="REPO-CLEAN" date="2026-04-20" type="HYG">
OBJ: Prevent repo bloat.
CAUSE: Tracking datasets/plots creates merge conflicts & history size issues.
RULE: `git rm --cached` large data/outputs. Add `data/`, `outputs/`, `.venv/` to `.gitignore`.
</syn>
