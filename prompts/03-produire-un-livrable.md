# Produire : app, présentation, Excel, Word

[Retour à l'index](README.md)

## Prompt W : Trouver votre meilleure app

**Quand :** Vous n'avez pas d'idée d'application, ou vous hésitez entre plusieurs.  
**À joindre :** Rien.

**À copier :**

````text
Aide-moi à choisir la meilleure petite application à créer sur Sites pour mon équipe, puis écris le prompt qui la crée.

Pose-moi ces questions une par une, et attends chaque réponse :
1. Quels calculs, décisions ou vérifications refais-je chaque semaine ?
2. Qui s'en servirait, et à quelle fréquence ?
3. Comment je le fais aujourd'hui, et combien de minutes ça me prend ?
4. Quelles sont les règles exactes : ce qu'on saisit, le calcul, le résultat ?
5. Peut-on le faire sans donnée client et sans connexion à un autre outil ?

Une idée n'est retenue que si je connais les règles exactes et qu'elle marche sans donnée client ni connexion. Sinon, dis-le et aide-moi à la simplifier.

Rends ensuite :
- 3 idées classées, avec pour chacune le gain estimé et le risque.
- Ta recommandation, en deux lignes.
- Dans un bloc à copier, le prompt complet de celle-ci : BUT, DONNÉES fictives, CE QUE L'APPLICATION FAIT (champs, calculs, alertes et leur condition exacte), FORME, TERMINÉ QUAND (trois résultats attendus, que tu calcules). L'application tourne sans serveur et n'est pas publiée.
````

**Vérifiez dans le résultat :**

- Il a attendu chaque réponse.
- L'idée retenue passe les deux critères : règles exactes connues, aucune donnée client ni connexion.
- Les trois résultats attendus sont justes : recalculez-en un vous-même.

**Et ensuite :** Collez le prompt obtenu dans Work, en créant un Site.

## Prompt S : Coder l'app « Comparateur de scénarios » sur Sites

**Quand :** En mode Work, pour créer un Site. Nordval veut comparer deux scénarios de feuille de route côte à côte.  
**À joindre :** Rien, ou vos données si elles ne contiennent aucune information client.

**À copier, puis remplacez les [crochets] :**

````text
Crée un Site : une application web interactive, codée en HTML, CSS et JavaScript, sans serveur et sans compte. Nom : [nom].

BUT
[Ce que l'utilisateur doit pouvoir décider ou voir, en une phrase.]

DONNÉES
[Vos données fictives ou non sensibles, une ligne par élément.]

CE QUE L'APPLICATION FAIT
1. [Les réglages que l'utilisateur modifie.]
2. [Ce qu'il coche, saisit ou choisit.]
3. [Les résultats recalculés immédiatement, et leur formule.]
4. [Les alertes, et leur condition exacte.]

FORME
En français. Sobre, lisible sur grand écran et sur téléphone. Aucune donnée client, aucun tarif.

TERMINÉ QUAND
Au démarrage, tu obtiens : [deux ou trois résultats que vous avez calculés vous-même]. Corrige toi-même tout écart. Si tu ne peux pas exécuter ce contrôle, dis-le. Puis montre-moi l'aperçu, sans rien publier.
````

**Vérifiez dans le résultat :**

- Sur le cas Nordval, A : 895 k€, 1 830 jours-homme, valeur 38, 0 risque élevé, 4,25 par 100 k€.
- Sur le cas Nordval, B : 1 100 k€, 2 280 jours-homme, valeur 40, 2 risques élevés, 3,64 par 100 k€.
- Sur vos données : les résultats que vous avez calculés vous-même sont retrouvés.
- Décochez ou modifiez un élément : tout change aussitôt.

**Et ensuite :** « [Une seule fonction de plus.] Ne change rien d'autre. »

<details><summary>Voir l'exemple déjà rempli</summary>

````text
Crée un Site : une application web interactive, codée en HTML, CSS et JavaScript, sans serveur et sans compte. Nom : « Comparateur de scénarios · Nordval Énergie (client fictif) ».

BUT
Pendant un comité, comparer côte à côte deux scénarios de feuille de route, et voir en direct ce que change chaque décision.

DONNÉES (projet ; budget en k€ ; charge en jours-homme ; valeur sur 10 ; risque)
1. Refonte ERP finance ; 420 ; 900 ; 8 ; Élevé
2. Tableau de bord budgétaire ; 60 ; 120 ; 7 ; Faible
3. Migration cloud ; 310 ; 640 ; 6 ; Moyen
4. Portail fournisseurs ; 180 ; 380 ; 6 ; Moyen
5. Maintenance prédictive ; 260 ; 520 ; 9 ; Élevé
6. Cybersécurité industrielle ; 220 ; 430 ; 9 ; Moyen
7. Application terrain ; 140 ; 310 ; 7 ; Faible
8. Données des compteurs ; 190 ; 400 ; 8 ; Moyen
9. Formation des chefs de projet ; 45 ; 90 ; 5 ; Faible
10. Archivage documentaire ; 70 ; 150 ; 3 ; Faible

SCÉNARIOS AU DÉMARRAGE
- Scénario A « Sécuriser » : projets 2, 3, 6, 8, 9, 10
- Scénario B « Accélérer » : projets 1, 2, 5, 6, 7

CE QUE L'APPLICATION FAIT
1. Deux réglages en haut : enveloppe budgétaire (curseur de 500 à 1 500 k€, 1 000 au départ) et capacité (curseur de 1 000 à 3 000 jours-homme, 2 000 au départ).
2. Un tableau des 10 projets, avec une case à cocher par scénario. Chaque clic recalcule tout, immédiatement.
3. Deux colonnes côte à côte, une par scénario : budget total, charge totale, valeur totale, nombre de projets à risque élevé, valeur par 100 k€.
4. Une alerte rouge qui donne l'écart exact si un scénario dépasse l'enveloppe ou la capacité. Une mention verte s'il respecte les deux.
5. Un graphique à barres qui compare les deux scénarios sur le budget et la charge, chacun rapporté à sa limite.
6. Une phrase de synthèse qui se met à jour, par exemple : « A respecte les limites. B apporte 2 points de valeur de plus, mais dépasse le budget de 100 k€ et la capacité de 280 jours-homme. »
7. Un bouton « Réinitialiser » qui revient aux scénarios de départ.

FORME
En français. Sobre et professionnel, fond blanc, lisible sur grand écran et sur téléphone. Tout tient sur une page. Une mention discrète en pied de page : « Client et chiffres fictifs ».

TERMINÉ QUAND
Au démarrage, tu obtiens : A = 895 k€, 1 830 jours-homme, valeur 38, 0 risque élevé, 4,25 de valeur par 100 k€. B = 1 100 k€, 2 280 jours-homme, valeur 40, 2 risques élevés, 3,64 de valeur par 100 k€. Corrige toi-même tout écart. Si tu ne peux pas exécuter ce contrôle, dis-le. Puis montre-moi l'aperçu, sans rien publier.
````

</details>

## Prompt P : La revue du comité, dans le modèle PowerPoint

**Quand :** En mode Work. Temps 1 d'abord, le plan. Le fichier ensuite.  
**À joindre :** Votre modèle PowerPoint et votre matière.

**À copier, puis remplacez les [crochets] :**

````text
Je prépare [la présentation] pour [public, date]. Je te joins [le modèle] et [la matière].

TEMPS 1 : LE PLAN
Pour chaque slide, écris le titre en une phrase qui dit le message, pas le thème. Attends mon accord avant de créer le fichier.

TEMPS 2 : LE FICHIER
- Remplis le modèle sans changer les couleurs, les polices ni l'ordre des slides.
- Une idée par slide, cinq puces maximum.
- Reprends le vocabulaire et les étapes du client.
- Chaque chiffre vient d'un fichier joint. S'il manque une information, écris « à compléter ».

TERMINÉ QUAND
Tu as relu le fichier créé et rendu chaque slide en image. Si tu ne peux pas le faire, dis-le. Rends-moi le PowerPoint, un tableau Chiffre | Fichier | Onglet ou page, et les slides à relire en priorité.
````

**Vérifiez dans le résultat :**

- Les titres disent un message, pas un thème.
- Sur le cas Nordval : engagements tenu le 24/09, en retard (reporté au 18/11), en attente.
- Sur le cas Nordval : utilisation 74 %, 60,5 %, 86 %. Support : 42 tickets dont 4 encore ouverts, 5,10 jours en moyenne.
- La mise en forme du modèle n'a pas bougé : ouvrez le fichier.

**Et ensuite :** « Ne change que la slide [numéro] : [la seule modification voulue]. »

<details><summary>Voir l'exemple déjà rempli</summary>

````text
Je prépare la revue trimestrielle T3 2026 de Nordval Énergie, client fictif, pour le comité du 12 novembre. Je te joins le modèle PowerPoint, le compte rendu du comité du 13 août, mis à jour au 30/09, et l'export des tickets et de l'utilisation.

TEMPS 1 : LE PLAN
Pour chaque slide du modèle, écris le titre en une phrase qui dit le message, pas le thème. Exemple : « L'utilisation remonte à 86 % après le creux d'août ». Attends mon accord avant de créer le fichier.

TEMPS 2 : LE FICHIER
- Remplis le modèle sans changer les couleurs, les polices ni l'ordre des slides. Si le skill triskell-design-system est installé, le modèle joint prime sur lui.
- Une idée par slide, cinq puces maximum.
- Chaque engagement a son statut et sa date. Tenu : preuve écrite. En retard : à Triskell d'agir, échéance passée ou reportée. En attente : au client ou à un tiers d'agir, ou échéance à venir.
- Reprends la demande du client sur la comparaison de deux scénarios dans les prochaines étapes.
- Chaque chiffre vient d'un fichier joint. S'il manque une information, écris « à compléter ».

TERMINÉ QUAND
Tu as relu le fichier créé et rendu chaque slide en image, et il garde le nombre de slides du modèle. Si tu ne peux pas le faire, dis-le. Rends-moi le PowerPoint, un tableau Chiffre | Fichier | Onglet ou page, avec le calcul des moyennes, et les slides à relire en priorité.
````

</details>

## Prompt X : Le tableau Excel qui répond au client

**Quand :** Un chiffre est contesté, ou un export doit devenir une analyse réutilisable.  
**À joindre :** Votre fichier Excel, sans donnée identifiant un client.

**À copier, puis remplacez les [crochets] :**

````text
Je te joins [le fichier]. Je veux répondre à cette question : [la question].

1. Décris d'abord le fichier : onglets, colonnes, nombre de lignes. Signale toute donnée anormale, et dis comment tu la traites.
2. Ajoute un onglet « Synthèse », sans modifier les onglets existants, avec : [les indicateurs, par quel axe].
3. Utilise de vraies formules Excel qui pointent vers les onglets sources, sans valeur écrite en dur, sur des colonnes entières : une ligne ajoutée met la synthèse à jour.
4. Ajoute un graphique simple de [l'indicateur].

TERMINÉ QUAND
Les totaux qui s'additionnent sont justes et aucune cellule n'affiche d'erreur. Si tu ne peux pas recalculer le fichier, dis-le. Rends-moi le fichier Excel, puis la réponse en trois lignes, chaque chiffre avec sa cellule.
````

**Vérifiez dans le résultat :**

- Sur le cas Nordval : 42 tickets, 5,10 jours en moyenne, délai maximal de 20 jours, 4 tickets ouverts.
- Question d'usage 14 tickets, 1,71 j. Paramétrage 12, 2,17 j. Incident 9, 5,22 j. Évolution 7, 16,71 j.
- Hors évolutions : 35 tickets, 2,77 jours. Résolus seuls : 38 tickets, 4,29 jours, et 34 tickets, 2,74 jours hors évolutions.
- Il dit que le fichier ne définit pas le délai des 4 tickets ouverts, sans inventer d'explication.
- Ajoutez une ligne de test à l'onglet source : la synthèse doit changer.

**Et ensuite :** « Montre-moi la formule de la cellule [référence]. »

<details><summary>Voir l'exemple déjà rempli</summary>

````text
Le client conteste un chiffre de ma revue : « Votre support met 5 jours à traiter un ticket, c'est trop. » Je veux savoir si le chiffre est juste, et ce qu'il cache. Je te joins l'export.

1. Décris d'abord le fichier : onglets, colonnes, nombre de lignes. Signale toute donnée anormale.
2. Ajoute un onglet « Synthèse », sans modifier les onglets existants. Par catégorie : le nombre de tickets, le délai moyen, le délai le plus long, les tickets ouverts, puis une ligne de total.
3. Ajoute le délai moyen sans les demandes d'évolution.
4. Pour les tickets au statut Ouvert : dis s'ils sont inclus, dis si le fichier définit leur délai, n'invente aucune explication, et donne chaque moyenne avec et sans eux.
5. Utilise de vraies formules Excel qui pointent vers l'onglet « Tickets T3 », sans valeur écrite en dur, sur des colonnes entières : si j'ajoute un ticket, la synthèse se met à jour.
6. Ajoute un graphique simple du délai moyen par catégorie.

TERMINÉ QUAND
Le total des tickets et le total des tickets ouverts égalent la somme des catégories, et aucune cellule n'affiche d'erreur. Si tu ne peux pas recalculer le fichier, dis-le. Rends-moi le fichier Excel, puis en trois lignes ce que je réponds au client, chaque chiffre avec sa cellule.
````

</details>

## Prompt D : Passer d'un PowerPoint à un Word, dans votre modèle

**Quand :** Un support de présentation à transformer en document de référence.  
**À joindre :** Le PowerPoint source et le modèle Word.

**À copier, puis remplacez les [crochets] :**

````text
Je te joins [le document source] et notre modèle [Word / PowerPoint]. Je veux [le document attendu].

1. Donne-moi d'abord le plan : quelle partie du modèle reçoit quel contenu. Attends mon accord avant de créer le fichier.
2. Remplis ensuite le modèle, sans ajouter aucun fait.

RÈGLES
- Ne change ni les titres, ni les styles, ni l'ordre du modèle.
- Chaque chiffre vient du document source. S'il manque une information, écris « à compléter ».

TERMINÉ QUAND
Tu as relu le fichier créé, rendu chaque page en image et contrôlé les chiffres. Si tu ne peux pas le faire, dis-le. Rends-moi le fichier, puis la liste de ce que tu n'as pas repris et pourquoi.
````

**Vérifiez dans le résultat :**

- Titres, styles et ordre du modèle sont intacts.
- Chaque chiffre est identique à celui du PowerPoint.
- La liste des slides non reprises est cohérente.

**Et ensuite :** « Ne change que la partie [numéro] : [la seule modification voulue]. »

<details><summary>Voir l'exemple déjà rempli</summary>

````text
Je te joins un PowerPoint et notre modèle Word. Je veux en faire un document de référence.

1. Donne-moi d'abord le plan : quelle partie du modèle reçoit quelles slides. Attends mon accord avant de créer le fichier.
2. Remplis ensuite le modèle Word avec le contenu du PowerPoint. Transforme les puces en phrases rédigées, sans ajouter aucun fait.

RÈGLES
- Ne change ni les titres, ni les styles, ni l'ordre du modèle.
- Chaque chiffre vient du PowerPoint. S'il manque une information, écris « à compléter ».

TERMINÉ QUAND
Tu as relu le fichier créé, rendu chaque page en image et contrôlé les chiffres. Si tu ne peux pas le faire, dis-le. Rends-moi le fichier Word, puis la liste des slides non reprises et pourquoi.
````

</details>
