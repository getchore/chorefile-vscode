# chorefile for VS Code

Syntax highlighting for [chore](https://github.com/getchore/chore) task files.

It applies to any file named `chorefile` and to any file with the `.chore`
extension, which is what `include` pulls in: `rust.chore`, `release.chore`,
`.github/ci.chore`. It colors comments, `task`
definitions and their parameters, the control keywords, the builtin commands,
the read-only builtin variables such as `$OS` and `$ROOT`, `$var` interpolation
inside double-quoted strings, `$(...)` captures, and the comparison, logical,
pipe and redirect operators.

Highlighting only. There is no language server, no formatter, and no task
integration.

## Install

```sh
curl -fsSL https://github.com/getchore/chorefile-vscode/releases/latest/download/chorefile.vsix -o /tmp/chorefile.vsix \
  && code --install-extension /tmp/chorefile.vsix
```

PowerShell:

```powershell
irm https://github.com/getchore/chorefile-vscode/releases/latest/download/chorefile.vsix -OutFile $env:TEMP\chorefile.vsix
code --install-extension $env:TEMP\chorefile.vsix
```

`latest/download` resolves server side, so the URL never changes between
releases. Swap `code` for `cursor` or `codium` to install into those.

Or download `chorefile.vsix` from the [latest release][rel] and use the
Extensions panel, "..." menu, Install from VSIX.

[rel]: https://github.com/getchore/chorefile-vscode/releases/latest

There are no automatic updates yet, since the extension is not on a marketplace.
Run the same command again to move to a newer release.

## License

MIT.
