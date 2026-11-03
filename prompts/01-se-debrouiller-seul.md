# Se débrouiller seul

[Retour à l'index](README.md)

## Prompt F : Le prompt quand vous êtes seul

**Quand :** Vous ne savez pas comment faire, ou la fonction a changé depuis la formation.  
**À joindre :** Rien.

**À copier, puis remplacez les [crochets] :**

````text
Je travaille dans ChatGPT Business. Je veux [votre tâche, et à quelle fréquence]. Donne-moi :

1. La solution la plus simple qui suffit : conversation, projet, skill, tâche planifiée, agent ou plugin. Dis pourquoi, et pourquoi pas la brique du dessus.
2. Les étapes, une par une. Vérifie-les en cherchant sur le web dans la documentation officielle d'OpenAI, avec le lien de chaque page. Si tu ne trouves pas, dis-le : n'invente pas un menu.
3. Ce qui peut dépendre des réglages de notre administrateur.
4. Le premier prompt à essayer, et comment je saurai que le résultat est bon.
````

**Vérifiez dans le résultat :**

- Chaque étape a un lien vers une page d'OpenAI : ouvrez-en une.
- Il explique pourquoi la brique du dessus n'est pas nécessaire.

**Et ensuite :** « Mon résultat ne va pas : [ce qui ne va pas]. Quelle consigne manquait ? »

<details><summary>Voir l'exemple déjà rempli</summary>

````text
Je travaille dans ChatGPT Business. Je veux chaque semaine préparer mes comités à partir de mes mails et du dernier compte rendu. Donne-moi :

1. La solution la plus simple qui suffit : conversation, projet, skill, tâche planifiée, agent ou plugin. Dis pourquoi, et pourquoi pas la brique du dessus.
2. Les étapes, une par une. Vérifie-les en cherchant sur le web dans la documentation officielle d'OpenAI, avec le lien de chaque page. Si tu ne trouves pas, dis-le : n'invente pas un menu.
3. Ce qui peut dépendre des réglages de notre administrateur.
4. Le premier prompt à essayer, et comment je saurai que le résultat est bon.
````

</details>

## Prompt U : Votre audit personnel, avec roast

**Quand :** Dans une nouvelle conversation Chat, hors projet, avec un modèle de réflexion. Le résultat ne regarde que vous.  
**À joindre :** Rien.

**À copier :**

````text
Audite ma façon d'utiliser ChatGPT Business et aide-moi à progresser. Ton direct et drôle, tutoiement. Tu vises ma façon de travailler, jamais ma personne.

1. CE QUE TU VOIS
Liste ce que tu peux consulter ici (mémoire, historique, projets, skills, tâches planifiées, agents, plugins) et ce que tu ne peux pas. Si tu vois trop peu de choses pour juger, pose-moi 5 questions au maximum et attends mes réponses.

2. LE VERDICT
- Une note sur 20 pour chaque axe : qualité de mes demandes, contexte donné, réutilisation, automatisation, vérification. Axe impossible à observer : écris « non évalué », sans note.
- Un score sur 100 : la moyenne des axes évalués, multipliée par 5. Ajoute ton niveau de confiance.
- Mon profil en trois mots.
- Un roast de 5 lignes. Chaque pique part d'un fait observé.

3. MON PLAN
Les 5 actions qui me feront gagner le plus de temps, dans un tableau : Rang | Action | Type (habitude, skill, tâche planifiée, agent, plugin, quota) | Avant → après | Gain estimé par semaine.

4. MES 7 JOURS
Une action par jour, 10 minutes maximum.

RÈGLES
- Marque chaque constat : (observé), (déclaré) si je te l'ai dit, ou (supposé). Un gain de temps est toujours une estimation.
- Aucun nom de client ni donnée confidentielle dans ta réponse.
- Pas d'introduction, une page et demie au maximum.
- Termine par : « Quelle action veux-tu que je prépare ? »
````

**Vérifiez dans le résultat :**

- Chaque pique du roast renvoie à un fait que vous reconnaissez.
- Les constats « supposé » ne sont pas présentés comme des certitudes.
- Les 5 actions sont faisables dans votre espace.

**Et ensuite :** « Prépare l'action 1 : écris le prompt, le skill ou la description d'agent prêts à coller. »

## Prompt G : Transformer une bonne conversation en skill

**Quand :** Vous venez d'obtenir un bon résultat, et la tâche reviendra.  
**À joindre :** Rien. À écrire à la fin de la conversation réussie.

**À copier :**

````text
Ce résultat me convient et la tâche va revenir. Crée un skill à partir de cette conversation.

Reprends la méthode, le format de sortie et mes corrections. Le skill doit contenir :
- une description de deux lignes : quand il sert, et quand il ne sert pas ;
- ce qu'il attend de moi au départ ;
- ce qu'il écrit quand il lui manque une information ;
- aucune donnée propre à ce cas : ni nom de client, ni chiffre venant de ce cas.

Pose-moi tes questions si besoin. Propose ensuite deux cas pour le tester, un où il doit se lancer et un où il ne doit pas, puis propose-moi de l'installer.
````

**Vérifiez dans le résultat :**

- Aucun nom de client ni chiffre venant de ce cas dans le skill.
- Dans une nouvelle conversation, il se lance sur le bon cas et pas sur l'autre.

**Et ensuite :** Testez-le dans une nouvelle conversation, sur un autre cas, avant de le partager.

## Prompt R : Le relais vers une nouvelle conversation

**Quand :** La conversation devient longue, ou l'assistant perd le fil.  
**À joindre :** Rien.

**À copier :**

````text
Résume cette conversation pour que je la reprenne dans une nouvelle, écrit pour un assistant qui n'a rien lu : l'objectif, les décisions prises, les contraintes, les fichiers utiles avec leur nom exact, ce qui a déjà échoué, ce qui reste à faire et la prochaine étape. Quinze lignes maximum, dans un bloc à copier. N'ajoute rien de nouveau.
````

**Vérifiez dans le résultat :**

- Collez le résumé dans une nouvelle conversation et demandez la prochaine étape : elle doit être la bonne.

**Et ensuite :** Ouvrez une nouvelle conversation, collez le résumé, et joignez seulement les fichiers encore utiles.
