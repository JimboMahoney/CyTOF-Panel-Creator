# CyTOF-Template-Creator
A web-based (Shiny) [interface](https://jimbomahoney.shinyapps.io/shiny/) to create CyTOF .tem files.

This allows (hopefully) easy creation of .tem files, which can then be loaded onto a CyTOF system for acquisition.

Last updated: 10th Jan 2020.

## Motivation:

- It seems unnecessary to download and install (CyTOF) software on an offline system to create an acquisition template.
- Creating a template at the machine (based on an e-mail or Excel file from a user) is risky unless the user is present to verify.
- There is no error-checking in the CyTOF software (e.g. it's easy to miss essential channels, such as EQ beads).
- Just for fun! It's the first time I've built and uploaded a Shiny app.

## Functionality:

- Default template containing common contaminants, barcodes and Cell ID (Live/Dead, Ir).
- Quickly create template for the [Direct Immune Profiling Assay](https://www.fluidigm.com/reagents/proteomics/201325-maxpar-direct-immune-profiling-assay).
- Upload template from Excel file (file must have headers for columns and mass/element in first column; target/markers in second column).
- Easy Add/Remove of Barcodes, Cell-ID, Bead (EQ), Contaminants and Blank (M +/- 1 plus isotopic impurities and +16 oxidation) channels.
- Easy swap of Live/Dead marker (Pt195 or Rh103).
- Lookup of isotope by mass or name.
- Sorting of Panel by mass or name.
- Save as .tem file ready for use on CyTOF.

## Error-Checking:

Checks to ensure that:

- All essential normalisation channels are present.
- Illegal characters are not present in the Target names. (This is a limitation imposed by CyTOF software).
- Cell ID (Ir) is present.

<br>



[![Foo](https://raw.githubusercontent.com/JimboMahoney/CyTOF-Panel-Creator/master/2019_11_22_14_12_17_CyTOF_Template_Creator.png)](https://jimbomahoney.shinyapps.io/shiny/)

## Disclaimer:
As with any software, this may have bugs and is used <b>at your own risk.</b>
<br>
<br>
This is not an official product of nor endorsed by Fluidigm or anyone else.
<br>
<br>
Before acquiring any data on an instrument, you should double-check that all channels / parameters are present! 
<br>
<br>
Having said that, this tool was specifically designed to <b>reduce</b> the likelihood of missing channels. It's more likely that you will acquire <b>more</b> data using this template creator!
<br>
Tested on a Helios running CyTOF software version 6.7.1014, using default Event mode parameters.

