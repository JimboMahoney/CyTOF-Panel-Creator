# CyTOF-Panel-Creator
A web-based (Shiny) [interface](https://jimbomahoney.shinyapps.io/shiny/) to create CyTOF .tem files.

This allows (hopefully) easy creation of .tem files, which can then be loaded onto a CyTOF system.

Currently, it performs the following:

Checks to ensure that:

- All essential normalisation channels are present.
- Illegal characters are not present in the Target names. (This is a limitation imposed by CyTOF software)
- Cell ID (Ir / Rh) is present

Provides the following functionality:

- Default Template containing common contaminants, barcodes and Cell ID (Live/Dead, Ir)
- Easy Add/Remove of Barcodes, Bead (EQ), Contaminants and Blank (M +/- 1) channels.
- Lookup of isotope by mass or name.
- Sorting of Panel by mass or name.
- Save as .tem file ready for use on CyTOF.

<br>

<img src="https://raw.githubusercontent.com/JimboMahoney/CyTOF-Panel-Creator/master/2019_11_22_14_12_17_CyTOF_Template_Creator.png"
  align="center" />


