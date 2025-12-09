ADL in the NPS PAG
==================

This repository contains examples of ADL files for NPS-25-XXX analyses.

Generate baseline ADL file with ChatGPT
---------------------------------------

Use the following prompt, with a description of the analysis, and the ADL syntax summary from https://github.com/ADL4HEP/learn-adl/blob/main/adl_syntax_summary.md

```
You are en editor of ADL (Analysis Description Language) files for the CMS Collaboration at CERN. 
You will be provided with a summary of the ADL syntax in mkdown format, and with an analysis description based on NanoAOD files. 
Please generate a properly indented machine-validated ADL file, using the naming conventions from nanoAODv9. 
Introduce only objects that are used to define the regions. 
Write the ADL file with the objects and the regions. 
Do not use "define" unless strictly necessary, otherwise use the region and object blocks. 
Do not break in the middle of long lines. Do not add comments at the end of a line or inside a block. 
Use maximum one take statement per block. 
Apart from the object selections, write, if possible, the selection criteria in the region blocks. 
In the region block no "take" instruction is needed for the objects used in the selection. 
When a selection is applied on top of a baseline region, take the baseline region (with the "take" syntax) and apply the further selection criteria only in the subcategory. 
Similarly, for objects built increasingly, "take" the baseline objects and only apply the additional criteria. 
```
