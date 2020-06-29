# StarWarsFFG

Ceci est une implémentation du jeu de rôle  [Star Wars de Fantasy Flight Games](http://www.fantasyflightgames.fr/jeux/collection/star_wars_aux_confins_de_lempire/) pour le programme [Foundry Virtual Tabletop](https://foundryvtt.com/).

Pour le support de ce systeme de jeu : Discord [The Foundry](https://discord.gg/bNyxuk9) #starwars-ffg
Pour le support de la communauté Francaise : Discord [La Fonderie](https://discord.gg/pPSDNJk) #starwars-ffg
Lire ce document dans une autre langue : [English](https://github.com/StarWarsFoundryVTT/StarWarsFFG/blob/master/README.md)

# Prérequis

Ce système a besoin du module [Special Dice Roller](https://foundry-vtt-community.github.io/wiki/Community-Modules/#special-dice-roller) pour lancer les dés et évaluer les résultats.
Ce module est disponible dans la bibliothèque de modules intégré au logiciel. Après l'avoir installé, vous aurez besoin de l'activer dans le monde. [GitHub](https://github.com/BernhardPosselt/foundryvtt-special-dice-roller)

# Installation

## Installation du système de jeu Star Wars FFG

1. Lancer Foundry VTT
2. Aller dans la tabulation "Systèmes de Jeu"
3. Cliquer sur le bouton "Installer un Système de jeu"
4. Copier le lien suivant dans le champ "URL du Manifest":
   https://raw.githubusercontent.com/StarWarsFoundryVTT/StarWarsFFG/master/system.json
5. Cliquer sur Installation, après quelques secondes le système devrait être installé.
6. Installer (si ce n'est pas déja fait) le module "Special Dice Roller", voir en-dessous pour les détails.

## Installation du module "Special Dice Roller"

1. Aller dans la tabualtion "Modules"
2. Cliquer sur le bouton "Installer un Module"
3. Dans le champ de recherche, taper "Special"
4. Appuyer sur le bouton "Installation" pour le module "Special Dice Roller".

# Contribuer

Veuillez consulter [CONTRIBUTING.md](https://github.com/StarWarsFoundryVTT/StarWarsFFG/blob/dev/CONTRIBUTING.md).

# A Faire

Voyez nos objectifs de productions et nos progés [ici](https://github.com/StarWarsFoundryVTT/StarWarsFFG/projects/1).

# Journal des modifications

- 24/06/2020 - Esrin - Correction de bug #160 & #159 - Limité l'utilisation des feuilles de personnages Adversaires aux acteurs de type "character".
- 24/06/2020 - Esrin - Correction de bug #161 - Intégré la vérification qu'une armure est portée pour le calcul de l'encombrance.
- 23/06/2020 - Cstadther - Correction de bug # 154 - Rajouté la différenciation de types de dégats pour les armes de mélée (Dégâts rajoutés) Intégré ces modifications dans le calcul des dégâts de l'arme (en complément de la vigeur).
- 23/06/2020 - Cstadther - Correction de bug # 155 partie 2 - Rajouté des attributs dans le template.json structure pour les pouvoirs de force et les specializations
- 23/06/2020 - Cstadther - Correction de bug # 155 - Les talents de force du compendium n'ont pas de champ d'attributes jusqu'à ce qu'ils soient importés dans le monde depuis le compendium.
- 23/06/2020 - Cstadther - Correction de bug # 152 - Taille des silhouette des vaisseaux.
- 22/06/2020 - Cstadther - Rajouta une option pour désactiver le calcul automatique de l'encaissement.
- 22/06/2020 - Cstadther - Amélioration - Gestion des erreurs a l'import des datas, et import asyncrhone.
- 21/06/2020 - Cstadther - Rajout de l'import des armures.
- 21/06/2020 - Cstadther - Rajout de l'import des armes.
- 21/06/2020 - Cstadther - Rajouta la mise a jour des items présent dans le compendium, de façon à ce que l'import puisse mettre aà jour correctement.
- 21/06/2020 - Cstadther - Intégra l'import de l'équipement, correction de bug avec la version 0.6.3 lié au changement de structure des compendiums.
- 21/06/2020 - Esrin - Retravailla le comportement du HUD pour que les fonctionalités core marchent avec la gestion des seuils de blessur et de stress de FFG.
- 21/06/2020 - Cstadther - Intégra le coût d'améliorations aux fiches de pouvoir de force.
- 21/06/2020 - Cstadther - Mise à jour Import de pouvoir de force - Suppression des rangées inutiles pour les pouvoirs de force qui ne les utilisent pas (ex. Soin/Blessure)
- 21/06/2020 - Cstadther - Correction de bug #126 - Cliquer sur un journal integre (dans une autre page) déclenche maintenant l'editeur aussi.
- 21/06/2020 - Cstadther - Correction de bug #138 - Fix CSS pour les connecteurs dans les spécialisations.
- 20/06/2020 - Cstadther - Intégra la gestion des symboles de OggDude pour améliorer le texte importé.
- 20/06/2020 - Cstadther - Rajoute l'import des pouvoirs de force depuis OggDude.
- 20/06/2020 - Cstadther - Correction de bug - Variable mal nomée dans l'importer.
- 19/06/2020 - Cstadther - Correction de bug #123 - Intégra la valeur localisée dans le dialogue de changement de caractéristiques.
- 19/06/2020 - Cstadther - Correction de bug pour l'erreure consle quand l'index du pack n'avait pas encore été généré.
- 19/06/2020 - Cstadther - Correction de bug pour les rangs de talents qui ne se cumulait pas correctement.
- 18/06/2020 - Cstadther - Première passe a l'Import des Talents depuis les données de OggDude.
- 17/06/2020 - Cstadther - Rajouta une case "Talent de Force" aux talents, intégration dans les feuilles de spécialisation.
- 17/06/2020 - Cstadther - Création feuille des Adversaires qui cache tout pour les non-owner sauf l'image, le nom et l'espèce. Le nom est dans le titre du Dialogue et ne peut pas facilement être changé.
- 17/06/2020 - Esrin - Localisation de tout les paramêtres systèmes.
- 17/06/2020 - Esrin - Rajouta un nouveau mode pour lister les joueurs dans le gestionnaire de groupes pour les gens qui partagent une session.
- 17/06/2020 - Esrin - Intégra l'option 'équipé' dans la partie des armures de l'inventaire du personnage. Seul l'armuer équipée appliquera sa valeur d'encaissement.
- 17/06/2020 - Cstadther - Correction de bug - Largeur du dialogue de séléction des caractéristiques.
- 17/06/2020 - Cstadther - Correction de bug #60 - Localization des dés.
- 17/06/2020 - Cstadther - Correction de bug #60 - Localization des dés.
- 17/06/2020 - Esrin - Intégra une vue limitée pour les joueurs dans le système de gestion des groupes.
- 17/06/2020 - Esrin - Fit en sorte que le tri alphabétique des compétences soit optionnel. Par défaut c'est désactivé.
- 17/06/2020 - Esrin - Répara la localisation des compétences pour les compétences de type Connaissances.
- 17/06/2020 - Cstadther - Amélioration #91, Différence de couleur pour les talents dans les arbres de spécialisation entre Actif et Passif.
- 16/06/2020 - Cstadther - Correction de bug vis à vis du lien bi-directionnel talents <-> spécialisation
- 16/06/2020 - Cstadther - Correction de bug #90, intégra le coût des talents dans les arbres de spécialisation.
- 16/06/2020 - Cstadther - Correction de bug #97, Réparation de l'apercu des talents quand on clique dessus.
- 16/06/2020 - Cstadther - Création du dialogue de changement de caratéristique, et intégration des valeurs localisés.
- 14/06/2020 - Cstadther - Rajouté la fonctionalité de change la caractéristque associe a une compétence.
- 14/06/2020 - Cstadther - Correction de bug #87 Valeur min/max des compétences et des caractéristiques
- 14/06/2020 - Cstadther - Correction de bug dans la fonction PrepareData de la feuille de personnage.
- 14/06/2020 - Cstadther - Correction de bug pour l'affichage des items, design plus réactif en enlevant la hauteure fixe établie.
- 14/06/2020 - Esrin - Correction de bug pour pas mal de soucis de performances dût a des faux acteurs contenant des objets de spécialisations.
- 14/06/2020 - Cstadther - Correction de bug #92, intégration d'un scrollbar dans les boôtes de dialogue des talents et des forces.
- 13/06/2020 - Cstadther - Added hook and text replace to add dice symbols to journal entries.
- 13/06/2020 - Esrin - Added 4 extra talent slots to the specialisation trees to match sourcebook examples.
- 13/06/2020 - Esrin - Added localisation to the talent activations on specialisation sheet.
- 13/06/2020 - Esrin - QoL improvements to specialisations to keep them synced up with any changes to linked talent descriptions or activations.
- 13/06/2020 - Esrin - Restored individual embedded talents to character sheets to allow for talents without associated specialisations (such as for rivals and nemesis).
- 13/06/2020 - Esrin - Bugfix to force power description display area.
- 12/06/2020 - Cstadther - Added Specializations Trees, utilizing drag and drop talents. Only for characters.
- 12/06/2020 - Esrin - Completed all initial Group Manager functionality and added last localisation hooks.
- 12/06/2020 - Cstadther - Added popout editor and dice symbol rendering for force powers. Updated popout editor to specify height/width/left/top.
- 12/06/2020 - Cstadther - Added popout editor for specials and dice symbol rendering in descriptions and specials
- 12/06/2020 - Esrin - Added warning on startup if Special-Dice-Roller module is not installed and activated.
- 12/06/2020 - Esrin - First pass on the group sheet. Now automatically populates with player characters, can open character sheets, change initiative mode and use the destiny pool. Other functionality under construction.
- 10/06/2020 - Cstadther - Readded Force Pool to Talent Tab
- 10/06/2020 - CStadther - Buxfix for Force Power Description field.
- 09/06/2020 - CStadther - Added drag-drop transfer of weapon, armour and gear items between owned character sheets.
- 08/06/2020 - CStadther - Added force power trees and associated view on the character sheets.
- 07/06/2020 - Esrin - Began localisation of Group Manager popup.
- 07/06/2020 - Esrin - Added new localisation for modifier types.
- 07/06/2020 - Esrin - Added new localisation for talent activations.
- 07/06/2020 - Esrin - Fixed localisation on character, minion and vehicle sheets for weapon range and firing arc display in inventory.
- 07/06/2020 - Jaxxa - Modify Wound / Strain tracking to be compatible with resource bars.
- 06/06/2020 - Jaxxa - Added Minion sheet calculating number of minions alive and reduce their skills as they die.
- 05/06/2020 - CStadther - Added select2 libraries for better dropdowns.
- 05/06/2020 - CStadther - Added Critical Injury and Critical Hit item types, along with associated display areas on character and vehicle sheets.
- 05/06/2020 - CStadther - Standardised localisation hooks for all langs.
- 05/06/2020 - Esrin - Removed legacy Critical Injury rolltable.
- 04/06/2020 - Esrin - Completed full transition to SASS. Removed old swffg.css file and ported all CSS logic into relevant SASS files.
- 04/06/2020 - HDScurox - Updated German language file.
- 04/06/2020 - ForjaSalvaje - Updated Spanish language file.
- 03/06/2020 - CStadther - Added localisation for all `swffg-config.js` values.
- 03/06/2020 - Esrin - Tweaked sensor range dropdown values.
- 03/06/2020 - CStadther - Fixed positioning issue with tool tips on vehicle sheet.
- 03/06/2020 - CStadther - Restyled bottom of vehicle biography section.
- 03/06/2020 - CStadther - Added localisation for skill names.
- 03/06/2020 - HDScurox - Updated German language file.
- 03/06/2020 - Esrin - Implemented scroll position saving when actor sheet elements are updated. No more popping back to the top of the skills list every time you make a change!
- 03/06/2020 - CStadther - Restyled vehicle weapon and attachment sheets.
- 03/06/2020 - Esrin - Bugfix to minion sheet groupskill display.
- 02/06/2020 - Esrin - Sheet styling tweaks.
- 02/06/2020 - Esrin - Correction de buges to minion sheet.
- 02/06/2020 - CStadther - Continued restyling vehicle sheet.
- 02/06/2020 - ForjaSalvaje - Spanish language translation.
- 02/06/2020 - Esrin - Some styling tweaks and fixes to the minion sheet skills display as suggested by Mandaar.
- 02/06/2020 - Mandaar - French language translation.
- 02/06/2020 - HDScurox - German language translation.
- 02/06/2020 - CStadther - Continued restyling minion sheet.
- 02/06/2020 - Esrin - Temporary display fixes to Minion and Vehicle sheets awaiting CStadther's eventual restyle.
- 02/06/2020 - Esrin - Minor bugfix to character sheet, soak value set to disabled for auto-calculation, encumbrance max and current values swapped to correct fields and current set to disabled for auto-calculation.
- 02/06/2020 - CStadther - Major sheet restyling
- 02/06/2020 - Jaxxa - Added Icons in the Dice roller, visually indicating the dice types.
- 31/05/2020 - Esrin - Work in progress on the group management GM tool. Destiny Pool now working (will reset on page refresh). Player Character list under construction.
- 31/05/2020 - Esrin - Bugfix to localisation hook for Gear Quantity on Character Sheet (thanks Alex | HDScurox for the bug report).
- 31/05/2020 - CStadther - Added SASS configuration using Gulp.
- 31/05/2020 - CStadther - Minor bugfix on .item click listener to prevent console errors when .item class components with no related item sheet are clicked, such as tabs.
- 31/05/2020 - CStadther - Added localization for character sheet.
- 29/05/2020 - Esrin - Minor bugfix to vehicle sheet, various fields will now accept string values to allow for from-to values as requested by Alex | HDScurox.
- 28/05/2020 - Esrin - Brought the Minion sheet inventory in line with the latest Character sheet changes. Added talents to Minion sheet. Fixed a minor bug with group skill calculations (thanks Alex | HDScurox for the bug report).
- 25/05/2020 - Esrin - Character sheet tweaks. Continued improvements to the inventory display in advance of equipable item support.
- 22/05/2020 - Esrin - Minor Correction de buges and tweaks, compatibility check with FVTT 0.6.0 stable release.
- 18/05/2020 - alfarobl - Tweak to dice display orders to match the chat order, kindly provided by alfarobl.
- 18/05/2020 - Esrin - A very hacky method has been introduced to allow the built in FoundryVTT combat tracker to roll initiative using FFG dice results. The resulting number is made up of successes and advantages. For example 1 success and 2 advantage would result in 1.02 for the initiative tracker. Warning, there might be bugs with this solution! Initiative can be switched between Vigilance and Cool via the System Settings section of the world configuration.
- 13/05/2020 - Esrin - Continued sheet design tweaks.
- 12/05/2020 - Esrin - Reworked actorsheet entities back down to a single entity with dynamic options based on actor.type. Now much easier to maintain in single place.
- 12/05/2020 - Esrin - First pass at improvements to inventory display to show more info on hover of certain areas (hover name for description, hover special for full text, etc). Still much more styling and layout work needed for sheets in general.
- 11/05/2020 - Esrin - First pass on some quality of life improvements to the inventory display (work in progress). Minor bugfixes.
- 11/05/2020 - Esrin - Fixed bug on vehicle sheet that was preventing data entry to some fields.
- 11/05/2020 - Esrin - Reworked the modifier tabs to be more foolproof and user friendly. Only Soak modifiers are calculated automatically at present. Automatic calculation of other stat / characteristic / skill modifiers is not a priority right now so putting on the backburner.
- 11/05/2020 - Esrin - Improved vehicle sheet design to have Defence in fore, aft, port, starboard cross pattern.
- 11/05/2020 - Esrin - Added Range, Skill, Firing Arc and Activation dropdowns to item and talent sheets where appropriate.
- 11/05/2020 - Esrin - Added skills filter to character and minion sheets, allowing filtering by General, Combat and Knowledge.
- 11/05/2020 - Esrin - Added career skills checkbox to character sheet.
- 11/05/2020 - Esrin - Fixed Handling on vehicle sheet. Now displays a + for positive values.
- 09/05/2020 - Esrin - Rollable table for Critical Injuries
- 09/05/2020 - Esrin - Cleaned up items to just use one JS class and get dynamic template by type.
- 09/05/2020 - Esrin - Built item sheet for ship weapons and ship attachments
- 09/05/2020 - Esrin - Built character sheet for vehicles
- 09/05/2020 - Esrin - Added data structure for ship weapons and ship attachments
- 09/05/2020 - Esrin - Added data structure for vehicles (using Jaxxa's work as a template)
- 09/05/2020 - Esrin - Added currency to characters
- 09/05/2020 - Esrin - Derived encumbrance from item values.
- 09/05/2020 - Esrin - Derived soak value from brawn, equipped armour, and modifiers on weapons, gear and talents as a test case for automation.
- 08/05/2020 - Esrin - Extended Actor class to allow for calculated Minion stat values (wounds from unit wounds _ quantity, and skills from group skills _ quantity-1)
- 08/05/2020 - Esrin - Added data structure for minions
- 08/05/2020 - Esrin - Built character sheet for minions
- 08/05/2020 - Esrin - Updated main character sheet to correctly display all three main item types, and talents.
- 08/05/2020 - Esrin - Added data structure for talents
- 08/05/2020 - Esrin - Updated main character sheet to show XP on all pages, and obligation types on Biography page.
- 08/05/2020 - Esrin - Built very basic item sheets for the three main item types.
- 08/05/2020 - Esrin - Added data structures for the three main item types, gear, weapons, armour.
- 07/05/2020 - Esrin - Minor tweaks to the character sheet styling. Begun restructuring the underlying data structure in template.json to introduce best practices, avoid unnecessary duplication and prepare for the addition of new actor and item types.
- 07/05/2020 - Esrin - First pass at character sheet styling. Next step, talents, items and derived modifiers.
- 06/05/2020 - Esrin - Added "Rolling <skillname>" into the chat message for FFG dice rolls to show which skill the person was rolling on.
- 06/05/2020 - Esrin - Added abbreviations (abrev) to characteristics, refactored skill display on ffg-actor-sheet.html to allow for linked characteristic abbreviations in display.
- 06/05/2020 - Esrin - Updated to TabsV2 class in actor-sheet-ffg.js to avoid deprecation of Tabs class in future FoundryVTT versions.
- 06/05/2020 - Esrin - Renamed remaining core files from Simple World Building to swffg naming scheme for consistency.
- 06/05/2020 - Esrin - Removed old SimpleWorldBuilding dependencies and fixed breakages where necessary.
