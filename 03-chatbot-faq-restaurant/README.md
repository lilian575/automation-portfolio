# Chatbot FAQ Restaurant — 80% des questions clients gérées sans humain

> **Avant** : Un employé passait 35 h/semaine à gérer des appels, messages et réservations — pour 1 600€/mois.

> **Après** : Un agent IA gère tout 24 h/24, 7j/7, pour une fraction du coût.

---

## Le problème résolu
Les restaurants perdent des clients chaque soir parce que personne ne répond aux questions en dehors des heures d'ouverture. Les réservations ratées et les appels sans réponse coûtent des dizaines de clients par mois — sans que vous le sachiez.

## Pour qui
Restaurants, hôtels, commerces locaux avec un volume de questions clients répétitives.

## Stack
- **n8n** — orchestration des workflows
- **Claude Haiku 4.5** — modèle IA qui répond naturellement dans la langue du client
- **Google Sheets** — FAQ modifiable par le client sans aucune compétence technique
- **PostgreSQL / Supabase** — mémoire persistante entre sessions
- **Telegram + Gmail** — notifications réservations + escalade humaine

## Fonctionnalités
- Prend les réservations et notifie le restaurant par Telegram en temps réel
- Répond aux questions FAQ 24 h/24 dans la langue du client
- Si la question dépasse la FAQ : collecte l'email et alerte un employé par Gmail
- FAQ mise à jour par le client directement dans Google Sheets — sans vous contacter
- Mémoire persistante — le client n'a jamais à se répéter entre deux conversations

## Résultat concret
80% des questions clients gérées sans intervention humaine. Réservations prises à 3 h du matin, le week-end, les jours fériés.

## Prix indicatif
400–800€ selon le périmètre. Maintenance optionnelle 50–150€/mois.

## Me contacter
[Malt](https://www.malt.fr/profile/lilianperfetti) · [LinkedIn](https://www.linkedin.com/in/lilian-perfetti-0a4816324/) · lilian.perfetti.auto@gmail.com
