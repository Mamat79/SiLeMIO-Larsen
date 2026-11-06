# Larsen Lupin — SiLeMI/O

Larsen Lupin is available as a standalone application and an audio plug-in. The interface is in English and the user guide is in French and English.

Windows 2027.7 fixes an unexpected standalone exit when switching a track between MONO and STEREO. Existing settings, cuts and input/output assignments are retained.

[Windows 2027.7 installer](https://github.com/Mamat79/SiLeMIO-Larsen/releases/download/v2027.7/SiLeMIO-Larsen-2027.7-Setup.exe) · [Windows bilingual guide](https://github.com/Mamat79/SiLeMIO-Larsen/releases/download/v2027.7/Larsen-Lupin-2027-Manual.pdf)

[macOS 2027.6 universal installer](https://github.com/Mamat79/SiLeMIO-Larsen/releases/download/v2027.6/SiLeMIO-Larsen-2027.6-Mac.dmg) · [macOS bilingual guide](https://github.com/Mamat79/SiLeMIO-Larsen/releases/download/v2027.6/Larsen-Lupin-2027-Manual-Mac.pdf) · [Mac SHA-256](https://github.com/Mamat79/SiLeMIO-Larsen/releases/download/v2027.6/SiLeMIO-Larsen-2027.6-Mac.dmg.sha256)

Windows x64 includes the standalone application and VST3. The macOS 2027.6 universal package includes standalone, AU and VST3 for Intel and Apple Silicon. macOS 11 is the minimum declared in its metadata. Mac applications use ad-hoc signatures and are not notarized with a Developer ID.

New Windows configurations start in **Manual**, with main processing at **70%**, extra Noise reduction **20%**, extra Reverb reduction **10%** and extra Feedback **0%**. Main automatic feedback protection remains active when extra Feedback is zero. Start gently and adjust by ear; use the least correction that works.

Existing projects and saved values are preserved. To recall the gentle extras in an existing setup, choose **Auto**, then **Manual**. Amount, timings and permanent cuts stay unchanged; double-click Amount to return it to 70%. The Settings menu provides Copy/Paste and confirmed transfer to other detected instances. Isolated host instances require Copy/Paste.

Free audio starts its first activation when connected to the Internet. If needed, open **Free / Support** and choose **Enable free audio**; no purchase or supporter code is required. Once activated, everyday audio use works offline. After the first 30 days, the launch reminder waits five seconds. The optional permanent supporter licence, EUR 49, removes this wait. Keep existing activation data and close the application and any host using the plug-in before updating.

[What's new in Windows 2027.7](RELEASE-2027.7.md) · [File integrity and Windows checks — FR/EN](QUALIFICATION-WINDOWS-2027.7.md) · [Product information and downloads](https://www.silemio.com/logiciels/larsen-lupin)

## macOS 2027.6

The universal installer includes standalone, AU and VST3 for Apple Silicon and Intel, with a separate bilingual Mac guide. Twelve selected native CTests and seven separate Python checks passed. Seven installer selections and the read-only mounted DMG were checked; the Apple Silicon synthetic smoke test exited normally.

Intel was cross-built and statically checked. macOS 11 is the declared minimum, without an oldest-OS execution matrix. No real AU/VST3 host, physical audio/feedback loop, Windows/Mac audio-equivalence or complete interactive visual acceptance is claimed. Ad-hoc signatures, without Apple Developer ID or notarization; no real commercial activation. Previous packages remain available.

## macOS 2027.6 — français

L’installeur universel réunit l’application autonome, l’AU et le VST3 pour Apple Silicon et Intel, avec un guide Mac bilingue distinct. Douze CTests natifs sélectionnés et sept contrôles Python séparés ont réussi. Sept sélections d’installation et le DMG monté en lecture seule ont été contrôlés ; l’essai synthétique Apple Silicon s’est fermé normalement.

Intel est compilé et vérifié statiquement. macOS 11 est le minimum déclaré, sans matrice d’exécution des anciens systèmes. Aucune recette dans un hôte AU/VST3 réel, sur matériel audio/boucle de larsen, d’équivalence audio Windows/Mac ou visuelle interactive complète n’est revendiquée. Signature ad hoc, sans Apple Developer ID ni notarisation ; aucune activation commerciale réelle. Les anciens paquets restent disponibles.

