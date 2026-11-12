# Changelog / Journal des versions

**English** · [Français](#français)

All notable changes to Arbora. Version numbers follow major.minor.patch: a new feature bumps the second number, a fix bumps the third.

## [1.2.0] - 2026-11-11

### Added
- **Family book as PDF**: cover, clickable contents, one entry per person (dates, places, parents, unions, children, life journey, notes, sources) with photos (or a blank icon when there is none), and an index. The cover carries the Arbora logo. Ancestors by generation with Sosa numbers, descendants, or the whole tree.
- **Life journey**: free events (job, studies, military service, move, census, religion, award, property, other) with date, place and detail, shown as a timeline per person with the age at each step. Their places appear on the map.
- **Structured sources**: a source is described once (type, repository and reference, link, reliability on 3 levels) and cited on several records, with what it proves. Source manager in the gear menu.
- **Sosa numbering and pedigree collapse**: number on each record and in the Ancestors view, table of completeness per generation, list of shared ancestors, CSV export.
- **Research to do** per record, gathered at the top of the Checks tab.
- **Advanced search**: name, sex, status, birth years, place, occupation, branch, missing information, with CSV export of the results.
- **Family calendar**: birthdays, wedding and death anniversaries for the next 30 days, and export as an .ics file for a phone or computer calendar.
- **Compare with another file**: read-only overview of identical, different, new and missing people before importing.
- **Password protection**: the tree is encrypted in the file (AES-GCM 256, key derived with PBKDF2) and the file asks for the password when opened.
- **Life journeys on the map**: a line per person from birth to death through dated steps.
- **Life journey in the record PDF**: optional (with or without) from the preview, always on one page.
- **Easier to find**: Sosa button next to « Record » on every record, family calendar in the gear menu, « Download the latest version » in About is a direct link to the file, password window that offers to remove the protection first when it is on.
- **Lighter file**: comments and useless spaces removed at build time (no change to the code itself).
- **Keyboard shortcuts**: list with the `?` key, new shortcuts (`/`, `N`, `E`, `1`–`8`, `Shift+F`).
- **Update and keep my tree**: the update banner can download the new version, put the open tree in it and save the file.
- Direct download: the update banner downloads the new file directly, and each release carries a stable `arbora.html` file for a permanent download link. Project home page with an online demo.

### Fixed
- Update detection: a new version could go unnoticed for up to 24 hours, and the banner was shown only once. The known version is now remembered and shown every time the file is opened, the check runs at most once an hour, and a failed check is retried at the next opening.
- A protected file no longer keeps unsaved changes in the browser cache.

## [1.1.0] - 2026-11-09

### Added
- Delete a person or a family from the top bar, with the consequences explained before confirming.
- Record export as JSON (to import into another tree, with the details you choose) or as a laid-out PDF including personal insights. Also available from the « Personal insights » window.
- Family export with a chosen level of detail, and smart import that recognises people already in the tree, merges them and links the family in the right place.
- Change history kept in the file, undo still possible after saving during the session, log export (text, CSV, JSON).
- Duplicate tool (side-by-side comparison, merge field by field or keep separate) and loop tool (full circuit, suspicious link, cut a link or split two namesakes).
- Every export carries Arbora’s name, version, logo and credit.
- Delete and export by surname, with options for partners, children and all descendants.
- Export window redesigned as cards grouped by purpose (whole tree, image or print, part of the tree, other formats).
- Record PDF on a single page with selectable text, « Arbora » linked to the project, and a preview before saving.
- Loop tool: before/after preview of the chosen fix (cut a parent-child link, remove a union, split two namesakes), then a confirm button. Loops that go through a union are now handled.
- Thumbnails of attached images in the record.
- Life photos: three dated photos (childhood, midlife, later life) above the events, picked from the documents or a file, with the age computed automatically. Included in the record PDF, still on one page.
- Images are lightened when attached: choice of size with a preview, actual size before/after and a reminder that Arbora is not a photo storage tool. A « Lighten images… » tool (gear menu) reduces the images already in the tree.
- Photos of children, siblings and half-siblings in the record.
- Life photos: reorder by drag and drop (mouse or touch), magnifier and one-click change in edit mode with a pencil badge, optional title (shown greyed as a suggestion only), age in the enlarged view.
- Web links (record photo, life photo, document): Arbora offers to save a local copy in the file so it stays readable offline, explains why and shows the estimated size increase. Sites that block copying keep the link only, with an explanation.
- Text documents (TXT, Word, spreadsheets…) are compressed automatically when attached. PDFs, images and ZIP files are already compressed and are kept as they are.
- Photos in the views (tree, ancestors, descendants, fan, timeline): photos only, photos and a blank icon in the sex colour for people without one, or none, chosen in the gear menu.
- Web link with a local copy: the compression level is chosen in the same window (image sizes with their weight, or lossless compression for documents).
- Trail of opened records above the record name when moving through links (hover shows the full list), closing a record returns to the previous one.
- Preview before saving for every PDF and image export (tree, views, statistics, PNG, SVG), and a clickable link to the GitHub project in the footer of every PDF.
- Duplicate tool for groups of 2, 3, 4 records or more: records to combine and main record chosen with a tick, value by value choice, documents and residences item by item, details of each record, « After merging » column updated live.
- Map: « Relocate all places… » button with an explanation (case of « Montréal » placed in the United States) and a progress bar.
- Light or dark look for every PDF and image export, chosen in the preview, using the colours of the active theme (changeable in the gear menu › Colour themes).
- In read mode, clicking the record photo opens it in a viewer.
- PDF export for the Ancestors, Descendants, Fan and Timeline views.
- Places report PDF from the Map: key figures, place diagram (circles sized by number of people, lines from place of birth to place of death), top places and countries, full table with the people of each place.
- Check report PDF, sorted by type of remark.
- « Check for updates » in the gear menu.
- « Buy me a coffee » button (Ko-fi) next to « Add a person » after 30 minutes of use, can be hidden and comes back 30 minutes later.
- Images over 1 MB are flagged: a banner offers to lighten them, and a « Lighten » button appears next to the document or in the record photo menu.

### Changed
- The Save button overwrites the open file once chosen in the session, and offers another location if writing fails.
- Records: clickable parent cards and sibling chips, reorganised header with buttons of the same height, back to the original record after « New person… » for a parent or sibling, empty sections shown as « No information » in read mode.
- Ages shown in the Ancestors and Descendants views.
- Windows adapt their width to avoid scrolling and keep the same gap below the top bar and at the bottom. « What’s new » opens right below its button, the support banner sits under the title.
- Help completed with the new features, « About Arbora » button highlighted, Help icon in the tabs bar, even spacing of the top buttons.
- « Auto layout » is now a button at the bottom right of the tree, next to + − Fit.
- Centring on a person (target button, double-click) accounts for the open record and log.
- Personal insights list every name (no more « and N others ») and show « unknown » when an age is missing.
- Automatic place lookups no longer clutter the log.
- The log is split into two equal areas with their own scrolling: current session (browser cache) and file history.
- Export window: whole tree, then part of the tree, then image or print with the view chooser on the same line. draw.io export removed.
- Fan chart: first name and surname are always shown, sized to each segment.
- « Add a person » button with an icon. In read mode, notes take the height of their text.
- Record photo: size choice with a preview when importing, and a menu (file, web link, documents, remove) when clicking it in edit mode.
- Children, sibling and half-sibling tiles take the sex colour like the parent cards, without the coloured dot, always with a photo or an avatar so they share the same height.
- Residence periods are shown in full.
- Import and duplicate merge take photos and documents into account: identical images and documents are recognised by their content and not duplicated, the record photo appears in the differences with thumbnails, the photo that is not kept goes to the documents, life photos fill the free slots.
- Identical documents when merging duplicates or importing: keep a single copy (recommended) or keep everything. Documents with the same name are always renamed automatically (« record (2).pdf »).
- A record without a photo shows a blank icon in its header. Blank icons in the views use the same style as the small tiles of the record (light background, outline in the sex colour).
- A record being edited stays open until « Done »: clicking outside, another box or a link does not close it or open another record.
- « This is me » is a star button in the style of the highlight button. The photo buttons are gone from the record: the photo or the icon opens the menu.
- Loop tool: before/after circle diagram, a split shown as two branches, and a window that stays open (click a name to open the record, the tool updates after every change).
- Descendants view with the same boxes as Ancestors (partners no longer squeezed into the boxes). Timeline: photos and icons in a column right of the names.
- The record history is a separate banner at the top of the record. Clicking elsewhere or on another box while a history exists asks whether to close it (and then opens the chosen box).
- « This is me » is shown as a yellow star badge on the record photo.
- Header: « Arbora » next to the logo, a separator, then the tree name, editable on hover. The logo and the footer « Arbora 1.1.0 · Designed by florentdoug » open « About Arbora ».
- Record photo in the PDF cut out as a vector shape with a clean border, round or square chosen in the preview like light or dark. The photo viewer can switch to actual size.
- Statistics export as two cards (PDF and PNG). In a window opened from Export, « Cancel » goes back to the Export menu, with a « Back to the Export menu » button.
- Places report PDF: base map with continents and country borders (Natural Earth, public domain).
- « Lighten images » also covers record photos and re-encodes heavy images even when they are already small in pixels.
- The round or square choice for photos applies to the record (photo, cards, tiles) and to every tab (Ancestors, Descendants, Fan, Timeline).
- Unions and children: the partner’s photo (or icon) appears in the header of each union and opens their record.
- Record documents: one line per document (long names truncated, full name on hover), actions as aligned, readable icons (feature, lighten, compress, remove). A heavy life photo shows a « lighten » badge, and the photo viewer offers to lighten a heavy image at the bottom of the window.

### Fixed
- Residences could be removed from a record in read mode.
- A place with its country (for example « Montréal, Canada ») could be located in the wrong country on the map.
- Saving a second time could download a copy named « (1) » instead of overwriting the file.
- A place whose country was added or changed afterwards (« Montréal » then « Montréal, Canada ») kept its old, wrong position.
- Some « Fix » buttons for loops did nothing.
- Values in the right-hand column of the duplicate tool were not aligned.
- The JSON export still contained images removed from records (they are only kept in memory to allow undo).
- The file history could not be scrolled in the log.
- Union cards: the divorce hint and « Export this family » were not aligned.
- « Web link… » for the record photo opened the relationship analysis instead of the link window.
- Duplicate tool: the « Keep the right-hand record instead » button now becomes « Keep the left-hand record instead » after switching, and both records stay in their column.
- « New person… » for a child or a partner created a record named « Nouvel enfant » or « Nouveau partenaire »: the fields are now empty and the new record opens in edit mode with a way back.
- Multi-page previews (check report, statistics…): the top of the first page was cut off.
- The « Attach a file » and « Add a web link » buttons of the Documents section were hidden in edit mode.

## [1.0.0] - 2026-11-08

First public release.

### Added
- Interactive tree with automatic layout, flagged isolated groups, mini-map.
- Records in read mode by default with an Edit button, personal insights, unions numbered by marriage date, divorce.
- Ancestry, descendants, fan chart, timeline and map views, all filterable.
- Statistics with “Did you know?” following the chosen filter.
- Checks: impossible dates, genealogical loops, duplicates, formats, research sources by country.
- Relationship analysis between two people.
- Family film (one person, one surname, the whole tree) with fun facts, exportable as MP4 or WebM.
- GEDCOM and JSON import with duplicate merging, data recovery from an old copy.
- PDF, image, GEDCOM and JSON exports, plus a copy of the tool (editable or read-only).
- AI instructions: tree correction, guided ancestor research, starting from scratch.
- Update check (can be turned off).
- Six languages, light and dark themes.

---

# Français

[English](#changelog--journal-des-versions) · **Français**

Toutes les évolutions notables d’Arbora. Les numéros suivent le format majeur.mineur.correctif : une nouveauté fait monter le deuxième chiffre, une correction le troisième.

## [1.2.0] - 2026-11-11

### Nouveautés
- **Livre de famille en PDF** : couverture, sommaire cliquable, une notice par personne (dates, lieux, parents, unions, enfants, parcours de vie, notes, sources) avec photos (ou une icône vierge quand il n’y en a pas), et un index. La couverture porte le logo Arbora. Ancêtres par génération avec numéros Sosa, descendants, ou tout l’arbre.
- **Parcours de vie** : événements libres (métier, études, service militaire, déménagement, recensement, religion, distinction, propriété, autre) avec date, lieu et précision, affichés en frise par personne avec l’âge à chaque étape. Leurs lieux apparaissent sur la carte.
- **Sources structurées** : une source se décrit une fois (type, lieu de conservation et cote, lien, fiabilité sur 3 niveaux) et se cite sur plusieurs fiches, avec ce qu’elle prouve. Gestion des sources dans la roue dentée.
- **Numérotation Sosa et implexe** : numéro sur chaque fiche et dans la vue Ascendance, tableau de complétude par génération, liste des ancêtres communs, export CSV.
- **Recherches à faire** par fiche, réunies en haut de l’onglet Vérifications.
- **Recherche avancée** : nom, sexe, statut, années de naissance, lieu, profession, branche, informations manquantes, avec export CSV des résultats.
- **Calendrier de la famille** : anniversaires, mariages et décès des 30 prochains jours, et export en fichier .ics pour l’agenda du téléphone ou de l’ordinateur.
- **Comparer avec un autre fichier** : vue en lecture seule des personnes identiques, différentes, nouvelles et absentes avant d’importer.
- **Protection par mot de passe** : l’arbre est chiffré dans le fichier (AES-GCM 256, clé dérivée par PBKDF2) et le fichier demande le mot de passe à l’ouverture.
- **Parcours de vie sur la carte** : un trait par personne, de la naissance au décès en passant par les étapes datées.
- **Parcours de vie dans la fiche PDF** : au choix (avec ou sans) depuis l’aperçu, toujours sur une page.
- **Plus facile à trouver** : bouton Sosa à côté de « Fiche » sur chaque fiche, calendrier de la famille dans le menu engrenage, « Télécharger la dernière version » dans À propos en lien direct vers le fichier, fenêtre du mot de passe qui propose d’abord de retirer la protection quand elle est active.
- **Fichier allégé** : commentaires et espaces inutiles retirés à la construction (sans toucher au code).
- **Raccourcis clavier** : liste avec la touche `?`, nouveaux raccourcis (`/`, `N`, `E`, `1`–`8`, `Maj+F`).
- **Mettre à jour en gardant mon arbre** : le bandeau de mise à jour peut télécharger la nouvelle version, y placer l’arbre ouvert et enregistrer le fichier.
- Téléchargement direct : le bandeau de mise à jour télécharge directement le nouveau fichier, et chaque release contient un fichier `arbora.html` au nom fixe pour un lien de téléchargement permanent. Page d’accueil du projet avec une démo en ligne.

### Corrections
- Détection des mises à jour : une nouvelle version pouvait passer inaperçue jusqu’à 24 heures, et le bandeau ne s’affichait qu’une fois. La version connue est maintenant mémorisée et affichée à chaque ouverture, la vérification se fait au plus une fois par heure, et une vérification en échec est retentée à l’ouverture suivante.
- Un fichier protégé ne garde plus de modifications non enregistrées dans le cache du navigateur.

## [1.1.0] - 2026-11-09

### Nouveautés
- Supprimer une personne ou une famille depuis la barre du haut, avec les conséquences expliquées avant de confirmer.
- Export d’une fiche en JSON (à importer dans un autre arbre, détails au choix) ou en PDF présenté proprement avec les informations personnalisées. Aussi depuis la fenêtre « Informations personnalisées ».
- Export d’une famille avec le niveau de détail voulu, et import intelligent qui reconnaît les personnes déjà présentes, les fusionne et rattache la famille au bon endroit.
- Historique des modifications gardé dans le fichier, annulation toujours possible après un enregistrement pendant la session, export du journal (texte, CSV, JSON).
- Outil de doublons (comparaison côte à côte, fusion champ par champ ou séparation) et outil de boucles (circuit complet, lien suspect, couper un lien ou séparer deux homonymes).
- Tous les exports portent le nom d’Arbora, sa version, son logo et le crédit.
- Suppression et export par nom de famille, avec options pour les conjoints, les enfants et toute la descendance.
- Fenêtre Exporter repensée en cartes regroupées par usage (tout l’arbre, image ou impression, une partie de l’arbre, autres formats).
- Fiche PDF sur une seule page, texte sélectionnable, « Arbora » en lien vers le projet, aperçu avant d’enregistrer.
- Outil des boucles : aperçu avant/après de la correction choisie (couper un lien parent-enfant, retirer une union, séparer deux homonymes), puis bouton de confirmation. Les boucles qui passent par une union sont maintenant prises en charge.
- Miniatures des images jointes dans la fiche.
- Photos de la vie : trois photos datées (enfance, milieu et fin de vie) au-dessus des événements, choisies dans les documents ou depuis un fichier, avec l’âge calculé tout seul. Reprises dans la fiche PDF, toujours sur une page.
- Images allégées à l’ajout : choix de la taille avec aperçu, poids réel avant/après et rappel qu’Arbora n’est pas un outil de stockage de photos. Un outil « Alléger les images… » (roue dentée) réduit les images déjà dans l’arbre.
- Photos des enfants, frères et sœurs, demi-frères et demi-sœurs dans la fiche.
- Photos de la vie : ordre par glisser-déposer (souris ou tactile), loupe et changement d’un clic en édition avec une pastille crayon, titre facultatif (proposé en grisé seulement), âge dans l’agrandissement.
- Liens web (photo de la fiche, photo de la vie, document) : Arbora propose d’enregistrer une copie dans le fichier pour la garder lisible hors ligne, explique pourquoi et affiche l’augmentation de taille estimée. Les sites qui bloquent la copie gardent seulement le lien, avec une explication.
- Les documents texte (TXT, Word, tableurs…) sont compressés automatiquement à l’ajout. Les PDF, images et ZIP sont déjà compressés et restent tels quels.
- Photos dans les vues (arbre, ascendance, descendance, éventail, frise) : photos seules, photos et icône vierge à la couleur du sexe pour les personnes sans photo, ou aucune, au choix dans la roue dentée.
- Lien web avec copie locale : le niveau de compression se choisit dans la même fenêtre (tailles d’image avec leur poids, ou compression sans perte pour les documents).
- Fil des fiches ouvertes au-dessus du nom quand on passe d’une fiche à l’autre par leurs liens (survol pour la liste complète), fermer une fiche ramène à la précédente.
- Aperçu avant d’enregistrer pour tous les exports PDF et image (arbre, vues, statistiques, PNG, SVG), et lien cliquable vers le projet GitHub dans le pied de tous les PDF.
- Outil des doublons pour des groupes de 2, 3, 4 fiches ou plus : fiches à réunir et fiche principale cochées, choix valeur par valeur, documents et résidences élément par élément, détails de chaque fiche, colonne « Après la fusion » en direct.
- Carte : bouton « Relocaliser tous les lieux… » avec explication (cas de « Montréal » placé aux États-Unis) et barre de progression.
- Rendu clair ou sombre pour tous les exports PDF et image, au choix dans l’aperçu, avec les couleurs du thème actif (modifiables dans la roue dentée › Thèmes de couleurs).
- En lecture, cliquer sur la photo de la fiche l’ouvre en grand.
- Export PDF pour les vues Ascendance, Descendance, Éventail et Frise.
- Rapport PDF des lieux depuis la Carte : chiffres clés, schéma des lieux (cercles selon le nombre de personnes, traits du lieu de naissance au lieu de décès), top des lieux et des pays, tableau complet avec les personnes de chaque lieu.
- Rapport de vérification en PDF, classé par type de remarque.
- « Vérifier les mises à jour » dans la roue dentée.
- Bouton « Offrir un café » (Ko-fi) à gauche de « Ajouter une personne » après 30 minutes d’utilisation, masquable et qui revient 30 minutes plus tard.
- Les images de plus de 1 Mo sont signalées : un bandeau propose de les alléger, et un bouton « Alléger » apparaît à côté du document ou dans le menu de la photo de la fiche.

### Changements
- Le bouton Enregistrer écrase le fichier ouvert une fois choisi dans la session, et propose un autre endroit si l’écriture échoue.
- Fiches : parents en cartes cliquables et fratrie en pastilles, en-tête réorganisé avec des boutons de même hauteur, retour à la fiche d’origine après « Nouvelle personne… » pour un parent ou un frère, parties vides affichées « Aucune information » en lecture.
- Âges affichés dans les vues Ascendance et Descendance.
- Les fenêtres adaptent leur largeur pour éviter le défilement et gardent le même écart sous la barre du haut et en bas. « Nouveautés » s’ouvre juste sous son bouton, le bandeau de soutien est sous le titre.
- Aide complétée avec les nouveautés, bouton « À propos d’Arbora » mis en avant, icône sur Aide, espacement régulier des boutons du haut.
- « Disposition auto » devient un bouton en bas à droite de l’arbre, à côté de + − Tout.
- Le centrage sur une personne (bouton cible, double clic) tient compte de la fiche et du journal ouverts.
- Les informations personnalisées listent tous les noms (plus de « et N autres ») et indiquent « inconnu » quand un âge manque.
- La localisation automatique des lieux n’alourdit plus le journal.
- Le journal est partagé en deux zones égales, chacune avec son défilement : session en cours (cache du navigateur) et historique du fichier.
- Fenêtre Exporter : tout l’arbre, puis une partie de l’arbre, puis image ou impression avec le choix de la vue sur la même ligne. Export draw.io retiré.
- Éventail : prénom et nom toujours affichés, à une taille adaptée à chaque secteur.
- Bouton « Ajouter une personne » avec une icône. En lecture, les notes prennent la hauteur de leur texte.
- Photo de la fiche : choix de la taille avec aperçu à l’import, et menu (fichier, lien web, documents, retirer) au clic en édition.
- Tuiles enfants, frères et sœurs et demi-frères et sœurs à la couleur du sexe comme les cartes des parents, sans le point de couleur, toujours avec photo ou avatar pour une hauteur identique.
- Les périodes des résidences s’affichent en entier.
- L’import et la fusion de doublons prennent en compte photos et documents : images et documents identiques reconnus par leur contenu et non dupliqués, photo de la fiche dans les écarts avec vignettes, la photo non gardée rejoint les documents, les photos de la vie complètent les emplacements libres.
- Documents identiques lors de la fusion de doublons ou de l’import : garder un seul exemplaire (recommandé) ou tout conserver. Les documents de même nom sont toujours renommés automatiquement (« acte (2).pdf »).
- Une fiche sans photo affiche une icône vierge dans son en-tête. Les icônes vierges des vues reprennent le style des petites tuiles de la fiche (fond clair, contour à la couleur du sexe).
- Une fiche en modification reste ouverte jusqu’à « Terminer » : un clic à côté, sur une autre case ou sur un lien ne la ferme pas et n’ouvre pas d’autre fiche.
- « C’est moi » devient un bouton étoile dans le style de la mise en évidence. Les boutons photo disparaissent de la fiche : la photo ou l’icône ouvre le menu.
- Outil des boucles : schéma en cercle avant / après, séparation montrée en deux branches, fenêtre qui reste ouverte (clic sur un nom pour ouvrir la fiche, l’outil se met à jour après chaque modification).
- Vue Descendance avec les mêmes cases que l’Ascendance (les conjoints ne sont plus tassés dans les cases). Frise : photos et icônes en colonne à droite des noms.
- L’historique des fiches est un bandeau séparé en haut de la fiche. Cliquer à côté ou sur une autre case alors qu’un historique existe propose de le fermer (puis ouvre la case choisie).
- « C’est moi » s’affiche en badge étoile jaune sur la photo de la fiche.
- En-tête : « Arbora » à côté du logo, une séparation, puis le nom de l’arbre, modifiable au survol. Le logo et le pied de page « Arbora 1.1.0 · Conçu par florentdoug » ouvrent « À propos d’Arbora ».
- Photo de la fiche dans le PDF découpée en forme vectorielle avec une bordure propre, ronde ou carrée au choix dans l’aperçu comme clair ou sombre. La visionneuse de photo passe à la taille réelle.
- Export des statistiques en deux cartes (PDF et PNG). Dans une fenêtre ouverte depuis Exporter, « Annuler » revient au menu Exporter, avec un bouton « Retour au menu Exporter ».
- Rapport des lieux en PDF : fond de carte avec continents et frontières (Natural Earth, domaine public).
- « Alléger les images » couvre aussi les photos des fiches et réencode les images lourdes même déjà petites en pixels.
- Le choix rond ou carré des photos s’applique à la fiche (photo, cartes, tuiles) et à tous les onglets (Ascendance, Descendance, Éventail, Frise).
- Unions et enfants : la photo (ou l’icône) du conjoint apparaît dans l’en-tête de chaque union et ouvre sa fiche.
- Documents de la fiche : une ligne par document (nom long tronqué, complet au survol), actions en icônes alignées et lisibles (mettre en avant, alléger, compresser, retirer). Une photo de la vie lourde affiche une pastille « alléger », et la visionneuse propose d’alléger une image lourde en bas de la fenêtre.

### Corrections
- Les résidences pouvaient être supprimées depuis une fiche en lecture.
- Un lieu avec son pays (par exemple « Montréal, Canada ») pouvait être placé dans le mauvais pays sur la carte.
- Un deuxième enregistrement pouvait télécharger une copie nommée « (1) » au lieu d’écraser le fichier.
- Un lieu dont le pays était ajouté ou changé après coup (« Montréal » puis « Montréal, Canada ») gardait son ancienne position, fausse.
- Certains boutons « Résoudre » des boucles ne faisaient rien.
- Les valeurs de la colonne de droite de l’outil de doublons n’étaient pas alignées.
- L’export JSON contenait encore les images retirées des fiches (elles ne sont gardées en mémoire que pour pouvoir annuler).
- L’historique du fichier ne défilait pas dans le journal.
- Cartes d’union : l’aide sur le divorce et « Exporter cette famille » n’étaient pas alignées.
- « Lien web… » de la photo de la fiche ouvrait l’analyse de lien au lieu de la fenêtre de lien.
- Outil des doublons : le bouton « Garder plutôt la fiche de droite » devient bien « Garder plutôt la fiche de gauche » après l’inversion, et chaque fiche reste dans sa colonne.
- « Nouvelle personne… » pour un enfant ou un conjoint créait une fiche nommée « Nouvel enfant » ou « Nouveau partenaire » : les champs sont maintenant vides et la nouvelle fiche s’ouvre en modification avec un retour.
- Aperçus de plusieurs pages (rapport de vérification, statistiques…) : le haut de la première page était coupé.
- Les boutons « Joindre un fichier » et « Ajouter un lien web » de la partie Documents étaient masqués en modification.

## [1.0.0] - 2026-11-08

Première version publique.

### Nouveautés
- Arbre interactif avec disposition automatique, groupes isolés signalés, mini-carte.
- Fiches en lecture par défaut avec bouton Modifier, informations personnalisées, unions numérotées par date de mariage, divorce.
- Vues ascendance, descendance, éventail, frise et carte, toutes filtrables.
- Statistiques avec « Le saviez-vous ? » qui suit le filtre choisi.
- Vérifications : dates impossibles, boucles généalogiques, doublons, formats, sources de recherche par pays.
- Analyse de lien de parenté entre deux personnes.
- Film de famille (une personne, un nom, tout l’arbre) avec anecdotes, exportable en MP4 ou WebM.
- Import GEDCOM et JSON avec fusion des doublons, reprise des données d’une ancienne copie.
- Exports PDF, image, GEDCOM, JSON, draw.io et copie de l’outil (modifiable ou en lecture seule).
- Consignes IA : correction de l’arbre, recherche encadrée d’ancêtres, démarrage de zéro.
- Vérification des mises à jour (désactivable).
- Six langues, thèmes clair et sombre.
