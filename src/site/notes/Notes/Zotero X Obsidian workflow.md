---
{"dg-publish":true,"permalink":"/notes/zotero-x-obsidian-workflow/","tags":["publish, compiled"]}
---


# Zotero X Obsidian workflow
To have literature manager that at the same time connected to more robust plan text - markdown file manager, the Obsidian.

1. Install Zotero
2. From [zetero web page](https://www.zotero.org/support/plugins), find the link to these plugin
	1. **[ZotFile](http://www.zotfile.com/ "http://www.zotfile.com")**
	2. **[Mdnotes for Zotero](https://github.com/argenos/zotero-mdnotes "https://github.com/argenos/zotero-mdnotes")**
	- Download the .xpi file.
	- On zotero, tools > Add-ons 
	- Drag the .xpi file to the Add-ons manager window
	- Zotero need to restart
3. Import paper to zotero
4. Add annotation
5. In the parent item, right click > add note from annotation. Then the new note under parent item will appear
6. In the note that appear, right click > Export Note.. export it as markdown
7. You can put directly to your obsidian vault

-------
# A more comprehensive one
## Plugins needed
### Zotero
- [Zotfile](http://zotfile.com/)
	Zotfile is a Zotero plugin to manage your attachments: automatically rename, move, and attach PDFs (or other files) to Zotero items, sync PDFs from your Zotero library to your (mobile) PDF reader (e.g. an iPad, Android tablet, etc.) and extract annotations from PDF files.
- [Mdnotes for Zotero](https://github.com/argenos/zotero-mdnotes "https://github.com/argenos/zotero-mdnotes")
	Export item metadata and notes as Markdown files
- [BetterBibtex](https://retorque.re/zotero-better-bibtex/)
	Better BibTeX (BBT) is an extension for [Zotero](https://www.zotero.org/) and [Juris-M](https://juris-m.github.io/) that makes it easier to manage bibliographic data, especially for people authoring documents using text-based toolchains (e.g. based on [LaTeX](https://www.latex-project.org/) / [Markdown](https://www.markdownguide.org/)).

### Obsidian
- [Citations](https://github.com/hans/obsidian-citation-plugin)
	The plugin supports reading bibliographies in [BibTeX / BibLaTeX `.bib` format](http://www.bibtex.org/) and [CSL-JSON format](https://github.com/citation-style-language/schema#csl-json-schema).
	-   If you use **Zotero** with [Better BibTeX](https://retorque.re/zotero-better-bibtex/):
    -   Select a collection in Zotero's left sidebar that you want to export.
    -   Click `File` -> `Export library ...`. Select `Better BibLaTeX` or `Better CSL JSON` as the format. (We recommend using the BibLaTeX export unless you experience performance issues. The BibLaTeX format includes more information that you can reference from Obsidian, such as associated PDF attachments, but loads more slowly than the JSON export.)
    -   You can optionally choose "Keep updated" to automatically re-export the collection -- this is recommended!
- [Pandoc Reference List](https://github.com/mgmeyers/obsidian-pandoc-reference-list)
- [Obsidian Enhancing Export](https://github.com/mokeyish/obsidian-enhancing-export)
- [Obsidian Link Converter](https://github.com/ozntel/obsidian-link-converter)


-------

### Simple way
1. At Zotero, at the paper you finished annotating. Right klik > Add note from annotation
2. At Zotero, file > Export library > 
	1. select "Better BibLaTex" 
	2. Export Notes, Use Journal Abbreviation
	3. Keep updated  --> select this so in the future you do not need to set it again. only need to press refresh in the  top right in the main windows of Zotero
	4. OK
3. Choose folder to save your My Library.bib (remember the address. need to setup at Obsidian)
4. at Obsidian, setting > open Citation plugin's setting, 
	1. set the "Citation database path" to be the path you saved the My Library.bib
	2. set the "literature note content template" at the 
	mine are:
	
6. Cmd+P > type "Citation" > select "Citation: Refresh citation database"
7. Cmd+P > type "Citation" > select "Citation: Open literature note"


Next time, replace step 2-3 to only click the refresh button in the top right of Zotero, no need to go to step 4 as well.


#### Linked notes
[[Notes/Why I choose Obsidian\|Why I choose Obsidian]]
