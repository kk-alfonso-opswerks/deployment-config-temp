# Deployment Configuration (GitOps)

This repository contains declarative Kubernetes manifests reconciled by Flux CD.

## Automated Handoff Contract
- **Edited by:** Jenkins CI bot
- **Target File:** `apps/production/deployment.yaml`
- **Target Field:** `spec.template.spec.containers[name=flaskapp].image`
- **Tag Format:** `v1.<build_number>.<short_sha>`
