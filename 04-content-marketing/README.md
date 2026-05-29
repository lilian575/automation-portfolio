# 04 — Pipeline Contenu & Marketing

Automatise la création de brouillons de posts à partir de tes idées Notion.

## Ce que ça fait

1. Se déclenche chaque lundi à 9h
2. Lit ta base Notion "Idées de posts" (filtre : statut = "À rédiger")
3. Génère un post LinkedIn via GPT-4o-mini (hook + problème/solution + hashtags)
4. Crée un brouillon Gmail prêt à être relu et publié
5. Met à jour le statut Notion → "Brouillon prêt"

## Configuration requise

| Étape | Action |
|-------|--------|
| Notion | Connecter ton compte + remplacer `YOUR_NOTION_DATABASE_ID` par l'ID de ta base |
| Gmail | Connecter ton compte Google |
| OpenAI | Ajouter ta clé API |

### Structure de la base Notion

La base doit contenir au minimum :
- `Titre` (propriété title)
- `Description` (propriété text) — décrit l'automation à promouvoir
- `Statut` (propriété select) avec les valeurs : `À rédiger`, `Brouillon prêt`, `Publié`

## Résultat

Un brouillon Gmail par idée, avec objet `Post à publier - [titre]`, prêt à copier-coller sur LinkedIn.
