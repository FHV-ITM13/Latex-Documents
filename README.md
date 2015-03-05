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

You may run into truble when you use this template together with umlauts since every operating system uses its own encoding standard. You may have to adapt the file 'template\packages.tex' at line 13 like this:

```
Windows
\usepackage[ansinew]{inputenc}
Linux
\usepackage[latin1]{inputenc}
Mac
\usepackage[applemac]{inputenc}

Should this not work try this:
\usepackage[utf8]{inputenc}
```

### Add new content (chapter,..)

All files including your text are located in the directory 'document\content'. Just edit the file 'document\content\content.tex' when you want to add a new file (e.g. containing a whole chapter) by adding the following line:

```
\include{document/content/FILENAME}
```

### Statutory declaration, blocking notice and attachment

If you need to change the text of the statuatory declaration, the blocking notice or the attachment you find the files in the directory 'document\other'.

### BibTeX

Please keep in mind that you have to build the document with BibTex seperatly. To get proper bibliography you have to perform the following compiling steps:

  1. LaTex
  2. BibTex
  3. LaTex
  4. LaTex

If you use any IDE take a look into the options menu - maybe you can find any option to automatize this.

It is also possible to use Zotero for reference management and BibTex.

The file containing the references is located at ''document\other'.

## Repo Usage

Create or Clone own empty repository:

```
git remote add template git@github.com:FHV-ITM13/Latex-Documents.git
git pull template fhvthesistemplate 
```

See: [2.5 Git Basics - Working with Remotes](http://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes)
