# Third-Party Fonts

These static TrueType fonts are bundled for the `Class Modern` installer
theme. Each remains under its upstream SIL Open Font License 1.1; the complete
license texts are stored in `Licenses/`.

| Bundled file | UI role | Upstream source | Version | SHA-256 | License |
| --- | --- | --- | --- | --- | --- |
| `Inter-Medium.ttf` | General UI, chat, and tooltip body text | https://github.com/rsms/inter | 4.1 | `97ad806f526e41546d46365bb3a393145f75b7b1568913db74549ad8b8dba872` | `Licenses/Inter-OFL.txt` |
| `BarlowCondensed-SemiBold.ttf` | Unit frames, nameplates, tabs, and combat labels | https://github.com/google/fonts/tree/main/ofl/barlowcondensed | google/fonts commit `7ff85c87f93ea6cca5f41c69f2e4edcb90240f26` | `7b619d14bc2327509a9ef32b0890f709626f7ecc9ff61191c2a4314c5499d2d9` | `Licenses/Barlow-OFL.txt` |
| `JetBrainsMonoNL-Medium.ttf` | Cooldowns, counts, data texts, and numeric overlays | https://github.com/JetBrains/JetBrainsMono | 2.304 | `44099e1efefba55637e0abbbf8dd3f526e59523345888a257bb01d39df4af74c` | `Licenses/JetBrainsMono-OFL.txt` |

The JetBrains Mono NL build omits programming ligatures, making it the safer
choice for the legacy World of Warcraft 3.3.5a text renderer.
