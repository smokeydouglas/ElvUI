# Third-Party Fonts

These static TrueType fonts are bundled for the `Class Modern` installer theme
and as optional LibSharedMedia choices. Each remains under its upstream SIL
Open Font License 1.1; the complete license texts are stored in `Licenses/`.

| Bundled file | UI role | Upstream source | Version | SHA-256 | License |
| --- | --- | --- | --- | --- | --- |
| `Inter-Medium.ttf` | Optional general-purpose sans serif | https://github.com/rsms/inter | 4.1 | `97ad806f526e41546d46365bb3a393145f75b7b1568913db74549ad8b8dba872` | `Licenses/Inter-OFL.txt` |
| `BarlowCondensed-SemiBold.ttf` | Optional condensed HUD and label face | https://github.com/google/fonts/tree/main/ofl/barlowcondensed | google/fonts commit `7ff85c87f93ea6cca5f41c69f2e4edcb90240f26` | `7b619d14bc2327509a9ef32b0890f709626f7ecc9ff61191c2a4314c5499d2d9` | `Licenses/Barlow-OFL.txt` |
| `JetBrainsMonoNL-Medium.ttf` | Optional monospaced numeric and data face | https://github.com/JetBrains/JetBrainsMono | 2.304 | `44099e1efefba55637e0abbbf8dd3f526e59523345888a257bb01d39df4af74c` | `Licenses/JetBrainsMono-OFL.txt` |
| `Roboto-Regular.ttf` | Class Modern default and small UI text | https://github.com/google/fonts/tree/main/ofl/roboto | Roboto 3.015; `wdth=100`, `wght=400` | `c76bbfa0c89791a8f3c6c25c5676ff3cc4a65833e521898127396c9c1ffe850a` | `Licenses/Roboto-OFL.txt` |
| `Roboto-Medium.ttf` | Optional medium-weight UI face | https://github.com/google/fonts/tree/main/ofl/roboto | Roboto 3.015; `wdth=100`, `wght=500` | `070b1134676412528e9cf3c9e3fe691bd3e293510a596515971876c3b6871930` | `Licenses/Roboto-OFL.txt` |
| `RobotoCondensed-Regular.ttf` | Optional compact UI face | https://github.com/google/fonts/tree/main/ofl/roboto | Roboto 3.015; `wdth=75`, `wght=400` | `df8a5049764410b7fda7b58e34ad7ae0e620abad73965993bba169bd20ade80b` | `Licenses/Roboto-OFL.txt` |
| `RobotoMono-Regular.ttf` | Optional timers, counts, and data face | https://github.com/google/fonts/tree/main/ofl/robotomono | google/fonts commit `7ff85c87f93ea6cca5f41c69f2e4edcb90240f26`; `wght=400` | `05950bb3fcaef7aad56ecf0802b37b83fab343e16ae6eeb83df5ca7b97e9a7f9` | `Licenses/RobotoMono-OFL.txt` |

The JetBrains Mono NL build omits programming ligatures, making it the safer
choice for the legacy World of Warcraft 3.3.5a text renderer.

The Roboto files were generated with FontTools 4.60.1 from the official Google
Fonts variable TTFs at commit `7ff85c87f93ea6cca5f41c69f2e4edcb90240f26`.
The source Roboto and Roboto Mono files have SHA-256 checksums
`d7598e12c5dbef095ff8272cfc55da0250bd07fbdecbac8a530b9b277872a134`
and `66a80e79d17e4c7cabd162e2916578a4cc08fd19eef6e2a643305eae9c567b2b`
respectively. All variation tables were removed from the generated static
instances for compatibility with the legacy client.
