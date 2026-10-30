# night-shift-agent-config

Configuration de l'agent des passes [night-shift](https://github.com/UnPoilTefal/night-shift) du homelab : refus ajoutés aux refus fixes du harness, et skills. Schéma et fonctionnement : [docs/agent-config.md](https://github.com/UnPoilTefal/night-shift/blob/v0.4.0/docs/agent-config.md).

- `select` lit la tête de la branche par défaut, donc la **dernière révision fusionnée**. Seuls `agent.yaml` et `skills/` atteignent l'agent.
- Aucune passe n'écrit ici : c'est une zone interdite. Un changement n'arrive à l'agent que par une PR fusionnée par un mainteneur.
- Dépôt **public** à dessein : sa garantie repose sur la protection de la branche par défaut (ruleset `protect-main`), payante sur un dépôt privé de compte personnel. Rien de secret n'y figure.

## Refus

| Refus | Pourquoi |
|---|---|
| `Bash(make release*)` | Une publication de release reste une décision humaine |
