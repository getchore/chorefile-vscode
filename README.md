# chorefile for VS Code

Syntax highlighting for [chore](https://github.com/getchore/chore) task files.

It applies to any file named `chorefile` and to any file with the `.chore`
extension, which is what `include` pulls in. It colors comments, `task`
definitions and their parameters, the control keywords, the builtin commands,
the read-only builtin variables such as `$OS` and `$ROOT`, `$var` interpolation
inside double-quoted strings, `$(...)` captures, and the comparison, logical,
pipe and redirect operators.

Highlighting only. There is no language server, no formatter, and no task
integration.

## Install

Download `chorefile.vsix` from the [latest release](https://github.com/getchore/chorefile-vscode/releases/latest), then:

```
code --install-extension chorefile.vsix
```

The same file works in Cursor (`cursor --install-extension chorefile.vsix`) and
VSCodium (`codium --install-extension chorefile.vsix`). You can also install it
from the editor: Extensions view, the `...` menu, "Install from VSIX".

The extension is not on a marketplace, so there are no automatic updates yet.
To upgrade, download the newer `.vsix` and run the same command again.

## License

MIT.
