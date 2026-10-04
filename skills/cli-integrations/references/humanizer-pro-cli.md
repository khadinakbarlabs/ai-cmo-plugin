# Humanizer PRO through its standalone CLI

Use the owner's separate CLI release: https://github.com/khadinakbarlabs/humanizer-pro-cli-plugin/releases/tag/v0.2.0 . The package is downloaded from that release, not the npm registry. Verify its checksum and install the standalone CLI according to the release instructions; AI CMO does not bundle its runtime.

```sh
humanizer-pro --help
humanizer-pro login
humanizer-pro status
humanizer-pro balance
```

Only revise a passage the user selects for this operation. Explain that rewriting sends that passage through Humanizer PRO to Rephrasy, consumes existing account words and stores private source/output history. Obtain or honor explicit consent for those effects; never silently process workspace files. Feed selected text through stdin using a quoted delimiter or direct process input, without shell expansion. The operation is `humanizer-pro rewrite --consent --mode marketing`; confirm the installed contract and 12,000-character limit first.

Report returned text, usage and meaning/factual checks. Do not promise unchanged claims or detector outcomes. Keep uncertain charged operations unresolved until history/balance is checked; do not automatically retry. This route is optional copy revision, not original ad generation. Manual editing is the fallback. Service terms/privacy: https://texthumanizer.pro/terms and https://texthumanizer.pro/privacy .
