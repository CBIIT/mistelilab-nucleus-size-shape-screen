# mistelilab-nucleus-size-shape-screen

This is a repo containing the R code used to generate the RNAi screen results included in the [biorXiv pre-print manuscript](https://www.biorxiv.org/content/10.1101/2022.05.28.493845v1) from the Misteli Lab at the National Cancer Institute/NIH. The R code heavily uses the [cellHTS2 package](https://www.bioconductor.org/packages/release/bioc/html/cellHTS2.html).

**Title:** Identification of epigenetic modulators as determinants of nuclear size and shape

**Authors:** Schibler, Andria; Jevtic, Pedja; Pegoraro, Gianluca; Levy, Daniel L.; Misteli, Tom.

**DOI:** 10.1101/2022.05.28.493845

The code is mainly organized in two self-contained folders: `CRL-1474` containing the RNAi screen data for the hTERT-CRL-1474 fibroblast cell line, and `MCF10AT`, respectively. 

Each of these folders contains:

- An `.Rmd` script that includes the R and `cellHTS2` code used to analyze the results of the image analysis pipeline. 
- The well level results obtained from the Columbus image analysis server, which is contained in the `Columbus_output` subfolder. 
- The `Janus_output` subfolder contains library reformatting metadata output by the liquid handler and is used by the `.Rmd` script to generate the siRNA oligos layouts for the imaging plates used in the screen. 
- A `Description.txt` file that contains details about the screen according to the `cellHTS2`
- A series of subfolders whose name starts with `cellHTS2_output` containing the results of the `cellHTS2` analysis. Each of these subfolder contains data relative to one of the cellular features analyzed and output by Columbus. 

The subfolders containing RNAi screen results relevant for the manuscript are:

- `cellHTS2_output_Nuclei Selected - Nucleus Area [µm²] - Mean per Well`: These are data relative to nucleus area.

- `cellHTS2_output_Nuclei Selected - Nucleus Roundness - Mean per Well`: These are data relative to nucleus roundness.

For information about this repo, please contact [Tom Misteli](mailto:mistelit@nih.gov) or [Gianluca Pegoraro](mailto:gianluca.pegoraro@nih.gov)
