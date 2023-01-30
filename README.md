# QR-test-documents

A small collection of pdf-documents with various amounts of QR-codes in them. Created with the help of Overleaf.
The base LaTeX is variations of the following:

```
\documentclass[11pt]{article}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}

\usepackage{pstricks}
\usepackage{pst-barcode}
\usepackage{lipsum}  

\begin{document}

\title{Multipage document with an increasing amount of qr-codes}
\date{}
\maketitle

\section{Introduction}

\lipsum[1-2]

\newpage

\section{Contract details}

\lipsum[3-4]

\begin{pspicture}(25mm,25mm)
\psbarcode{https://luisto.fi}{eclevel=H width=1.0 height=1.0}{qrcode}
\end{pspicture}


\newpage


\section{Epilogue}

\begin{pspicture}(25mm,25mm)
\psbarcode{https://luisto.fi}{eclevel=H width=1.0 height=1.0}{qrcode}
\end{pspicture}
\lipsum[5]
\begin{pspicture}(25mm,25mm)
\psbarcode{https://luisto.fi}{eclevel=H width=1.0 height=1.0}{qrcode}
\end{pspicture}

\newpage

\section{Calamity}
\begin{pspicture}(25mm,25mm)
\obeylines
\psbarcode{%
BEGIN:VCARD^^J
VERSION:4.0^^J
N:Luisto,Rami^^J
FN:Rami Luisto^^J
ORG:Digital Workforce^^J
URL:https://luisto.fi^^J
EMAIL:rami.luisto@digitalworkforce.com^^J
TEL;TYPE=work,voice;VALUE=uri:tel:+44-123-456-789^^J
ADR;TYPE=home;LABEL="Street address, City, Province, Postal-code, Country":Post office box;Extended address;Street address;City;Province;Postal-code;Country^^J
END:VCARD
}{width=1.0 height=1.0}{qrcode}%
\end{pspicture}

\lipsum[1]

\begin{pspicture}(25mm,25mm)
\psbarcode{https://luisto.fi}{eclevel=H width=1.0 height=1.0}{qrcode}
\end{pspicture}
\begin{pspicture}(25mm,25mm)
\psbarcode{https://luisto.fi}{eclevel=H width=1.0 height=1.0}{qrcode}
\end{pspicture}
\begin{pspicture}(25mm,25mm)
\obeylines
\psbarcode{%
BEGIN:VCARD^^J
VERSION:4.0^^J
N:Luisto,Rami^^J
FN:Rami Luisto^^J
ORG:Digital Workforce^^J
URL:https://luisto.fi^^J
EMAIL:rami.luisto@digitalworkforce.com^^J
TEL;TYPE=work,voice;VALUE=uri:tel:+44-123-456-789^^J
ADR;TYPE=home;LABEL="Street address, City, Province, Postal-code, Country":Post office box;Extended address;Street address;City;Province;Postal-code;Country^^J
END:VCARD
}{width=1.0 height=1.0}{qrcode}%
\end{pspicture}
\begin{pspicture}(25mm,25mm)
\psbarcode{https://luisto.fi}{eclevel=H width=1.0 height=1.0}{qrcode}
\end{pspicture}
\begin{pspicture}(25mm,25mm)
\psbarcode{https://luisto.fi}{eclevel=H width=1.0 height=1.0}{qrcode}
\psbarcode{https://luisto.fi}{eclevel=H width=1.0 height=1.0}{qrcode}
\psbarcode{https://luisto.fi}{eclevel=H width=1.0 height=1.0}{qrcode}
\end{pspicture}


\end{document}
```
