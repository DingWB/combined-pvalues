A library to combine, analyze, group and correct p-values in BED files.
Unique tools involve correction for spatial autocorrelation.
This is useful for ChIP-Seq probes and Tiling arrays, or any data with spatial
correlation.

Forked from https://github.com/brentp/combined-pvalues

## Installation
```shell
# uninstall
pip uninstall cpv
pip install git+https://github.com/DingWB/combined-pvalues
```

## Documentation
```
acf   - calculate autocorrelation within BED file (output is: *.acf.txt)
slk   - Stouffer-Liptak-Kechris correction of spatially correlated p-values (*.slk.bed.gz, one more col: combined-pval)
fdr   - Benjamini-Hochberg correction of p-values (*cpv.fdr.bed.gz, corrected pval)
peaks - find peaks in a BED file (*regions.bed.gz)
region_p  - generate SLK p-values for a region (*.regions-p.bed.gz, Stouffer-Liptak p-value of the region and the Sidak correction of that p-value)
manhattan - a manhattan plot of values in a BED file.
pipeline  - run the series of commands to find DMRs.
```

### dist
300 bp, ref: BSmooth
500 bp, ref: Human body epigenome maps reveal noncanonical DNA methylation variation