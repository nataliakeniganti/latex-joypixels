# JoyPixels for LaTeX

If you are setting this up for a project or looking to expand the documentation, here are a few additional tips you might want to include or keep in mind for users:

### 1. Mention the Engine Requirement
Since `joypixels` relies on system fonts and color emoji support, it **will not work with pdfLaTeX**. It's helpful to explicitly state:
> **Note:** This project must be compiled with **XeLaTeX** or **LuaLaTeX**. Standard pdfLaTeX is not supported.

### 2. Licensing Note
The `joypixels` package provides a bridge to the JoyPixels emoji set. Depending on the version being used, users might need to be aware of the [JoyPixels license](https://www.joypixels.com/licenses).

### 3. Example Usage
Adding a tiny usage example in the README helps users verify their installation immediately:
```latex
\documentclass{article}
\usepackage{joypixels}

\begin{document}
Hello World! \joypixel{1f600} % Prints a grinning face
\end{document}
```

### 4. Troubleshooting common issues
Sometimes `tlmgr` installs the style files but not the actual font assets due to licensing. If users see missing glyphs, they may need to manually download the JoyPixels font and install it to their system fonts folder.
