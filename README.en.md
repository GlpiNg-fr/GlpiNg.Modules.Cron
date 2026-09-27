# GlpiNg.Modules.Cron

*[Version française](README.md)*

GlpiNg's Cron module: runs, at a regular interval, the automatic actions (`ICronTask`) contributed by modules.

> **Disclaimer** — GlpiNg is an independent project. It is not affiliated with, endorsed,
> supported or sponsored by Teclib' or the GLPI project. "GLPI" and "GLPI-Agent" are trademarks
> of their respective owners; they are mentioned here only to describe GlpiNg's compatibility
> with the GLPI-Agent protocol and import from a GLPI database.

## Contents

- Background service with a global interval set from `/config`
- Persisted state per action: enabled, frequency, last run
- Run log

## Usage

This repository is a submodule of [GlpiNg](https://github.com/GlpiNg-fr/GlpiNg), under
`src/GlpiNg.Modules.Cron`. It does not build on its own: it references `GlpiNg.Modules.Abstractions` by relative path.

```bash
git clone --recurse-submodules https://github.com/GlpiNg-fr/GlpiNg.git
```

The host registers it with `services.AddCronModule()` (see `Program.cs`).

## License

[GNU Affero General Public License v3.0](LICENSE).
