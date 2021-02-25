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

Docs:

https://www.scala-sbt.org/1.x/docs/

### Metals VSCode Extension

https://scalameta.org/metals/docs/editors/vscode.html

Install from [Marketplace](https://marketplace.visualstudio.com/items?itemName=scalameta.metals)

In VSCode Settings, set `metals.superMethodLensesEnabled` to `true`

Next, open a directory containing your Scala code. The extension activates when the main directory contains `build.sbt` or `build.sc` file, a Scala file is opened, which includes `*.sbt`, `*.scala` and `*.sc` file, or a standard Scala directory structure `src/main/scala` is detected.

Add to `.gitignore`:

```
# ~/.gitignore
.metals/
.bloop/
.ammonite/
metals.sbt
```

### Scalafmt

First install [Coursier](https://get-coursier.io/docs/cli-installation)

```
$ curl -fLo cs https://git.io/coursier-cli-"$(uname | tr LD ld)"
$ chmod +x cs
$ ./cs install cs
$ rm cs
```

Use `coursier` to install `scalafmt`

```
cs install scalafmt
scalafmt --version
```
