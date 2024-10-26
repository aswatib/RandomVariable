---
title: "metaDMM"
layout: default
---

# metaDMM for Metagenomics
Metagenomics has risen into a transformative field that allows researchers to study the genetic material of entire microbial communities directly from environmental samples, providing unprecedented insights into microbial diversity, functions, and interactions.

When we talk about microbiome data, we're usually referring to the relative abundances of different microbial species in a sample. This data is compositional because it describes the proportions of microbes relative to each other, rather than absolute counts.

During my master thesis project, I got a chance to generate synthetic abundance data reflecting a microbial composition similar to that of a sewage environment. In order to simulate FASTQ reads as if generated from a sequencer, I applied a Python script ensuring that the reads representing individuals were present with a specific distribution on a taxon level – species in this case.

The distribution model that I used for this simulation was Dirichlet-Multinomial – a compound modeling method that explains two significant aspects of microbiome abundance data: the multinomial component explains the counts of different species in each sample, and the Dirichlet components explains the variation of each species across samples.

The metaDMM method allows you to generate synthetic microbiome reads with this underlying Dirichlet-Multinomial distribution – although it still has a few areas of improvement.



<script src="https://utteranc.es/client.js"
        repo="RandomVariable"
        issue-term="pathname"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>
