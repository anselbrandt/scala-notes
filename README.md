# scala-notes

### SDKMAN

```
curl -s "https://get.sdkman.io" | bash

source "$HOME/.sdkman/bin/sdkman-init.sh"

sdk version
```

### sbt

```
sdk install sbt
```

### Metals VSCode Extension

https://scalameta.org/metals/docs/editors/vscode.html

Install from [Marketplace](https://marketplace.visualstudio.com/items?itemName=scalameta.metals)

Next, open a directory containing your Scala code. The extension activates when the main directory contains `build.sbt` or `build.sc` file, a Scala file is opened, which includes `*.sbt`, `*.scala` and `*.sc` file, or a standard Scala directory structure `src/main/scala` is detected.
