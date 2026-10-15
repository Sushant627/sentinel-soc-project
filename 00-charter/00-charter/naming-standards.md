# Naming Standards

## Azure resources
Pattern: <type>-<org>-<workload>-<env>-<region>-<instance>
Org = hp, workload = sec (security operations), env = prod, region = eus, instance = 001

| Resource | Prefix | Example |
|---|---|---|
| Resource group | rg | rg-hp-sec-prod-eus-001 |
| Log Analytics workspace | log | log-hp-sec-prod-eus-001 |
| Data collection rule | dcr | dcr-hp-winsecurity-prod-eus-001 |
| Logic App (playbook) | logic | logic-hp-enrich-ip-prod-eus-001 |

Prefixes follow Microsoft's Cloud Adoption Framework abbreviations.

## Sentinel content
| Item | Pattern | Example |
|---|---|---|
| Analytics rule | DET<ID>-<Tactic>-<Description>-v<N> | DET001-CredAccess-MultipleFailedSignIns-v1 |
| Watchlist | wl-<purpose> | wl-vip-users |
| Workbook | WB-<Audience>-<Topic> | WB-SOC-Overview |
| Hunting query | HUNT<ID>-<Hypothesis> | HUNT001-MailboxForwardingRules |

## Rules
- The detection ID is also the file name in the repo (detections/DET001-...md), so the rule and its documentation always match.
- Increase the version number (v1, v2) whenever a rule's logic changes, and record why in the file.
- Tag every resource with owner, env, and project.
- Lowercase for Azure resources; no spaces anywhere.
