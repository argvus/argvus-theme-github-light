# GitHub Light theme for ARGVUS

Official ARGVUS Light theme, `github-light`, with its Sticky and Float variants.

[![CI](https://github.com/argvus/argvus-theme-github-light/actions/workflows/ci.yml/badge.svg)](https://github.com/argvus/argvus-theme-github-light/actions/workflows/ci.yml)
[![Release](https://github.com/argvus/argvus-theme-github-light/actions/workflows/release.yml/badge.svg)](https://github.com/argvus/argvus-theme-github-light/actions/workflows/release.yml)
[![License](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](LICENSE)
[![Language: Shell](https://img.shields.io/badge/Shell-POSIX-4EAA25?logo=gnubash&logoColor=white)](https://www.gnu.org/software/bash/)
[![Platform: Arch Linux | Wayland](https://img.shields.io/badge/platform-Arch%20Linux%20%7C%20Wayland-1793D1?logo=archlinux&logoColor=white)](https://archlinux.org/)
[![Pull requests](https://img.shields.io/github/issues-pr/argvus/argvus-theme-github-light)](https://github.com/argvus/argvus-theme-github-light/pulls)
[![Issues](https://img.shields.io/github/issues/argvus/argvus-theme-github-light)](https://github.com/argvus/argvus-theme-github-light/issues)
[![Last commit](https://img.shields.io/github/last-commit/argvus/argvus-theme-github-light)](https://github.com/argvus/argvus-theme-github-light/commits/main)

## Theme identity

| Field | Value |
| --- | --- |
| Theme ID | `github-light` (Float variant: `github-light-float`) |
| Display name | GitHub Light |
| Mode | `light` |
| Default highlight | `#0969DA` |
| GTK color scheme | `prefer-light` |
| Package | `argvus-theme-github-light` |
| Wallpaper | `/usr/share/backgrounds/argvus/abstract/light/github-light-abstract-light.jxl` |

The values above are the ones declared in
`src/usr/share/argvus/themes/github-light/theme.toml`, the manifest that the
desktop reads. The manifest is the source of truth; this page describes it.

## Installing

The package depends on `argvus` and `argvus-appearance`, so pacman installs them with it.

```sh
sudo pacman -S argvus-theme-github-light
```

Select the theme in the Control Center (Appearance > Themes), or run
`argvus theme-switch github-light`.

## Files

The package installs the theme manifest,
`/usr/share/argvus/themes/github-light/theme.toml` (schema 2: name, category, wallpaper and
the palette), the templates it overrides under `overrides/` when it has any, and its
wallpapers under `/usr/share/backgrounds/argvus`. The files of every component are
rendered from the palette by the component's own templates when the theme is applied,
for Sticky and Float alike. `argvus theme check src/usr/share/argvus/themes/github-light`
renders them all and reports any error.

## Development

Validate with `make validate` before building. The design rules are in
[DEVELOPMENT.md](DEVELOPMENT.md); the ARGVUS documentation for themes is in
`argvus/docs/en/user-guide/appearance.md` of the `argvus` repository.

## Contributing and policies

- [CONTRIBUTING.md](https://github.com/argvus/.github/blob/main/CONTRIBUTING.md) — contribution workflow
- [SECURITY.md](https://github.com/argvus/.github/blob/main/SECURITY.md) — private vulnerability reports
- [Code of Conduct](https://github.com/argvus/.github/blob/main/policies/CODE_OF_CONDUCT.md) — community standards
- [AI usage policy](https://github.com/argvus/.github/blob/main/policies/IA_USAGE.md) — rules for AI-assisted contributions

## License

GPL-3.0-only. See [LICENSE](LICENSE).
