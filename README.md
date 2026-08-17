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

## Visual Evidence & Screenshots
Screenshots of the Galaxy workflow and sequence statistics  results are provided as evidence of the analysis steps and outputs.


**Figure 1.** Screenshot showing the genome uploaded in Galaxy.
![Figure 3. 15 Longest Scaffolds](Screenshot evidence Figure 1.png)

**Figure 2.** Screenshot showing the summary statistics of the Felis pardus genome assembly.
![Figure 3. 15 Longest Scaffolds](Screenshot evidence figure 2.png)


## Galaxy History & Reproducibility

**Shared Galaxy History:** [View Complete Analysis History on Galaxy]([https://usegalaxy.org/](https://usegalaxy.org/u/eugene_7/h/genome-exploration-ii-ansag-panthera-pardus)...)
