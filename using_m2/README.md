# information on m2 grammatical correction extracting divergences

## what you need:
m2 files (with the same annotation scheme e.g. errant, to provide consisitency)

## process:
1) preprocessing.py - gets as an argument a directory with m2 files, it will then create
new files (one sentence on each line) one of the original sentences 
and one with the corrected sentences
2) run udpipe on these files to get 2 conllu files (one original, one corrected)
3) run GEC_UD_divergences/using_m2/GEC_UD_divergences_m2.py with original conllu file, corrected conllu file,
and matching m2 file. This will create files with confusion matrices.
