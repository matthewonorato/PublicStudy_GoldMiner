# Public Study Workflow 
**define search terms → search GEO/SRA/ENA → select best studies → collect metadata → download samples → create sample sheet for alignment**

**Goal:** Since all companies use public data, the goal is to find gold standard studies quickly. Ultimately, we want to work with the most reliable, sufficiently powered studies. Starting with a few search terms, this pipeline will do the following:
- **Script 1:** Collect relevant studies from GEO, SRA, and ENA based on your query
	- Example (GEO query): 'Retinitis pigmentosa[All Fields] AND Homo sapiens[Organism] AND 10:1000[Number of Samples] AND "expression profiling by high throughput sequencing"[DataSet Type]'
- **Script 2:** For each selected study, add metadata (biological and technical variables, md5 check status, read lengths, strandedness), download samples (fastq files), and create sample sheet for alignment (RNA-Seq alignment pipeline)
