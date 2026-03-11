# wine-proton Prebuilt Releases

Prebuilt **wine-proton hybrid** binaries for those who want to use wine-proton without having to compile it themselves.

## What's This?

These are hybrid builds that combine two of [Kron4ek's](https://github.com/Kron4ek/Wine-Builds) builds together:

- **Wine base** — Kron4ek's [wine-tkg](https://github.com/Frogging-Family/wine-tkg-git) builds (protonified Wine)
- **Proton base** — Kron4ek's official Valve Steam Proton builds

The result is a wine-proton hybrid that's ready to drop into your launcher of choice. These are provided purely for convenience — no modifications are made, just the legwork of putting them together so you don't have to.

## Available Releases

### Standard Builds

These use Kron4ek's wine-tkg (protonified Wine) as the Wine base paired with Kron4ek's Valve Steam Proton builds.

| Version | Build Name |
|---------|------------|
| 10.0-4  | `wine-proton-10.0-4-amd64-wow64` |
| 9.0-4   | `wine-proton-9.0-4-amd64` |
| 9.0-4   | `wine-proton-9.0-4-x86` |
| 8.0-5   | `wine-proton-8.0-5-amd64` |
| 8.0-5   | `wine-proton-8.0-5-x86` |
| 7.0-6   | `wine-proton-7.0-6-amd64` |
| 7.0-6   | `wine-proton-7.0-6-x86` |

### Bleeding Edge Builds

All bleeding edge builds use the **Valve Bleeding Edge** Wine build (`8.0-15630-g61cbb052f84`) as the Wine base, paired with Valve's own Proton builds pulled directly from Steam. All are x86_64 only.

> ⚠️ **Heads up:** Bleeding edge builds are based on in-development Wine code. They may offer better compatibility or performance for some titles, but can also be less stable than the standard releases. If something breaks, try the equivalent standard build.

| Version / Variant | Build Name |
|-------------------|------------|
| 10.0  | `wine-proton-10.0-bleeding_edge-x86_64` |
| 9.0   | `wine-proton-9.0-bleeding_edge-x86_64` |
| 8.0   | `wine-proton-8.0-bleeding_edge-x86_64` |
| 7.0   | `wine-proton-7.0-bleeding_edge-x86_64` |
| Experimental | `wine-proton-experimental-bleeding_edge-x86_64` |
| Hotfix  | `wine-proton-hotfix-bleeding_edge-x86_64` |

The **Experimental** build uses Valve's Proton Experimental branch — Valve's own testing ground for new features and fixes before they land in stable Proton. The **Hotfix** build uses Valve's Proton Hotfix branch, which carries urgent patches that Valve pushes outside of the normal release cycle. Both are pulled straight from Steam.

### Experimental Wine + GE-Proton Builds

These pair Kron4ek's **protonified wine-experimental** builds as the Wine base with **GE-Proton** (GloriousEggroll's community Proton builds) as the Proton base. The 10.0 build is amd64-wow64 only, while 9.0 comes in both amd64 and x86 variants, same as the standard releases.

| Version | Build Name |
|---------|------------|
| 10.0    | `wine-proton-10.0-experimental-amd64-wow64` |
| 9.0     | `wine-proton-9.0-experimental-amd64` |
| 9.0     | `wine-proton-9.0-experimental-x86` |

Head to the [**Releases**](../../releases) tab to download.

## Usage

1. Download the archive for your desired version from the [Releases](../../releases) page.
2. Extract it somewhere convenient:
   ```bash
   tar -xf wine-proton-<version>.tar.xz
   ```
3. Point your application/launcher at the extracted directory, or set `WINE` to the binary path:
   ```bash
   export WINE=/path/to/wine-proton-<version>/bin/wine
   ```

If you're using a launcher like **Lutris**, **Bottles**, or **Heroic**, you can usually add a custom Wine runner by pointing it at the extracted folder directly.

## Credits

- [Kron4ek / Wine-Builds](https://github.com/Kron4ek/Wine-Builds) — Upstream wine-tkg and Proton builds
- [Frogging-Family / wine-tkg-git](https://github.com/Frogging-Family/wine-tkg-git) — TkG's Wine build system
- [Valve / Proton](https://github.com/ValveSoftware/Proton) — Upstream Proton patches

## License

The binaries are built from upstream open-source projects and carry their respective licenses (largely LGPL). See the individual upstream repos for details.
