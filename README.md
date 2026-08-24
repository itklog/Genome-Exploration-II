# Genome-Exploration-II

## Species Info

- **Species:** *Panthera pardus* (Leopard)
- **NCBI Assembly Accession:** `GCF_024362965.1`

### Objective

To evaluate the genome assembly structure and contiguity of *Panthera pardus* by analyzing sequence statistics, applying a 10 kb length filter, and examining the longest scaffolds and their contribution to the genome assembly.

### Tools and Parameters Used

1. **Fasta Statistics:** Default settings were used to determine total assembly length, sequence count, N50, and GC content.
2. **Filter Sequences by Length:** A minimum length cutoff of **10,000 bp (10 kb)** was applied to remove short scaffolds.
3. **Compute Sequence Length:** Used to determine the length of individual scaffolds and identify the longest sequences.
4. **Sort Dataset:** Scaffold lengths were sorted in descending order to identify the **15 longest scaffolds**.
5. **getorf:** Standard genetic code, protein translation output, and default minimum size threshold were used to identify and translate Open Reading Frames (ORFs).
6. **Bar Chart Visualization:** A bar chart was generated to visualize the lengths of the **15 longest scaffolds** and assess assembly contiguity.

### Key Findings

- The original assembly contained **382 sequences**, which decreased to **322 sequences** after the 10 kb filter.
- Filtering removed **60 short scaffolds** but caused only a negligible decrease in total assembly length (~0.0002 Gb).
- **N50 remained at 126.8 Mb**, indicating that short scaffolds had little effect on assembly contiguity.
- The **15 longest scaffolds** ranged from approximately **89 to 205 Mb**, demonstrating the presence of large, chromosome-scale scaffolds.
- The **GC content remained stable at 41.75%**, indicating no substantial compositional change after filtering.

## Analysis Results Summary

The assembly contained **382 sequences**, which decreased to **322** after filtering at ≥10 kb. This removed **60 short scaffolds** but caused only a negligible loss in assembly length (~0.0002 Gb), while **N50 (126.8 Mb)** and **GC content (41.75%)** remained unchanged. The 15 longest scaffolds ranged from approximately **89 to 205 Mb**, indicating that the assembly is dominated by large, chromosome-scale scaffolds.

**Full Results Table:** [`results_table.md`](results_table.md) or [`results_table.csv`](results_table.csv)

## Genome Interpretation

The *Panthera pardus* assembly represents a highly contiguous genome, with half of the approximately **2.44 Gb** assembly contained in only eight scaffolds (**N50 = 126.8 Mb; L50 = 8**). The longest scaffold reaches approximately **204.9 Mb**, consistent with chromosome-scale continuity.

Although many short scaffolds are present, their contribution to total genome size is negligible, as shown by the minimal change after filtering below **10 kb**. The stable **GC content of 41.75%** indicates that filtering did not introduce substantial compositional bias.

ORF analysis demonstrated that open reading frames can be identified within the assembly; however, ORFs alone do not confirm functional genes and require supporting evidence such as genome annotation, transcriptomic data, or protein homology.

Overall, the results indicate a highly contiguous, chromosome-scale assembly in which long scaffolds provide most of the genome representation.

## Visual Evidence and Screenshots
The following figures document the Galaxy workflow and the main assembly
statistics obtained during the analysis of the *Panthera pardus* genome.
These outputs provide evidence of the analysis steps used to evaluate
genome assembly structure and contiguity.

### **Figure 1. Galaxy History and Analysis Workflow**

The Galaxy History shows the sequence of tools used to characterize the
*Panthera pardus* genome assembly, including assembly statistics,
sequence-length filtering, scaffold-length calculation and sorting,
ORF identification, and visualization of the longest scaffolds.

<img width="2560" height="1600" alt="1000040605" src="https://github.com/user-attachments/assets/af6e0cd2-aa6f-456a-b126-feb0a01132bf" />


**Figure 1.** Galaxy History showing the workflow used to analyze the
*Panthera pardus* genome assembly (`GCF_024362965.1`).



### **Figure 2. Assembly Summary Statistics**

The assembly summary statistics provide the main characteristics of the
*Panthera pardus* genome assembly before and after applying the 10-kb
sequence-length filter. These statistics include the total number of
sequences, total assembly length, N50, L50, and GC content.

<img width="2560" height="1600" alt="ad07b12a-d6bc-4234-b353-7dafd3942b58-1_all_6554" src="https://github.com/user-attachments/assets/443e9804-385d-41b0-9703-8f468f6acf9d" />

**Figure 2.** Summary statistics of the *Panthera pardus* genome assembly
showing assembly size, sequence count, N50, L50, and GC content before
and after filtering.



## Galaxy History & Reproducibility
[🔗 View Complete Analysis History on Galaxy](https://usegalaxy.org/u/eugene_7/h/genome-exploration-ii-ansag-panthera-pardus)


