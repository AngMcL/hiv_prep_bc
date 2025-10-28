* unaligned files were exported from the data cleaning script, moved into 00_unaligned
    * uniqID or uniqSamp, pol or integrase
* next, add HXB2 reference and for pol, the DRM reference (ref and DRMs in 01_...; modf'd fasta in 02_intermediate)
* align intermediate files using mafft --auto file.fasta > file_aligned.fasta
* trim the alignments of DRMs and frayed ends, remove reference
* use this alignment "trimmed_noref" for building phylogenies
