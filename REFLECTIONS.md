# Retail-IQ: Project Wisdom & Reflections

<syn id="ARTIFACT-PATH-STRICT" date="2026-04-20" type="PREF">
OBJ: Prevent tool failures when creating documents.
CAUSE: Tried to set `IsArtifact: true` for a path in the project workspace.
RULE: Only use `IsArtifact: true` when the path is within the dedicated `.gemini/antigravity/brain/<id>/` directory. For project repository files, always set `IsArtifact: false`.
</syn>

<syn id="TECH-STACK-ALIGNMENT" date="2026-04-20" type="PREF">
OBJ: Keep `requirements.txt` in sync with `README.md`.
CAUSE: Project plan mentioned XGBoost and Flask, but they were missing from the environment config.
RULE: Proactively verify if planned tech stack components (from documentation) are reflected in `requirements.txt`.
</syn>
