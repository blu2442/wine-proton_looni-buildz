# wine-proton Prebuilt Releases

Prebuilt **wine-proton hybrid** binaries for those who want to use wine-proton without having to compile it themselves.

## What's This?

These are prebuilt hybrids that combine a Wine build and a Proton build:

- **Wine base** —  any upstream/custom Wine build
- **Proton base** — any official/custom Proton build

These are made to provide stable as well as experimental and bleeding edge builds — no modifications are made other than using umu-protonfixes as opposed to plain protonfixes in the installer. It's just the effort to put together some good to use builds that work well and can be used inside and outside of your launcher of choice. Just extract the tarball and drop the wine-proton into your folder of choice. Then it will be ready to use :3

## Available Releases

### Standard Builds

These use Kron4ek's wine-tkg protonified Wine as the Wine base paired with Kron4ek's Proton builds.

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

### Experimental wine-proton Builds

These pair Kron4ek's **protonified wine-experimental** builds as the Wine base with various Proton bases. The versioned 10.0 and 9.0 builds use **GE-Proton**, while the Experimental and Hotfix variants use Valve's own Proton branches pulled from Steam — all on the wine-experimental 10.0 base. The 9.0 builds come in both amd64 and x86 variants; all others are amd64-wow64 only.

| Version / Variant | Build Name |
|-------------------|------------|
| 10.0         | `wine-proton-10.0-experimental-amd64-wow64` |
| 9.0          | `wine-proton-9.0-experimental-amd64` |
| 9.0          | `wine-proton-9.0-experimental-x86` |
| Experimental | `wine-proton-experimental-amd64-wow64` |
| Hotfix       | `wine-proton-hotfix-amd64-wow64` |

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

Built on top of [ValveSoftware](https://github.com/ValveSoftware/wine), [Wine-TKG](https://github.com/Frogging-Family/wine-tkg-git), [Proton-TKG](https://github.com/Kron4ek/proton-archive), [GE-Proton](https://github.com/GloriousEggroll/proton-ge-custom), [protonfixes](https://github.com/nicowillis/protonfixes), [umu-protonfixes](https://github.com/Open-Wine-Components/umu-protonfixes), and the broader Wine project.

## License

The binaries are built from upstream open-source projects and carry their respective licenses (largely LGPL). See the individual upstream repos for details.
