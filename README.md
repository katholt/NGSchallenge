# ASM NGS Challenge 2015
Data for the outbreak investigation software challenge session at the ASM NGS 2015 conference

##Pathogen Surveillance Software Demonstration

[2015 Rapid NGS Bioinformatic Pipelines for Enhanced Molecular Epidemiologic Investigation of Pathogens](http://conferences.asm.org/index.php/upcoming-conferences/2015-rapid-ngs-bioinformatic-pipelines-for-enhanced-molecular-epidemiologic-investigation-of-pathogens)

[Session Program](http://conferences.asm.org/index.php/upcoming-conferences/2015-rapid-ngs-bioinformatic-pipelines-for-enhanced-molecular-epidemiologic-investigation-of-pathogens/122-conferences/2015-rapid-ngs-bioinformatic-pipelines-for-enhanced-molecular-epidemiologic-investigation-of-pathogens/307-preliminary-program#Saturday)

## Instructions

###Overview

Please note that this challenge is comprised of sequence data from Salmonella and Listeria isolates collected in the field and from clinical sources. As the data is “real” there will undoubtedly be some ambiguity about inferred relationships of isolates that cannot be resolved. Participants are therefore encouraged in their presentations to provide details about how they arrived at their conclusion rather than simply showing the results.

For each data set participants are required to define what constitutes a match/inclusion, non-match/exclusion, and ambiguous/uncertain results. Examples of such criteria include cutoffs, thresholds, or odds/probabilities based on SNP, MLST, wgMLST, etc. 

Results should be recorded on the “Results” sheet of the attached spreadsheet describing the isolates. 

Participants are encouraged to submit supporting information, such as distance, SNP, MLST tables and matrices.

###Data Set 1: Listeria Monocytogenes

######BioProject [PRJNA295367](http://www.ncbi.nlm.nih.gov/bioproject/?term=PRJNA295367)

(SRA accessions provided in attached spreadsheet.)

Epidemiological investigations into a regional cluster of Listeria illnesses suggested that cheese was the source of the infection. Food histories of the affected individuals identified two different brands of cheese, from two different manufacturers, as the potentially contaminated food. Inspections were performed at the respective production facilities and 12 environmental positive swabs along with 4 isolates from finished product were obtained at facility #1. At facility #2 no isolates were obtained from product testing but 2 of the environmental swabs were positive for Listeria monocytogenes.

####Questions

1. Do the product isolates from facility #1 match the environmental swabs from facility #1? The manufacturer claims that since the positive swabs did not come from food contact surfaces the contamination must come from another source. Do the product isolates match any other food/environmental isolates currently in the NCBI/SRA database under BioProjects [PRJNA212117](http://www.ncbi.nlm.nih.gov/bioproject/?term=PRJNA212117) or [PRJNA215355](http://www.ncbi.nlm.nih.gov/bioproject/?term=PRJNA215355)?

2. Do the environmental/product isolates from either facility match clinical isolates in the BioProjects listed in question 1, or any other clinical Listeria monocytogenes isolates available from other public data sources? Can you identify the clinical cases associated with this contamination event?

###Data Set 2: Salmonella Enteritidis

######BioProject [PRJNA295366](http://www.ncbi.nlm.nih.gov/bioproject/?term=PRJNA295366)

(SRA accessions provided in attached spreadsheet.)

Epidemiologists have established that a small number of individuals (n=4) became ill with Salmonella after consuming eggs or egg products from a particular distributor. Traceback investigations have determined that the eggs came from laying houses in state #2 but the producer has multiple production farms and the origin of the contaminated eggs cannot be definitively determined. The producer also has laying houses at a single farm in state #1. FDA investigators collected food and environmental samples from facilities in each state and the isolates from positive samples are included in the data set.

####Questions

1. Do the 4 clinical isolates (ASM_26, ASM_31, ASM_49, and ASM_50) that are epidemiologically linked to eggs from state #2 match any of the environmental or food swabs collected at those facilities?

2. Do any of the remaining 19 clinical isolates match clinical isolates from question #1? Do they match any of the food or environmental isolates? Are there additional clinical clusters?

3. Are there other clinical Salmonella isolates in public databases (including, but not limited to, samples from BioProjects [PRJNA237212](http://www.ncbi.nlm.nih.gov/bioproject/?term=PRJNA237212), [PRJNA227458](http://www.ncbi.nlm.nih.gov/bioproject/?term=PRJNA227458), [PRJNA252015](http://www.ncbi.nlm.nih.gov/bioproject/?term=PRJNA252015), and [PRJNA230403](http://www.ncbi.nlm.nih.gov/bioproject/?term=PRJNA230403)) that match food or environmental isolates collected at these facilities in these two states?

## Downloading Data

SRR accessions are given in the spreadsheet and via the BioProject links below

Example Download - NCBI SRA toolkit installed and network access available 

Executing the command will produce two files, reads 1 and 2, for SRR accession SRR2352185:

    fastq-dump --split-files SRR2352185 
