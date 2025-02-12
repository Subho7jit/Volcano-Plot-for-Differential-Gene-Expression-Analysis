# Volcano-Plot-for-Differential-Gene-Expression-Analysis
Description:
This script generates a volcano plot to visualize differentially expressed genes (DEGs) based on log fold change (logFC) and p-value thresholds. The plot highlights significantly upregulated and downregulated genes, aiding in the identification of potential biomarkers.

Steps Involved:
Load Required Packages:

The script checks for and installs the ggplot2 package if not already available.
Set Working Directory & Load Data:

The working directory is set to "C:\\Users\\Gobin\\Downloads".
The script reads gene expression data from a CSV file (DEGs_totall.csv).
Define Significance Thresholds:

Log Fold Change (logFC) threshold: ±1
P-value threshold: 0.05
Generate the Volcano Plot:

Each gene is plotted based on its logFC (x-axis) and -log10(PValue) (y-axis).
Genes are colored based on significance:
Red: Upregulated (logFC > 1, p < 0.05)
Blue: Downregulated (logFC < -1, p < 0.05)
Black: Non-significant genes
Horizontal and vertical dashed lines indicate p-value and logFC thresholds.
The y-axis limit is set to 0–18 for better visualization.
