Beamer Theme Cuerna
===================

Beamer theme "Cuerna", version 1.1

Copyright (C) Geri Ochoa  (2016)

e-mail: geri@bluesimplex.com

web site: http://bluesimplex.com

Dependencies:
-------------

   - textpos
   - tikz
   - xcolor
   - lmodern
   - amssymb
   - graphicx

Use *template.tex* as template for a new presentation.

This work may be distributed and/or modified under the conditions of the LaTeX
Project Public License, either version 1.3c of this license or (at your option)
any later version. The latest version of this license is in
http://www.latex-project.org/lppl.txt and version 1.3c or later is part of all
distributions of LaTeX version 2008/05/04 or later.

Installation:
-------------
The package is available on the **CTAN** repositories, so the easiest way to
install it on TexLive (as far as I know this should work on MacTeX too) is to
update the list of available packages running this command:

```bash
   sudo tlmgr update --list 
```

and install `beamertheme-cuerna` with the following command:

```bash
   sudo tlmgr install beamertheme-cuerna
```

Another method is to download the file **beamertheme-cuerna.tar.xz** from this
repository, open a terminal and run

```bash
   sudo tlmgr install --file beamertheme-cuerna.tar.xz 
```

That will place the files in the right folders and make the theme available
system-wide.

**Note:** The aforementioned commands will only work if you have installed
TeXLive from their official website. If you used your distribution package
manager or any other source those commands might not work.

If you prefer to use your local texfm directory you can find the source `*.sty`
files in `beamertheme-cuerna/tex/latex/beamertheme-cuerna/`



Usage:
------
After installing the package, download *template.tex* and the *pictures*
folder, place them in the same directory, open *template.tex* in your favorite
LaTeX editor and compile it. The code there is standard for any Beamer
document.

For the sake of completeness of this README file, the snippet below provides a
very basic example:

```TeX
\documentclass{beamer}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}

\usetheme{Cuerna}
\usecolortheme{default}

\logo{\includegraphics[width=1.7cm]{bluesimplex.png}}
\title{A rather long title without specific meaning}
\author{Geri Ochoa\\
\texttt{geri@bluesimplex.com}}

\date{Important Congress 2016}
\institute{Institute of Mathematics, Great University}

\begin{document}

  \begin{frame}
    \titlepage
  \end{frame}

  \section{Introduction}
  \begin{frame}
    \frametitle{Title of the slide}
    \framesubtitle{Subtitle}
    Some text on top of this slide
    \[
    \int_{0}^{\infty} \frac{5x^2}{\sqrt{a+b}}\, dx
    \]
    \begin{itemize}
    \item[\checkmark] Fist item in the list
    \item Second item
    \item Another item
    \item And finally, the last item
  \end{itemize}
  \end{frame}

\end{document}
```

The output will be different depending on the parameter passed to
`\usecolortheme`:

- `default`

![default](https://github.com/geriom/beamercuerna/blob/master/img/default.png
"Default Colour Theme")

- `bluesimplex`

![bluesimplex](https://github.com/geriom/beamercuerna/blob/master/img/bluesimplex.png
"Bluesimplex Colour Theme")

- `lettuce`

![lettuce](https://github.com/geriom/beamercuerna/blob/master/img/lettuce.png
"Lettuce Colour Theme")

- `brick`

![brick](https://github.com/geriom/beamercuerna/blob/master/img/brick.png
"Brick Colour Theme")
