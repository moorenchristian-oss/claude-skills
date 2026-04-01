# Claude Code — Skills disponibles

Liste des skills intégrés dans Claude Code avec leur description.

| Skill | Description |
|---|---|
| `update-config` | Configurer les comportements automatiques via `settings.json` (hooks) |
| `keybindings-help` | Personnaliser les raccourcis clavier (`~/.claude/keybindings.json`) |
| `simplify` | Réviser du code modifié pour la qualité, la réutilisabilité et l'efficacité |
| `loop` | Exécuter une commande à intervalle régulier (ex: `/loop 5m /foo`, défaut 10m) |
| `schedule` | Créer des agents distants planifiés (cron) et gérer les triggers automatisés |
| `claude-api` | Construire des applications avec l'API Claude / Anthropic SDK |
| `design-md` | Analyser des projets Stitch et synthétiser un design system dans `DESIGN.md` |
| `enhance-prompt` | Transformer des idées UI vagues en prompts précis et optimisés pour Stitch |
| `react-components` | Convertir des designs Stitch en composants modulaires React/Vite |
| `remotion` | Générer des vidéos de walkthrough depuis des projets Stitch avec Remotion |
| `shadcn-ui` | Intégrer et construire avec les composants shadcn/ui (installation, customisation) |
| `stitch-design` | Point d'entrée unifié pour le design Stitch (prompt, design system, génération d'écrans) |
| `stitch-loop` | Construire des sites web itérativement avec Stitch via un pattern de boucle autonome |

## Utilisation

Pour invoquer un skill, utilisez `/nom-du-skill` dans Claude Code.

Exemples :
- `/simplify` — révise le code modifié
- `/loop 5m /simplify` — révise toutes les 5 minutes
- `/schedule` — gérer les tâches planifiées
