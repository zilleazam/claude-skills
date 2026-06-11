# claude-skills

Claude Code skills library — synced from the Cyfen Elastic observability VM.

## Structure

```
user/         ← Custom SOC/Elastic/n8n skills
  alert-triage/
  apm-health-summary/
  apm-service-dependencies/
  attack-discovery-triage/
  case-management/
  detection-rule-management/
  generate-sample-data/
  k8s-blast-radius/
  manage-alerts/
  ml-anomalies/
  n8n-code-javascript/
  n8n-code-python/
  n8n-expression-syntax/
  n8n-mcp-tools-expert/
  n8n-node-configuration/
  n8n-validation-expert/
  n8n-workflow-patterns/
  observe/

public/       ← General purpose skills
  docx/
  file-reading/
  frontend-design/
  pdf/
  pdf-reading/
  pptx/
  product-self-knowledge/
  xlsx/
```

## Install on a new machine

```bash
git clone https://github.com/zilleazam/claude-skills.git

# Linux/VM (global)
mkdir -p ~/.claude/skills
cp -r claude-skills/user ~/.claude/skills/
cp -r claude-skills/public ~/.claude/skills/

# Windows (global, run in PowerShell)
mkdir "$env:USERPROFILE\.claude\skills" -Force
xcopy /E /I claude-skills\user "$env:USERPROFILE\.claude\skills\user"
xcopy /E /I claude-skills\public "$env:USERPROFILE\.claude\skills\public"
```

## Sync updates

```bash
cd claude-skills && git pull
# then re-copy to ~/.claude/skills/
```

