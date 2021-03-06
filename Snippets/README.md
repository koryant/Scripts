#Snippets

[BAR][Home] Snippets. This directory is a depository of generic and reusable templates to be recycled
by BAR users. They are installed under `BAR>Snippets>`, a menu containing several other commands:

 - `List Snippets`: Prints the contents of this directory to a dedicated window. Files can then be
   opened in the Script Editor by double-click. This may be preferable to
   [Shift-clicking](http://fiji.sc/BAR#OpeningBAR) the Menu bar
 - `Reveal Snippets`: Opens this directory in the file browser of the operating system
 - [`New Snippet...`](../BAR/README.md#bar-plugins): A Java plugin implementing a convenient way to
   generate new scripts. The prompt features a drop-down menu containing source code that pre-loads
   scripting additions stored in the [lib](../lib/README.md#lib) directory.
   ([Source code](../BAR/src/main/java/bar/plugin/SnippetCreator.java))

   [![SnippetCreator](http://fiji.sc/_images/d/de/SnippetCreator.png)](http://fiji.sc/BAR#Snippets)


##List of Snippets
####[Median Filter](./Median_Filter.py)
A [Python](#python) script that exemplifies how to perform a filtering operation.
([Download .py](./Median_Filter.py?raw=true))

####[NN Distances](./NN_Distances.py)
A [Python](#python) script that calculates nearest neighbor distances from a 2D/3D list of centroid
coordinates.
([Download .py](./NN_Distances.py?raw=true))

####[Batch Processors](http://fiji.sc/BAR#Batch_Processors)
These are scripts written in different languages that batch process images in a more customizable
way than the _Process>Batch>Macro_ built-in command. The scripts are modular in design, so that
routines to be applied to individual files are contained in a single function. Each _Batch Processor_
performs the following operations ([documentation page](http://fiji.sc/BAR#Batch_Processors)):

 1. Take an input folder specified by the user
 2. Apply a series of operations to individual files of matched extension(s)
 3. Save processed files to a dedicated directory, so that no files are overwritten

In the current examples, both the Python (Jython) and ImageJ macro (IJM) implementation perform the
task of obfuscating filenames: 1) They copy images from one folder to another, 2) Rename their
filenames using a random string and 3) Log changes to a CSV table (so that id of randomized filename
can be traced back to the original file). This approach is useful for unbiased/blind analyses that
are sensitive to user interpretation.

#####[Process Folder IJM](./Process_Folder_IJM.ijm)
A batch processor written in the [IJ macro language](#imagej-macro-language).
([Walkthrough](http://fiji.sc/BAR#IJ_Macro_Language))
([Download .ijm](./Process_Folder_IJM.ijm?raw=true))

#####[Process Folder PY](./Process_Folder_PY.py)
A batch processor written in [Python](#python).
([Walkthrough](http://fiji.sc/BAR#Python))
([Download .py](./Process_Folder_PY.py?raw=true))


####[Search BAR](./Search_BAR.bsh)
   A BeanShell script that searches for content in this directory.
   ([Download .bsh](./Search_BAR.bsh?raw=true))

##Useful Resources

####Scripting additions
 - [lib]

####ImageJ Macro Language
 - [Introduction into Macro Programming](http://fiji.sc/Introduction_into_Macro_Programming)
 - [Built-in macro functions](http://imagej.nih.gov/ij/developer/macro/functions.html)
 - [IJ1 developer resources](http://imagej.nih.gov/ij/developer/index.html)
 - [IJ1 macro repository](http://imagej.nih.gov/ij/macros/)
 - Fiji examples in `Fiji.app/plugins/Examples/` and Editor's _Templates_ menu

####Python
 - [Fiji documentation](http://fiji.sc/Jython_Scripting)
 - [Image Processing and Analysis @EMBL](http://cmci.embl.de/documents/120206pyip_cooking/python_imagej_cookbook)
 - [IJ1 examples](http://imagej.nih.gov/ij/macros/python/)
 - [Python documentation](https://www.python.org/doc/)
 - [Jython documentation](http://www.jython.org/docs/)
 - [Python Central](http://www.pythoncentral.io)
 - [The Hitchhiker’s Guide to Python](http://docs.python-guide.org/en/latest/)
 - Fiji examples in `Fiji.app/plugins/Examples/` and Editor's _Templates_ menu




| [Home] | [Analysis] | [Data Analysis] | [Annotation] | [Segmentation] | [Tools] | [Plugins] | [lib] | [Snippets] | [Fiji] |
|:------:|:----------:|:---------------:|:------------:|:--------------:|:-------:|:---------:|:-----:|:----------:|:------:|

[Home]: https://github.com/tferr/Scripts#ij-bar
[Analysis]: https://github.com/tferr/Scripts/tree/master/Analysis#analysis
[Data Analysis]: https://github.com/tferr/Scripts/tree/master/Data_Analysis#data-analysis
[Annotation]: https://github.com/tferr/Scripts/tree/master/Annotation#annotation
[Segmentation]: https://github.com/tferr/Scripts/tree/master/Segmentation#segmentation
[Morphometry]: https://github.com/tferr/Scripts/tree/master/Morphometry#morphometry
[Tools]: https://github.com/tferr/Scripts/tree/master/Tools#tools-and-toolsets
[Plugins]: https://github.com/tferr/Scripts/tree/master/BAR#bar-plugins
[lib]: https://github.com/tferr/Scripts/tree/master/lib#lib
[Snippets]: https://github.com/tferr/Scripts/tree/master/Snippets#snippets
[Fiji]: http://fiji.sc/BAR
