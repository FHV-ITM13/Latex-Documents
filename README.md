Latex thesis template for FHV
===============

## Template information

This latex template was especially created for writing a bachelor or master thesis at University of Applied Sciences Vorarlberg (FHV).

Feel free to use this template for your thesis too. You can also provide any pull requests if you like.

Feedback is welcome.

## Template usage

### Settings

To change the visibility of blocking notice page, abstract, toc, tol, tof, todos, summary, reference pages, attachment page and statutory declaration or to change the page borders see file at (about) line 70:

```
template\settings\settings.tex
```

To change the content of variables like your name, the title of your thesis, your supervisors' name .... please see the following file. It is highly recommended that you adapt this file and change the values of the attributes to your needs.

```
document\settings\attributes.tex
```

### BibTeX

Please keep in mind that you have to build the document with BibTex seperatly. To get proper bibliography you have to perform the following compiling steps:

  1. LaTex
  2. BibTex
  3. LaTex
  4. LaTex

If you use any IDE take a look into the options menu - maybe you can find any option to automatize this.

It is also possible to use Zotero for reference management and BibTex.

## Repo Usage

Create or Clone own empty repository:

```
git remote add template git@github.com:FHV-ITM13/Latex-Documents.git
git pull template fhvthesistemplate 
```

Push it to your own Repository:

```
git push origin fhvthesistemplate
```
