# PopAds Automation (bootstrap)
- Python 3.11, venv local
- Entrée: `config/campaigns.yaml`
- Modules à implémenter ensuite:
  - `config_loader`: lecture + validation YAML, fusion defaults/campagne
  - `popads_api`: create/pause/resume/stats via API PopAds
  - `firestore_repo`: persistance états (running/paused/error)
  - `monitor_campaigns` (CF Gen2): check quotas toutes les 2 min
  - `resume_campaigns` (CF Gen2): relance quotidienne 00:05 Europe/Paris
