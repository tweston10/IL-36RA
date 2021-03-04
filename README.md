# IL-36RA
 
Data relating to the interleukin-36 receptor antagonist protein (IL-36RA) in complex with Interleukin-1 Receptor-Like 2 (IL1RL2) and associated computational metrics/representations.

## Data files

`il36ra.pdb` - PDB file with structure coordinates for L-36RA+IL1RL2 complex

`data.xlsx` - Excel workbook with database data from ZoomVar, gnomAD, ClinVar, and Delta-SASA scores computed by POPSCOMP. Constituent data files can be accessed more readily:
* `gnomAD_v2.1.1_IL36RA_2021_03_03_15_40_29.csv` - gnomAD 2.1.1 missense variant data for IL-36RA (comma-delimited)
* `gnomAD_v3.1_IL36RA_2021_03_03_15_42_35.csv` - gnomAD 3.1 missense variant data for IL-36RA (comma-delimited)
* `clinvar_result_IL36RA.txt` - ClinVar missense SAV data for IL-36RA (tab-delimited)
* `residueSASA_il36ra.csv` - POPSCOMP SASA values for all residues in IL-36RA+IL1RL2 complex (comma-delimited)
* `residueIsoSASA_il36ra.csv` - POPSCOMP SASA values for all residues in IL-36RA and IL1RL2 without the other present (comma-delimited)
* `residueDeltaSASA_il36ra.csv` - POPSCOMP change in SASA values for residues in IL-36RA+IL1RL2 complex on going from isolated molecules to complex (comma-delimited)

## Session Files

`Graded_Heat_Map.pse` - Mapping of mCSM predicted stability change to position in IL-36RA+IL1RL2 complex, using count of saturation mutagenesis residue changes predicted destabilising out of 19 (via G. Rinaldi)
* Green = 0 predicted destabilising
* Yellow = 1-6 predicted destabilising
* Orange = 7-11 predicted destabilising
* Red = 12-16 predicted destabilising
* Dark Red = 17-19 predicted destabilising

`il36ra_gnomad_common.pse` - Mapping of common gnomAD IL-36RA missense variant positions (MAF > 0.0001 in either gnomAD 2.1.1 or gnomAD 3.1) onto IL-36RA+IL1RL2 complex structure
* Cyan = gnomAD (common)

`il36ra_gnomad_rare.pse` - Mapping of rare gnomAD IL-36RA missense variant positions (MAF > 0.0001 in either gnomAD 2.1.1 or gnomAD 3.1) onto IL-36RA+IL1RL2 complex structure
* Magenta = gnomAD (rare)

`il36ra_clinvar_all.pse` - Mapping of all IL-36RA missense variant positions in ClinVar onto IL-36RA+IL1RL2 complex structure
* Purple = ClinVar

`il36ra_clinvar_sig.pse` - Mapping of all IL-36RA missense variant positions in ClinVar onto IL-36RA+IL1RL2 complex structure by significance
* Green = Benign
* Yellow = Uncertain Significance
* Orange = Contested Pathogenicity
* Red = Pathogenicity

`il36ra_super_all.pse` - Mapping of all IL-36RA missense variant positions onto IL-36RA+IL1RL2 complex structure (priority: gnomAD common > ClinVar > gnomAD rare)
* Cyan = gnomAD (common)
* Purple = ClinVar
* Magenta = gnomAD (rare)

`interface.pse` - Mapping of all positions in IL-36RA at the interface in IL-36RA+IL1RL2 complex structure, according to POPSCOMP Delta-SASA calculation
* Yellow = Delta-SASA > 0
* Orange = Delta-SASA > 1
* Red = Delta-SASA > 10

## Input files

Input files for colouring above session files.
* `gnomad_common.txt`
* `gnomad_rare.txt`
* `clinvar_all.txt`
* `clinvar_sig.txt`
* `super_all.txt`
* `interface_chainA.txt`
