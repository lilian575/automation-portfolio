# 05 — Triage Support Client Gmail

Classe automatiquement les emails entrants et envoie une réponse adaptée.

## Ce que ça fait

1. Se déclenche toutes les 30 minutes
2. Récupère les emails non lus dans ta boîte Gmail (max 20)
3. Classifie chaque email via GPT-4o-mini : `achat`, `bug`, `question`, `autre`
4. Applique un label Gmail correspondant
5. Envoie une réponse automatique selon la catégorie

## Réponses automatiques

| Catégorie | Réponse envoyée |
|-----------|-----------------|
| `achat` | Merci pour votre achat ! Votre automation sera livrée sous 24h. |
| `bug` | Merci de nous avoir contacté. Notre équipe examine votre problème. |
| `question` | Merci pour votre question. Nous vous répondons sous 48h. |
| `autre` | Merci pour votre message. Nous vous répondons bientôt. |

## Configuration requise

### 1. Créer les labels Gmail manuellement
Dans Gmail → Paramètres → Labels, créer :
- `Support/Achat`
- `Support/Bug`
- `Support/Question`
- `Support/Autre`

### 2. Connecter les services dans n8n
| Service | Credential |
|---------|-----------|
| Gmail | OAuth2 Google |
| OpenAI | API Key |

## Notes

- La classification utilise GPT-4o-mini avec temperature 0 pour être déterministe
- Les emails déjà lus ne sont pas retraités
- Tu peux ajuster les messages de réponse directement dans les noeuds "Réponse - *"
