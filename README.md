# DYEP
DoYouEvenPushBro?

## GitHub en Slack Notificatie Systeem

Dit systeem controleert of gebruikers hun werk hebben gepusht naar GitHub en stuurt notificaties via Slack op specifieke tijdstippen.

## Setup

### Vereisten

- Python 3.8 of hoger.
- Een GitHub token met de juiste toegangsrechten.
- Een Slack token met de juiste toegangsrechten.

### Configuratie

1. Clone de repository.
2. Configureer de geheimen (`GITHUB_TOKEN`, `SLACK_TOKEN`) in de GitHub repository settings onder 'Settings > Secrets'.
3. Pas de gebruikersnaam in de workflow YAML en/of het Python script aan naar de gewenste GitHub gebruikersnaam.

### Gebruik

De workflow wordt automatisch uitgevoerd op de geconfigureerde tijdstippen (standaard om 12:00 en 16:00 UTC). Je kunt het script ook lokaal draaien met de volgende commando's:

```bash
python script.py check_push_noon
python script.py check_push_any
python script.py get_activity
```
