gpdfx-ng - a graphical tool to extract parts of a PDF as a PDF
===============================

`gpdfx-ng` is a GTK application written in Python using the Poppler library
to render the PDF. It uses pdfTeX and PDFCrop to create the extracted
PDF.

# Features
My improvements to the ancient `gpdfx`:

- Add a "Open" button (open file). 
- Add a "Auto Fit" botton. It helps to fit the pdf file according to the size of the window.
- Add a button "Viewport". It copies the "viewport" of the selected area to the clipboard. 
- Add a status bar.

# Install
Dependency
- Python2 or Python3
- poppler-glib
- python-gobject
- gtk3
- python-cairo

# Usage
- Run `gpdfx` and open a pdf file.
- Select an area.
- Export the selection to a pdf file, or copy the "viewport" to the clipboard.

## Viewport
If you want to insert the selected area of your pdf file in a LaTeX document, you may find the following codes useful.
```
  \begin{figure}[ht]
    \includegraphics[clip, page=1, viewport=1 2 3 4,
    width=1.0\textwidth, fbox]{paper.pdf}
  \end{figure}
```

Upstream
--------
- https://github.com/lehner/gpdfx
- Author: Christoph Lehner (clehner // users.sourceforge.net)
