# Vorlage für Dokumentation und Abschlussarbeiten

## Installation

1. [TeX Live](https://www.tug.org/texlive/) installieren

2. Die Packages aus packages.txt müssen zunächst installiert werden. Dazu kann folgender Befehl verwendet werden:

   ```sh
   # Linux/macOS
   $ xargs tlmgr install < packages.txt
   # Windows (cmd)
   > for /F %i in (packages.txt) do tlmgr install %i
   # Windows (PowerShell)
   PS> Get-Content packages.txt | ForEach-Object { tlmgr install $_ }
   ```

   Bei macOS muss evtl. `sudo` und bei Windows `Als Administrator ausführen` verwendet werden.

3. Für die Darstellung von Code wird das "minted"-Package verwendet. Damit dies kompiliert muss folgendes erledigt werden:
   https://alipourmousavi.com/blog/index.php/2018/02/08/using-minted-package-in-latex-to-format-codes/

### Visual Studio Code + TeX Live
- Erweiterung für VSCode: [LaTex-Workshop](https://github.com/James-Yu/LaTeX-Workshop/wiki)

### IntelliJ + MiKTex
- Plugin für IntelliJ: [TeXiFy IDEA](https://plugins.jetbrains.com/plugin/9473-texify-idea)
- Weitere Schritte die nötig sind für das Plugin: https://github.com/Hannah-Sten/TeXiFy-IDEA/wiki/Installation
