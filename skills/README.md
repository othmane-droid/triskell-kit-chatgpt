# Les skills

| Besoin | Skill | Ce qu'il fait |
|---|---|---|
| Présentations | `design-system/triskell-design-system` | Crée un PowerPoint dans le modèle officiel et contrôle la charte |
| Kick-off | `triskell-kickoff-dc-dsc` | Passation DC → DSC, contrôles de cohérence, verdict GO / NO GO |
| Réunions | `triskell-compte-rendu` | Transcription ou notes → compte rendu et mail de suivi |
| COPIL | `triskell-synthese-copil` | Compte rendu, mails, notes → pack COPIL |
| Synthèse | `triskell-synthese-documents` | Documents → synthèse sourcée |
| Mails | `triskell-emails` | Tri, réponses, relances, en brouillon |
| Excel | `triskell-excel-analyse` | Analyse, corrections listées, onglet Synthèse |
| Avant-vente | `triskell-reponse-appel-offres` | Analyse d'AO, go / no-go, matrice de conformité |
| Sécurité | `triskell-questionnaire-securite` | Questionnaire rempli depuis la base validée |
| Documents | `triskell-document-modele` | Source + modèle → nouveau document Word |
| Support | `triskell-reponse-support` | Ticket → classement, réponse, note d'escalade |
| Marketing | `triskell-webinaire-contenus` | Replay → article, posts, newsletter, FAQ |
| Veille | `triskell-veille-ppm` | Veille PPM datée et sourcée |
| Traduction | `triskell-traduction` | FR ↔ EN, ES, DE, avec glossaire PPM |

## Installer un skill

1. Téléchargez son `.zip` dans le dossier [`zips/`](../zips).
2. Dans ChatGPT : Plugins, onglet Skills, créer, puis téléverser le fichier. L'administrateur peut avoir à autoriser l'import.
3. Ouvrez une nouvelle conversation et testez-le avec un fichier de [`exemples/fichiers-de-test/`](../exemples/fichiers-de-test).

**Si l'import n'est pas proposé :** ouvrez le `SKILL.md`, copiez son contenu et recréez le skill avec l'assistant de création de ChatGPT, en joignant les fichiers de ses dossiers.

**Les skills qui fabriquent un fichier** utilisent des scripts Python, testés hors de ChatGPT. Faites un premier essai sur un fichier de test.

**Pour le préciser :** chaque `SKILL.md` se termine par « Pour affiner le skill ». Les informations attendues sont marquées `[à compléter par Triskell]`.
