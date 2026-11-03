# Nordval - export tickets T3 : description du fichier et réponse client

## Étape 1 - Description du fichier
- Onglet « Tickets T3 » : 42 tickets (43 lignes avec l'en-tête), 5 colonnes : Ticket, Ouvert le, Catégorie, Statut, Délai de traitement (jours). Aucun doublon d'identifiant (NV-1001 à NV-1042).
- Onglet « Utilisation » : 3 lignes (juillet, août, septembre 2026), 4 colonnes : Mois, Utilisateurs actifs, Licences achetées, Projets suivis.
- 4 catégories : Question d'usage (14), Paramétrage et droits (12), Incident (9), Demande d'évolution (7). Statuts : 38 Résolu, 4 Ouvert.

### Données anormales
1. **Les 4 tickets ouverts ont un délai renseigné** (NV-1041 : 15 j, NV-1037 : 12 j, NV-1033 : 20 j, NV-1028 : 4 j). Un ticket non résolu n'a pas de délai de traitement, et le fichier ne définit pas ce nombre : à clarifier avant de le citer. Il est pourtant inclus dans les moyennes. Trois de ces quatre tickets sont des demandes d'évolution.
2. **Dates en texte** (format jj/mm/aaaa), pas de vraies dates Excel : tri et calculs de date impossibles sans conversion.
3. Lignes triées par date d'ouverture, mais numéros de ticket non chronologiques (ex. NV-1041 ouvert avant NV-1034).
4. Le délai maximum de 20 jours est atteint deux fois : NV-1034 (résolu) et NV-1033 (ouvert).
5. Pas de date de résolution ni d'unité précisée (jours calendaires ou ouvrés ?).
6. Médiane globale : 3 jours (la moyenne de 5,10 est tirée par quelques valeurs hautes).

## Résultats de la synthèse (onglet « Synthèse », vérifiés par calcul indépendant)
| Catégorie | Tickets | Délai moyen (j) | Max (j) | Ouverts |
|---|---|---|---|---|
| Question d'usage | 14 | 1,71 | 3 | 0 |
| Paramétrage et droits | 12 | 2,17 | 5 | 0 |
| Incident | 9 | 5,22 | 8 | 1 |
| Demande d'évolution | 7 | 16,71 | 20 | 3 |
| **Total** | **42** | **5,10** | **20** | **4** |
| Hors demandes d'évolution | 35 | 2,77 | 8 | 1 |

## Réponse au client (3 lignes, cellules de l'onglet « Synthèse »)
1. Sur 42 tickets (B8), le délai moyen est de 5,10 jours (C8), dont 4 tickets encore ouverts (E8) : le chiffre de 5 jours est exact en moyenne globale.
2. Cette moyenne est tirée par les demandes d'évolution (7 tickets, 16,71 jours, C7) : hors évolutions, 35 tickets (B10) sont traités en 2,77 jours en moyenne (C10).
3. Questions d'usage : 1,71 j (C4) ; paramétrage et droits : 2,17 j (C5) ; incidents : 5,22 j (C6) ; le plus long : 20 jours (D8).

Réserve à dire au client : les 4 tickets ouverts sont comptés avec un délai qui n'est pas un délai de résolution. En ne gardant que les tickets résolus, les moyennes baissent (tickets résolus seuls : 38 tickets, 4,29 j de moyenne ; hors évolutions : 34 tickets, 2,74 j).
