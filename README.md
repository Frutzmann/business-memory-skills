# Business Memory Skills

Skills dynamiques pour le **Business Memory Agent** du cabinet Morel & Associés.

Chaque skill est un fichier Markdown (`SKILL.md`) chargé dynamiquement par l'agent n8n via l'API GitHub.

## Structure

```
skills/
├── relance/SKILL.md        # Relance de factures impayées
├── facturation/SKILL.md    # Émission et gestion de factures
├── reporting/SKILL.md      # Rapports mensuels internes et clients
└── onboarding/SKILL.md     # Onboarding nouveau client (4 semaines)
```

## Usage

L'agent interroge l'endpoint :
```
GET /repos/Frutzmann/business-memory-skills/contents/skills/
```

Puis charge le skill approprié selon la demande utilisateur.

## Licence

Usage interne — Cabinet Morel & Associés.
