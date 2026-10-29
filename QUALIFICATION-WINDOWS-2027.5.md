# Larsen Lupin 2027.5 — qualification Windows / Windows qualification

## Français

Windows 11 x64 : autonome construit localement sur le Dell depuis la source privée `676f0023b96fc7b17cdd8f96402c7bcd299397c4`, branche `release/windows-2027.5-20261029`, avec Visual Studio 2022, JUCE 8.0.12 et la recette `Installer/Larsen-2027.5.iss`. Le VST3 et son manifeste sont réemployés depuis `2b002fcc7c356a2f95c6766770ce1abc1f1df8ea` : toutes leurs entrées de production sont identiques, les dépendances réelles de compilation excluent les fichiers de tests modifiés, et leurs empreintes sont vérifiées. Ce VST3 n'est pas présenté comme une nouvelle compilation.

Installateur : **78504570 octets**, SHA-256 `3cd6e1d6eda93c8c76e7254600fae9827b8b6adc86739b035b2060c8e69c6e75`. L'extraction contient 11 fichiers conformes ; les deux identifiants VST3 et l'identité de mise à jour sont conservés. L'installation réelle a terminé avec le code 0 ; les 11 fichiers réellement installés correspondent au paquet.

Le contrôle complet `--verify-ui` passe d'abord sur l'EXE privé puis sur l'EXE installé. Le contrôle installé `--verify-settings-transfer` passe également. Les rapports vérifient commandes, paramètres, transfert et captures dans un profil isolé. La suite source dédiée a réussi 38 579 assertions (incluant des échantillons, pas autant de scénarios indépendants). Les deux échecs précédents du banc d'interface sont conservés : accès vide après RESET/Auto puis scénario tentant des commandes désactivées en Auto. Les scénarios sont corrigés ; aucun calcul audio ni contrat produit n'a été assoupli.

Les sauvegardes privées C/D et la copie de restauration ont été conservées ; une comparaison fraîche avant/après confirme les 41 fichiers personnels suivis inchangés, avec contenu, flux, dates de création/modification et droits contrôlés. Les licences sont conservées comme données opaques. Aucune ancienne version publique ni aucun ancien tag n'est supprimé.

Limites : gestes des boutons natifs de fenêtre, menu humain et presse-papiers non exercés ; deux captures revues sur les quinze produites. Installateur Windows non signé ; tests sans périphérique audio physique, sans boucle acoustique ni hôte DAW réel, sans nouvelle activation commerciale. Les illustrations spectrales synthétiques ne sont pas des mesures du moteur. La fixture de guide des tests ne prouve pas l'ouverture du vrai PDF ; son contenu est livré et son empreinte contrôlée. macOS reste **2027.4**, avec sa qualification propre ; aucune version Mac 2027.5 n'est revendiquée. Mod est exclu.

## English

Windows x64 standalone built locally from private source `676f0023b96fc7b17cdd8f96402c7bcd299397c4` using Visual Studio 2022, JUCE 8.0.12 and the unchanged 2027.5 installer recipe. The VST3 and SDK manifest reuse the build from source `2b002fcc7c356a2f95c6766770ce1abc1f1df8ea`, with all production inputs unchanged, actual compiler dependencies checked and exact hashes preserved. This is explicitly reused binary provenance.

The extracted 11-file payload matches the package. Actual installation exited 0, and all 11 installed files match. The complete private EXE UI check passes before packaging; the installed EXE UI and settings-transfer checks then pass in isolated profiles. The dedicated source suite passes 38,579 assertions, including samples rather than 38,579 independent scenarios. Earlier UI harness failures remain recorded; their fixtures were corrected without changing DSP calculations or weakening the product contract.

Existing private backups and restoration rehearsal are retained. Fresh before/after checks confirm all 41 monitored personal files unchanged, including content, streams, creation/write times and ACLs. Licence data remains opaque. Previous public releases, tags and assets are preserved.

Limits: native title-bar clicks, human menu interaction and clipboard not exercised; two of the fifteen generated captures reviewed. Unsigned Windows installer; no physical audio, acoustic loop, real DAW host or new commercial activation acceptance. Synthetic spectral illustrations are not production-engine measurements. The test's guide fixture does not prove opening the real manual. macOS remains separately qualified **2027.4**; Mod is excluded.
