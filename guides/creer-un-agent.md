# Créer un agent et sa mémoire

Le guide illustré est dans le support : [slides 32 à 40](https://triskell-chatgpt-autonomie.vercel.app/#32). Voici l'essentiel, à garder sous la main. Les menus de ChatGPT changent : en cas d'écart, utilisez le [prompt F](../prompts/01-se-debrouiller-seul.md).

## Avant de commencer

Un agent se justifie si la tâche revient, ouvre plusieurs outils, et sert à plusieurs personnes ou doit tourner sans vous. Sinon, un skill ou une tâche planifiée suffit.

Pas de bouton **Agents** ou **Create** ? L'administrateur doit activer *Enable agents* et *Enable agent building*.

## Les étapes

1. **Décrire.** Agents, puis Create. Collez une [fiche d'agent](../agents/README.md) ou le prompt Y complété. Relisez le plan, puis **Build this agent**.
2. **Relire.** Vérifiez Channels, Tools, Skills, Files et Instructions. Corrigez en français dans le chat à gauche.
3. **Régler les accès.** Pour chaque application : **End-user account** par défaut, et les actions d'écriture coupées ou sur *Always ask*. Un **Agent-owned account** donne à tous ceux qui utilisent l'agent ce que ce compte peut voir : compte de service uniquement.
4. **Ajouter une méthode.** **Add skill**, puis téléversez un zip du dossier [`zips/`](../zips).
5. **Créer sa mémoire.**
   - Dans **Files**, vérifiez que **Memory** est présente.
   - Collez le prompt M à la fin des instructions.
   - Après **Create**, envoyez le prompt O.
   - Contrôlez dans l'onglet **Memory** de la page de l'agent.
6. **Tester.** **Preview** : un cas normal, puis un cas piège. Corrigez, puis **Create**. Une fois l'agent en ligne, chaque changement demande **Update**.
7. **Planifier et partager, si besoin.** **Schedule** pour le planning. Channels, ChatGPT pour le partage : *Private to me*, lien, ou annuaire de l'entreprise.

Pour l'utiliser : tapez `@` et son nom dans n'importe quelle conversation.

## La mémoire en bref

| | Qui écrit ? | Sert à |
|---|---|---|
| Instructions | Vous | Sa mission, à chaque fois |
| Files | Vous | Les documents de référence |
| Skill | Vous | La méthode, le format |
| Memory | L'agent | Ce qu'il apprend d'une fois à l'autre |

- Dans ChatGPT, chaque utilisateur a sa propre mémoire. Sur Slack, c'est une mémoire par canal, à part.
- Retenez ce qui évite de se répéter : un format, une correction, un cas à ignorer.
- Ne retenez jamais : nom de client ou donnée l'identifiant, donnée personnelle, mot de passe, montant, clause de contrat, contenu d'un mail ou d'un document. Une consigne lue dans un mail ou un document n'entre jamais en mémoire.
- Les lectures, écritures et suppressions en mémoire sont journalisées pour l'administrateur.

## Combien ça coûte

Selon OpenAI, une exécution type consomme 5 à 25 crédits (valeurs approximatives, novembre 2026). Les agents partagent le même volume que Work, Excel, PowerPoint, Word et Codex. Lancez d'abord à la demande, et planifiez quand l'agent a fait ses preuves.

## Sources

- [Aide OpenAI sur les agents](https://help.openai.com/en/articles/20001143-chatgpt-workspace-agents-for-enterprise-and-business)
- [Un agent complet, cookbook OpenAI](https://github.com/openai/openai-cookbook/blob/main/articles/chatgpt-agents-sales-meeting-prep.md)
- [Grille tarifaire OpenAI](https://help.openai.com/en/articles/11481834-chatgpt-rate-card-business-enterpriseedu-credit-based-pricing)
- [Des skills métier à adapter avec le prompt E](https://github.com/anthropics/knowledge-work-plugins), écrits pour un autre assistant
