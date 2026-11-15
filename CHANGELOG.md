# Changelog / Journal des versions

**English** · [Français](#français)

All notable changes to Arbora. Version numbers follow major.minor.patch: a new feature bumps the second number, a fix bumps the third.

## [1.5.0] - 2026-11-15

### Added
- **Residences with start and end years**: two 4-digit year fields per residence, an optional « Detail » kept from old entries, and a « Sort by date » button (from oldest to most recent, still adjustable by hand afterwards).
- **Checks: old residence periods converted** (« 2007-2012 » becomes start 2007, end 2012), one by one or all at once. Details such as an address or a month are kept, approximate periods are flagged.
- **AI: research the history of a surname**: origin, variants, geographic spread, bearers already in the tree and archive leads, each fact with its source. Leads come back into « Research to do ».
- **AI: advice on each assistant's deep research mode** and an explanation of the sources it consults, valid worldwide, with their limits.
- **Gallery**: click an image for a preview, with « Open full size in a new tab ». Click the name to open the record.
- **After « Update and keep my tree »**: a window explains that the tree moved to the new version, with « Close the tool », « Redo the update » and « Close this message ».

### Changed
- **Checks redesigned**: tree health first, « My research to do » folded just below, « Quick wins » with 3 one-click fixes, coloured tiles per category with a progress bar, congratulations when a category is done, international sources first.
- **Export redesigned like Import**: first choose the type (a view of the tool, documents and reports, save the data, share), then the options. The views follow the order of the tabs. Contact sheet, places report and checks report are always available.
- **Smoother mouse wheel zoom** on the tree (wheel steps grouped per frame), and the **Map opens faster** (the person list is built on first use).
- **Guided tour fully redone for beginners**: header, every tab, the tree, the record, saving and help, in 33 short steps.
- **New welcome screen**: Arbora logo at the top and a glowing « Discover the tool in 2 minutes » button.
- Looping animations above the tree have been stopped.
- **Contact sheet**: full names under each picture, on two lines if needed.
- **Update and keep my tree**: the suggested file name follows the save format (Arbora_tree name_DD-MM-YYYY_HH-MM.html), and the window explains that the browser cannot close the old version or open the new one by itself.
- **AI instructions**: residences with start and end years, sources named generically for every country.
- Browser tab title: « Arbora | tree name ».

### Fixed
- The « changes only kept in this browser » reminder now disappears as soon as the file is saved.
- Checks no longer suggest a « correction » identical to the current value.

## [1.4.0] - 2026-11-15

### Added
- **Reorder residences**: in edit mode, each residence has a handle to drag it into place, plus up and down arrows (handy on phones). The life journey, the map and the distance travelled follow this order, and the move can be undone.
- **One person's journey on the map**: pick a person in the new field above the map to see only their journey, with numbered steps (birth, baptism, residences, journey, marriages, death) and the map framed on it.
- **Sosa numbering can be hidden everywhere**: Settings, Display, « Sosa numbering ». It hides the numbers in records, ancestors, hourglass, record PDF and family book.
- **d’Aboville numbering can be hidden everywhere**, like Sosa (Settings, Display).
- **Record header**: the name now sits at the top in place of « Record », with the current age below (or « Died aged … » with the years).
- **Guided switch to the new file after an update**: on Chrome, Edge and Brave, the current file can be replaced directly (no duplicate, then « Reload now »). Otherwise a window explains the 3 steps with the exact file name. The new file welcomes you on first opening, and an old copy warns that a newer file exists.

### Changed
- **About redesigned**, wider: version status (« Up to date », « Not checked yet » or « New version available ») on the same line as « Check », « Discover Arbora » (presentation page) and a glowing « Support Arbora » card side by side (« Buy the creator a coffee »), « Why Arbora » folded into a single line. The direct download button is replaced by the presentation page.
- **Settings redesigned**: three columns (File and tree tools, Display, Help and maintenance) with an icon in front of each entry and each display option.
- **Map**: « Life journeys » is now a clearly visible switch with a route icon, aligned with the rest, and the person field looks like the main search. The chosen person's journey is drawn in gold (like the highlighted person) and the other bubbles are hidden.
- **Gallery**: the same « Show » filter as the other views, plus a person's ancestors or descendants.
- **PDF exports**: larger « Arbora » header with the logo in colour at the top left of every page.
- **AI instructions updated** (improve and start with an AI, 6 languages): they now describe the fields added since 1.0 (life journey, witnesses and godparents, structured and cited sources, research to do, adoption and foster links, life photos) and what the AI must never change. Research leads go into « Research to do » instead of the notes.
- **Defaults**: round and large photos in the boxes, small tree text. Settings already chosen are kept.
- **Record**: the Sex field has its icon, like the other fields.

### Fixed
- Gallery: the list now scrolls when the images go beyond the window.
- About: the « Download the latest version » button was hard to read in light mode (removed, see above).
- Gallery: the chosen branch did not stay displayed in its list after selection.

## [1.3.0] - 2026-11-13

### Added
- **Hourglass view**: the ancestors on the left and the descendants on the right of one person, with the same boxes, zoom and exports (PDF, PNG, SVG) as the Ancestors and Descendants views.
- **Gallery**: all the photos (record photos, life photos) and documents of the tree in one view, filtered by type, by name and by branch (whole tree, ancestors or descendants of the selected person). A click opens the person's record, the magnifier shows the image or opens the document.
- **Witnesses and godparents**: people linked to a birth, baptism, death or marriage (witness, godfather, godmother, informant, officiant). They are shown in both records, kept when merging duplicates, removed when the person is deleted, printed in the record PDF and exported to GEDCOM (ASSO).
- **Typed parent links**: adoption or foster family, chosen in the Parents section, drawn as a dotted line in the tree (with a legend entry), shown on the parent and child cards, in the record PDF and in GEDCOM (PEDI, import and export).
- **« Today in the family »**: on opening, a discreet reminder of today's birthdays and anniversaries and of the coming week, once a day. It can be turned off (and back on from the family calendar).
- Keyboard shortcuts `1` to `9` and `0` for the ten views.
- **Search across all content**: the search box now also looks in notes, sources, life journey, residences, baptism, marriages, research to do and document names, and shows the matching excerpt under the name.
- **Favourites**: a bookmark next to « Record » marks a record, a button near the search box (and an entry in the gear menu) lists the favourites. They are saved in the file.
- **CSV table import**: one line per person (names, sex, birth, death, places, occupation, notes) with father, mother and spouse columns to link the lines. Column names are recognised in the 6 languages, a template can be downloaded, and the import goes through the usual analysis with duplicate detection.
- **French Republican calendar**: a date such as « 18 brumaire an VIII » typed in a date field is converted to the Gregorian date, and the Republican equivalent is shown under dates between 22 September 1792 and 31 December 1805. Also accepted in the CSV import.
- **Historical landmarks** in the life journey, as an option (world wars, 1929 crash, first steps on the Moon…), with the person's age at each one.
- **Gallery contact sheet as PDF**: the filtered gallery on A4 pages, 4 tiles per row, with names and captions.
- **Hourglass**: Sosa numbers in the ancestor boxes and the « Sosa » button, as in the Ancestors view.
- **Family book**: witnesses, godparents and the parent link type (adoption, foster) are printed in each entry.
- **GEDCOM**: witnesses and godparents are read back on import (ASSO), and marriage witnesses are exported.
- About: a « Check for updates » button next to the download button.
- **Statistics**: a new « Records and curiosities » chapter (largest sibling group, longest union, old age, most common occupations, great travellers with distances, distance travelled between all known places, twins, wedding months), and a « Portrait of the group » that adapts to each filter: first known bearer and cradle for a surname or a branch, life milestones, infant mortality, causes and decades of death for a century, a generation, a sex or a status, relatives counts for a person.
- **Hourglass**: d’Aboville numbering of descendants (1.2 is the 2nd child, 1.2.1 their first child), mirroring the Sosa numbers of ancestors.
- **Checks that guide you**: clicking a name opens the record with a banner « Remark 3 of 40 » and the buttons Fix (opens the right field in edit mode), Previous and Next; a « Why? » under each remark explains it in plain words; a remark can be ignored with a reason and restored at the bottom of the tab; the tree health score keeps its history, with the change since last week and a small curve.
- **New checks**: baptism before birth, residence or life event outside the person's life, witness or godparent not alive at the event, two living children with the same first name, birth more than 10 months after the father's death (full dates), and **places to harmonise** (the same place written in several ways, fixed in one click).
- **Record PDF layouts**: Classic, Banner (full-width coloured header) or Cards (each part in a card on a tinted background), chosen in the preview next to light/dark, photo shape and life journey. The header is as high as the photo, with the text block and the photo centred vertically and the Sosa number next to « Record ».
- **Customisable record PDF**: in the preview, an « Appearance » row (8 colour palettes or your own theme, layout, light or dark, modern or classic serif font) and a « Content » row (photo round, square or none, life photos, life journey, Sosa number, and the parts Family, Witnesses, Notes and sources, Personal facts). Choices are remembered and the record always fits on one page.
- **Import**: before choosing the file, two clear cards « Merge with my tree » and « Replace my tree », with an explanation; the chosen mode is shown at the top of the import window and preselected in the analysis.
- **Example tree**: on the welcome screen, « Try with an example tree » opens a small fictional family (15 people) to test everything. Nothing is saved, a banner offers « Start my tree » or « Leave the example ».
- **Field icons** in the record, in read and edit mode, to find each piece of information at a glance.
- **Life photos in the record PDF** are linked by arrows to show the evolution, and the space for captions is only reserved when there is one.
- **Lighten images**: real preview on the largest image of each group (before and after at the same scale, detail at 100 % or whole image, with dimensions and weight), updated at every size or quality change, and a clear note on what is never changed (non-image documents, web-linked images, GIF and SVG, images already smaller than the chosen size)). You can pick the image to preview, move around in it, and see the sending limits (Outlook, Gmail, Yahoo, Proton Mail attachments with encoding included, Discord) turn from a red cross to a green tick.
- **Map**: « Relocate all places » becomes « Refresh all places » and looks up several places at once (much faster), skipping places already up to date unless asked. A « Locate the N places » button above the places to locate replaces clicking « Search » then « Confirm » for each one. The example tree opens with its places already on the map.

### Changed
- The tab bar stays on one line on common screen widths: the save status is shortened instead of wrapping.
- Phones: the save button is an icon (a disk when there are changes, a tick when everything is saved) instead of a shortened label.
- **Record panel**: all parts share the same foldable title and left edge (life journey, witnesses, sources, research to do, documents), spacing is tighter in edit and read mode, residences are shown as text with the period aligned right, and the header shows « Record » above the name with one row of chips (Sosa, favourite, personal information).
- **Checks**: tree health takes 2/3 of the width and « Where to search » 1/3, and both appear at the same time.
- **File half the size** (about 1 MB instead of 2.1 MB for 1.2.0): the code is minified and stored compressed (lossless, checked byte for byte at each build), with a small embedded decompressor (fflate, MIT licence). Nothing is removed from the tool.
- Exporting a record now offers PDF first and by default.
- Closing a record that is being edited asks whether to save the changes, discard them or go back to the record.
- The credit band of exported images (SVG and PNG) is centred, in the colours of the chosen look, with the logo next to the text; the second credit drawn inside the image is gone.
- Statistics tiles have their own colour and icon, and « Group members » shows one line per person.
- Record in read mode: birth, baptism and death are compact tiles that are always visible; baptism and death only appear when there is information, and the death tile no longer shows the « Deceased » box (« Deceased (date unknown) » when there is no date). The life journey uses the same icons and colours for these three events.
- Lightening images: the weight shown is the real weight in the file, photos (record and life photos) and documents are handled separately (1,024 px and 1,600 px by default), with a choice of size and quality, and an explanation when a size brings no gain.
- « Save the blank tool » suggests the name Arbora_1.3.0.html.

### Fixed
- Record PDF: the « Photo: round or square » choice had disappeared from the preview in 1.2.0.
- Mobile: the page no longer overflows sideways by a few pixels in languages with a long « Saved » label.
- Build: the build now refuses to complete when two modules declare the same internal name (the cause of both regressions found in 1.2.0), and a single command runs all test suites, including the minified file.
- Map: switching quickly from the Map tab to another tab could show the error « Cannot read properties of undefined (reading '_leaflet_pos') ».
- Exported views could keep boxes half transparent when the export was started while the view was still appearing.

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

## [1.5.0] - 2026-11-15

### Ajouts
- **Résidences avec année de début et de fin** : deux champs d’année sur 4 chiffres par résidence, une « Précision » facultative gardée depuis les anciennes saisies, et un bouton « Trier par date » (de la plus ancienne à la plus récente, ajustable à la main ensuite).
- **Vérifications : conversion des anciennes périodes de résidence** (« 2007-2012 » devient début 2007, fin 2012), une par une ou toutes d’un coup. Les précisions comme une adresse ou un mois sont gardées, les périodes approximatives sont signalées.
- **IA : rechercher l’histoire d’un nom de famille** : origine, variantes, répartition géographique, porteurs déjà dans l’arbre et pistes d’archives, chaque fait avec sa source. Les pistes reviennent dans « Recherches à faire ».
- **IA : conseil sur le mode de recherche approfondie** de chaque assistant, et explication des sources consultées, valable dans le monde entier, avec leurs limites.
- **Galerie** : clic sur une image pour l’aperçu, avec « Ouvrir en taille réelle dans un nouvel onglet ». Clic sur le nom pour ouvrir la fiche.
- **Après « Mettre à jour en gardant mon arbre »** : une fenêtre explique que l’arbre est passé à la nouvelle version, avec « Fermer l’outil », « Refaire la mise à jour » et « Fermer ce message ».

### Changements
- **Vérifications remaniées** : santé de l’arbre en premier, « Mes recherches à faire » repliées juste en dessous, « Petites victoires » avec 3 corrections en un clic, tuiles colorées par catégorie avec barre de progression, félicitations quand une catégorie est terminée, sources internationales en premier.
- **Exporter repensé comme Importer** : on choisit d’abord le type (une vue de l’outil, documents et rapports, sauvegarder les données, partager), puis les options. Les vues suivent l’ordre des onglets. Planche contact, rapport des lieux et rapport de vérification toujours disponibles.
- **Zoom à la molette plus fluide** sur l’arbre (crans regroupés par image), et **Carte plus rapide à s’ouvrir** (la liste des personnes est calculée au premier usage).
- **Visite guidée entièrement refaite pour les débutants** : en-tête, chaque onglet, l’arbre, la fiche, l’enregistrement et l’aide, en 33 étapes courtes.
- **Nouvel écran d’accueil** : logo Arbora en tête et un bouton lumineux « Découvrir l’outil en 2 minutes ».
- Les animations en boucle au-dessus de l’arbre ont été arrêtées.
- **Planche contact** : nom complet sous chaque image, sur deux lignes si besoin.
- **Mettre à jour en gardant mon arbre** : le nom proposé suit le format d’enregistrement (Arbora_nom de l’arbre_JJ-MM-AAAA_HH-MM.html), et la fenêtre explique que le navigateur ne peut pas fermer l’ancienne version ni ouvrir la nouvelle tout seul.
- **Consignes IA** : résidences avec année de début et de fin, sources citées de façon générique pour tous les pays.
- Titre de l’onglet du navigateur : « Arbora | nom de l’arbre ».

### Corrections
- Le rappel « modifications gardées seulement dans ce navigateur » disparaît dès que le fichier est enregistré.
- Les vérifications ne proposent plus de « correction » identique à la valeur actuelle.

## [1.4.0] - 2026-11-15

### Ajouts
- **Réordonner les résidences** : en mode modification, chaque résidence a une poignée pour la glisser à sa place, et des flèches monter et descendre (pratiques sur téléphone). Le parcours de vie, la carte et les kilomètres parcourus suivent cet ordre, et le déplacement peut être annulé.
- **Parcours d’une personne sur la carte** : choisis une personne dans le nouveau champ au-dessus de la carte pour ne voir que son parcours, avec les étapes numérotées (naissance, baptême, résidences, parcours, mariages, décès) et la carte cadrée dessus.
- **Numérotation Sosa désactivable partout** : Paramètres, Affichage, « Numérotation Sosa ». Les numéros disparaissent des fiches, de l’ascendance, du sablier, de la fiche PDF et du livre de famille.
- **Numérotation d’Aboville désactivable partout**, comme le Sosa (Paramètres, Affichage).
- **En-tête de fiche** : le nom remonte à la place de « Fiche », avec l’âge actuel en dessous (ou « Décédé à … » avec les années).
- **Passage guidé vers le nouveau fichier après une mise à jour** : sur Chrome, Edge et Brave, le fichier actuel peut être remplacé directement (pas de doublon, puis « Recharger maintenant »). Sinon, une fenêtre explique les 3 étapes avec le nom exact du fichier. Le nouveau fichier souhaite la bienvenue à sa première ouverture, et une ancienne copie signale qu’un fichier plus récent existe.

### Changements
- **À propos remanié**, plus large : état de la version (« À jour », « Pas encore vérifiée » ou « Nouvelle version disponible ») sur la même ligne que « Vérifier », tuiles « Découvrir Arbora » (page de présentation) et « Soutenir Arbora » qui brille, côte à côte (« Offre un café au créateur »), « Pourquoi Arbora » replié sur une ligne. Le bouton de téléchargement direct est remplacé par la page de présentation.
- **Paramètres remaniés** : trois colonnes (Fichier et outils de l’arbre, Affichage, Aide et maintenance), avec une icône devant chaque entrée et chaque option d’affichage.
- **Carte** : « Parcours de vie » devient un interrupteur bien visible avec une icône de trajet, aligné avec le reste, et le champ de personne reprend le style de la recherche principale. Le parcours de la personne choisie est tracé en or (comme la personne mise en évidence) et les autres bulles sont masquées.
- **Galerie** : le même filtre « Afficher » que les autres vues, avec en plus les ancêtres ou les descendants d’une personne.
- **Exports PDF** : en-tête « Arbora » avec le logo en couleur et plus grand, en haut à gauche de chaque page.
- **Consignes IA mises à jour** (améliorer et démarrer avec une IA, 6 langues) : elles décrivent les champs ajoutés depuis la 1.0 (parcours de vie, témoins, parrains et marraines, sources structurées et citées, recherches à faire, adoption et accueil, photos de la vie) et ce que l’IA ne doit jamais modifier. Les pistes de recherche vont dans « Recherches à faire » au lieu des notes.
- **Réglages par défaut** : photos rondes et grandes dans les cases, texte de l’arbre petit. Les réglages déjà choisis sont conservés.
- **Fiche** : le champ Sexe a son icône, comme les autres champs.

### Corrections
- Galerie : la liste défile maintenant quand les images dépassent la fenêtre.
- À propos : le bouton « Télécharger la dernière version » était peu lisible en mode clair (retiré, voir plus haut).
- Galerie : la branche choisie ne restait pas affichée dans sa liste après la sélection.

## [1.3.0] - 2026-11-13

### Nouveautés
- **Vue Sablier** : les ancêtres à gauche et les descendants à droite d’une même personne, avec les mêmes cases, le même zoom et les mêmes exports (PDF, PNG, SVG) que les vues Ascendance et Descendance.
- **Galerie** : toutes les photos (photos de fiche, photos de la vie) et tous les documents de l’arbre dans une vue, filtrables par type, par nom et par branche (tout l’arbre, ascendance ou descendance de la personne sélectionnée). Un clic ouvre la fiche de la personne, la loupe affiche l’image ou ouvre le document.
- **Témoins, parrains et marraines** : des personnes liées à une naissance, un baptême, un décès ou un mariage (témoin, parrain, marraine, déclarant, officiant). Elles apparaissent dans les deux fiches, sont conservées à la fusion de doublons, retirées si la personne est supprimée, imprimées dans la fiche PDF et exportées en GEDCOM (ASSO).
- **Filiation typée** : adoption ou famille d’accueil, à choisir dans la partie Parents, dessinée en pointillés dans l’arbre (avec une entrée de légende), affichée sur les cartes des parents et des enfants, dans la fiche PDF et en GEDCOM (PEDI, import et export).
- **« Aujourd’hui dans la famille »** : à l’ouverture, un rappel discret des anniversaires du jour et de la semaine à venir, une fois par jour. Il se désactive (et se réactive depuis le calendrier de la famille).
- Raccourcis clavier `1` à `9` et `0` pour les dix vues.
- **Recherche dans tout le contenu** : la barre de recherche regarde aussi les notes, les sources, le parcours de vie, les résidences, le baptême, les mariages, les recherches à faire et les noms des documents, et affiche l’extrait trouvé sous le nom.
- **Favoris** : un signet à côté de « Fiche » marque une fiche, un bouton près de la recherche (et une entrée du menu engrenage) liste les favoris. Ils sont enregistrés dans le fichier.
- **Import d’un tableau CSV** : une ligne par personne (noms, sexe, naissance, décès, lieux, profession, notes) avec des colonnes père, mère et conjoint pour relier les lignes. Les noms de colonnes sont reconnus dans les 6 langues, un modèle se télécharge, et l’import passe par l’analyse habituelle avec repérage des doublons.
- **Calendrier républicain** : une date comme « 18 brumaire an VIII » saisie dans un champ de date est convertie en date grégorienne, et l’équivalent républicain s’affiche sous les dates comprises entre le 22 septembre 1792 et le 31 décembre 1805. Accepté aussi dans l’import CSV.
- **Repères historiques** dans le parcours de vie, au choix (guerres mondiales, krach de 1929, premiers pas sur la Lune…), avec l’âge de la personne à chacun.
- **Planche contact de la galerie en PDF** : la galerie filtrée sur des pages A4, 4 vignettes par ligne, avec noms et légendes.
- **Sablier** : numéros Sosa dans les cases des ancêtres et bouton « Sosa », comme dans la vue Ascendance.
- **Livre de famille** : les témoins, parrains, marraines et le type de filiation (adoption, accueil) sont imprimés dans chaque notice.
- **GEDCOM** : les témoins, parrains et marraines sont relus à l’import (ASSO), et les témoins de mariage sont exportés.
- À propos : un bouton « Vérifier les mises à jour » à côté du bouton de téléchargement.
- **Statistiques** : nouveau chapitre « Records et curiosités » (plus grande fratrie, plus longue union, grand âge, métiers les plus fréquents, grands voyageurs avec les distances, kilomètres parcourus entre tous les lieux connus, jumeaux, mois des mariages), et un « Portrait du groupe » qui s’adapte à chaque filtre : premier porteur connu et berceau pour un nom ou une branche, âges de la vie, mortalité infantile, causes et décennies des décès pour un siècle, une génération, un sexe ou un statut, nombre de proches pour une personne.
- **Sablier** : numérotation d’Aboville des descendants (1.2 est le 2e enfant, 1.2.1 son premier enfant), en miroir des numéros Sosa des ancêtres.
- **Des vérifications qui guident** : cliquer sur un nom ouvre la fiche avec un bandeau « Remarque 3 sur 40 » et les boutons Corriger (ouvre le bon champ en modification), Précédente et Suivante ; un « Pourquoi ? » sous chaque remarque l’explique simplement ; une remarque peut être ignorée avec une raison et rétablie en bas de l’onglet ; le score de santé de l’arbre garde son historique, avec l’évolution depuis la semaine précédente et une petite courbe.
- **Nouveaux contrôles** : baptême avant la naissance, résidence ou événement hors de la vie de la personne, témoin ou parrain qui n’est pas en vie à l’événement, deux enfants vivants du même prénom, naissance plus de 10 mois après le décès du père (dates complètes), et **lieux à harmoniser** (le même lieu écrit de plusieurs façons, corrigé en un clic).
- **Mises en page de la fiche PDF** : Classique, Bandeau (en-tête de couleur pleine largeur) ou Carnet (chaque partie dans une carte sur fond teinté), au choix dans l’aperçu, à côté du rendu clair ou sombre, de la forme de la photo et du parcours de vie. L’en-tête a la hauteur de la photo, avec le texte et la photo centrés verticalement et le numéro Sosa à côté de « Fiche ».
- **Fiche PDF personnalisable** : dans l’aperçu, une ligne « Apparence » (8 palettes de couleurs ou ton propre thème, mise en page, clair ou sombre, police moderne ou classique avec empattement) et une ligne « Contenu » (photo ronde, carrée ou aucune, photos de la vie, parcours de vie, numéro Sosa, et les parties Famille, Témoins, Notes et sources, Informations personnalisées). Les choix sont mémorisés et la fiche tient toujours sur une page.
- **Importer** : avant de choisir le fichier, deux cartes claires « Fusionner avec mon arbre » et « Remplacer mon arbre », avec une explication ; le mode choisi s’affiche en haut de la fenêtre d’import et il est présélectionné dans l’analyse.
- **Arbre d’exemple** : sur l’écran d’accueil, « Essayer avec un arbre d’exemple » ouvre une petite famille fictive (15 personnes) pour tout tester. Rien n’est enregistré, un bandeau propose « Commencer mon arbre » ou « Quitter l’exemple ».
- **Icônes des champs** dans la fiche, en lecture comme en modification, pour repérer chaque information d’un coup d’œil.
- **Photos de la vie dans la fiche PDF** reliées par des flèches pour montrer l’évolution, et l’espace des légendes n’est réservé que s’il y en a.
- **Alléger les images** : aperçu réel sur la plus grande image de chaque groupe (avant et après à la même échelle, détail à 100 % ou image entière, avec dimensions et poids), mis à jour à chaque changement de taille ou de qualité, et une note claire sur ce qui n’est jamais modifié (documents qui ne sont pas des images, images en lien web, GIF et SVG, images déjà plus petites que la taille choisie)). On peut choisir l’image à prévisualiser, se déplacer dedans, et voir les limites d’envoi (pièces jointes Outlook, Gmail, Yahoo, Proton Mail encodage compris, Discord) passer de la croix rouge à la coche verte.
- **Carte** : « Relocaliser tous les lieux » devient « Actualiser tous les lieux » et cherche plusieurs lieux en même temps (beaucoup plus rapide), en sautant les lieux déjà à jour sauf demande. Un bouton « Localiser les N lieux » au-dessus des lieux à localiser remplace « Chercher » puis « Valider » pour chacun. L’arbre d’exemple s’ouvre avec ses lieux déjà sur la carte.

### Changements
- La barre d’onglets reste sur une ligne sur les largeurs d’écran courantes : l’état d’enregistrement est raccourci au lieu de passer à la ligne.
- Téléphone : le bouton d’enregistrement est une icône (une disquette quand il y a des modifications, une coche quand tout est enregistré) au lieu d’un libellé tronqué.
- **Fiche** : toutes les parties partagent le même titre repliable et le même bord gauche (parcours de vie, témoins, sources, recherches à faire, documents), les espacements sont resserrés en modification et en lecture, les résidences s’affichent en texte avec la période alignée à droite, et l’en-tête montre « Fiche » au-dessus du nom avec une rangée de pastilles (Sosa, favori, informations personnalisées).
- **Vérifications** : la santé de l’arbre occupe 2/3 de la largeur et « Où chercher » 1/3, et les deux apparaissent en même temps.
- **Fichier deux fois plus léger** (environ 1 Mo au lieu de 2,1 Mo pour la 1.2.0) : le code est minifié et stocké compressé (sans perte, vérifié octet par octet à chaque construction), avec un petit décompresseur intégré (fflate, licence MIT). Rien n’est retiré de l’outil.
- Exporter une fiche propose maintenant le PDF en premier et par défaut.
- Fermer une fiche en cours de modification demande s’il faut enregistrer les modifications, les ignorer ou revenir à la fiche.
- Le bandeau de crédit des images exportées (SVG et PNG) est centré, aux couleurs du rendu choisi, avec le logo collé au texte ; le second crédit dessiné dans l’image a disparu.
- Les tuiles de statistiques ont chacune leur couleur et leur icône, et « Membres du groupe » tient sur une ligne par personne.
- Fiche en lecture : naissance, baptême et décès sont des tuiles compactes toujours visibles ; baptême et décès n’apparaissent que s’il y a une information, et la tuile Décès n’affiche plus la case « Décédé » (« Décédé (date inconnue) » s’il n’y a pas de date). Le parcours de vie reprend les mêmes icônes et couleurs pour ces trois événements.
- Alléger les images : le poids affiché est le poids réel dans le fichier, les photos (de fiche et de la vie) et les documents sont traités à part (1 024 px et 1 600 px par défaut), avec le choix de la taille et de la qualité, et une explication quand une taille ne fait rien gagner.
- « Enregistrer l’outil vierge » propose le nom Arbora_1.3.0.html.

### Corrections
- Fiche PDF : le choix « Photo : ronde ou carrée » avait disparu de l’aperçu dans la 1.2.0.
- Mobile : la page ne déborde plus de quelques pixels sur le côté dans les langues où « Enregistré » est long.
- Construction : elle refuse désormais d’aboutir si deux modules déclarent le même nom interne (la cause des deux régressions trouvées dans la 1.2.0), et une seule commande lance toutes les suites de tests, fichier minifié compris.
- Carte : passer vite de l’onglet Carte à un autre onglet pouvait afficher l’erreur « Cannot read properties of undefined (reading '_leaflet_pos') ».
- Une vue exportée pendant son animation d’apparition pouvait garder des cases à moitié transparentes.

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
