# GlpiNg.Modules.Cron

*[English version](README.en.md)*

Module Cron de GlpiNg : exécute à intervalle régulier les actions automatiques (`ICronTask`) contribuées par les modules.

> **Avertissement** — GlpiNg est un projet indépendant. Il n'est ni affilié à, ni approuvé,
> soutenu ou sponsorisé par Teclib' ou le projet GLPI. « GLPI » et « GLPI-Agent » sont des
> marques de leurs propriétaires respectifs ; elles ne sont citées ici que pour décrire la
> compatibilité de GlpiNg avec le protocole GLPI-Agent et l'import depuis une base GLPI.

## Contenu

- Service de fond à intervalle global réglable depuis `/config`
- État persisté par action : activation, fréquence, dernière exécution
- Journal d'exécution

## Utilisation

Ce dépôt est un sous-module de [GlpiNg](https://github.com/GlpiNg-fr/GlpiNg), sous
`src/GlpiNg.Modules.Cron`. Il ne se compile pas seul : il référence `GlpiNg.Modules.Abstractions` par chemin relatif.

```bash
git clone --recurse-submodules https://github.com/GlpiNg-fr/GlpiNg.git
```

L'hôte l'enregistre par `services.AddCronModule()` (voir `Program.cs`).

## Licence

[GNU Affero General Public License v3.0](LICENSE).
