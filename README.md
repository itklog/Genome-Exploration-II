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

### Interpretation

The *Panthera pardus* assembly is characterized by high contiguity, with most of the genome represented by a small number of large, chromosome-scale scaffolds. The minimal effect of removing short scaffolds further supports the quality and chromosome-level structure of the assembly.
