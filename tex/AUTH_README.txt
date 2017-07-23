                 The dgruyter package:                 
preparing books and journals for Walter de Gruyter GmbH


File:       README
Author:     le-tex publishing services


DESCRIPTION
===========

The dgruyter package assists in preparing manuscripts for de Gruyter
with {\LaTeX}. It provides some special commands for journal papers
as well as for books and generates the required appearance.
Together with corresponding font packages it allows to produce the 
final layout of De Gruyter books and journal articles.

Copyright:  (C) 2015, 2016 Walter de Gruyter GmbH


FILES IN DISTRIBUTION
=====================

   BASE DISTRIBUTION:

      README                  This file.
      dgruyter.ins            Package installation file.
      dgruyter.dtx            Package source file.
      dg-degruyter.eps/.pdf   Logo files.
      dg-mouton.eps/.pdf      Logo files.
      dg-saur.eps/.pdf        Logo files.
      DG_attention.eps/.pdf   Vignette files.
      DG_exercise.eps/.pdf    Vignette files.
      DG_information.eps/.pdf Vignette files.
      DG_notice.eps/.pdf      Vignette files.
      DG_question.eps/.pdf    Vignette files.
      book.tex                Template file for a book.
      article.tex             Template file for a journal article.
      

   DOCUMENTATIONs:

      dgruyter.pdf            User manual for dgruyter package. 
                              It is produced as described below.

      dgruyter-faqs.pdf       Frequently asked questions to dgruyter.sty

     


BASIC INSTALLATION
====================

   To get the package style file 'dgruyter.sty' and the
   index style files 'dgruyter.ist' and 'dgruyter.xdy' execute:
     latex dgruyter.ins

   The minimum requirement to use the package is to have
     dgruyter.sty and dgruyter.ist/dgruyter.xdy
     (as well as the logo and vignette files)
     in a directory where TeX can find it.

   To get the documentation 'dgruyter.pdf' execute:
     pdflatex dgruyter.dtx (at least twice)
