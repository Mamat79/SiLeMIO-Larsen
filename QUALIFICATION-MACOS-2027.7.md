# Larsen Lupin 2027.7 — macOS / qualification et intégrité

## Français

Installeur universel : application autonome, AU et VST3 pour Apple Silicon et Intel. macOS 11 est le minimum déclaré dans les métadonnées, sans matrice d'exécution sur les anciens systèmes.

DMG : 149194437 octets. SHA-256 : `8f616f114a199cf4631d25fa5750352dfe94b5e12ae139321951cbf2a8f37cb7`.
Notice Mac bilingue distincte : 69795 octets, neuf pages ; SHA-256 `b8980ecee73da8c19272ba9faa137e632ef58989a408e23c90c5f0158c5088cb`.

Douze CTests natifs sélectionnés et sept diagnostics Python séparés ont réussi. Les sept sélections non vides de l'installeur, le refus d'une sélection inconnue, les quatre exécutables universels et leurs huit architectures ont été vérifiés. Quinze essais du Trousseau utilisent des identités de test et conservent/restaurent les états attendus, sans activation client.

Le DMG monté en lecture seule a fourni l'application autonome réellement exécutée sur Apple Silicon : aperçu logiciel isolé, fermeture normale code 0, huit bascules mono/stéréo directes et quatre changements par le vrai sélecteur et la file normale d'événements. Les paramètres, coupures, affectations et l'autre processeur sont conservés par ces assertions. Deux rendus de composants nouveaux ont été relus ; cela ne constitue pas une recette visuelle manuelle de tout le bureau.

Limites : Intel compilé et contrôlé statiquement, sans exécution sur matériel Intel ; aucun hôte AU/VST3 réel, carte son/boucle acoustique ou preuve d'équivalence audio Windows/Mac. Signature ad hoc contrôlée, sans Apple Developer ID ni notarisation ; aucune nouvelle activation commerciale. Les tests natifs sont sélectionnés et n'incluent pas toutes les anciennes campagnes optionnelles.

## English

Universal installer: standalone application, AU and VST3 for Apple Silicon and Intel. macOS 11 is the metadata minimum; the oldest-OS execution matrix was not run. DMG and distinct nine-page bilingual Mac-guide sizes and SHA-256 values are listed above.

Twelve selected native CTests and seven separate Python diagnostics passed. Seven nonempty installer selections, rejection of unknown selections, four universal executables/eight slices and fifteen isolated Keychain state tests were checked without client activation.

The actual standalone application from the read-only mounted DMG ran on Apple Silicon in isolated synthetic preview and exited normally with code 0. Eight direct mono/stereo changes and four changes through the actual selector/event queue passed while retaining processing parameters, cuts, routing and another processor. Two new component renders were reviewed; complete interactive desktop visual acceptance is not claimed.

Limits: Intel was cross-built and statically inspected, without physical Intel execution. No real AU/VST3 host, hardware/acoustic feedback loop or Windows/Mac audio-equivalence acceptance. Ad-hoc signing only, without Apple Developer ID or notarization; no new commercial activation. Selected native tests do not cover every historical optional campaign.
