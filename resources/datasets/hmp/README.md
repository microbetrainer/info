
The raw data for HMP can be accessed on SRA via the run browser
([here](https://www.ncbi.nlm.nih.gov/Traces/study/?acc=SRP002395)).
Using sratoolkit's fastq-dump, it's easy to get fastq's from this.
However, it seems that some of the runs are deconvoluted whereas others
still have multiple samples in each SRR file. The "SFF and Library 
Metadata File Generation" [documentation](http://hmpdacc.org/doc/SFF_LibraryMetadataFiles_SOP.pdf)
on the [HMR16S page](http://hmpdacc.org/HMR16S/) explains this.

From the "16S rRNA Processing" [documentation](http://hmpdacc.org/doc/16S_SOP.pdf)
on the [HM16STR page](http://hmpdacc.org/HM16STR/)
(trimmed data), it looks like de-convoluting these files was not trivial.

tl;dr - it's probably best to just use the trimmed, deconvoluted fasta
files in HM16STR. Thankfully Chris and Scott already did the hard work
of downloading all those files! Files and associated documentation are
on coyote: /net/radiodurans/alm/lab/data/hmp/trim/