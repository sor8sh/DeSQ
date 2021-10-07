# SPEQ: Spectrum Quality

High-Throughput Quality Assessment of Peptide Tandem Mass Spectra

---

This is the source code for the first version of SPEQ.
To run the program, run the `speq.py` python file with python3.

### MS input data:
* The MS input data should be in MGF format. 
* The data file is then automatically generated by the program.

### Labels:
* A database search result in `.tsv` format (MS-GF+ output) is used to generate the labels file.
* The decoy prefix used in the database-searching should be defined in the `config.yml` file. The program uses 1% FDR.
* If you want, you can provide your own `label.csv` file.
  It should be a one-column file where each row specifies the label for the spectrum with the scan number equal to the number of the line
  (e.g. If you have a spectrum with scan number 7, then the 7th row of the `label.csv` file should be the label for that spectrum).
