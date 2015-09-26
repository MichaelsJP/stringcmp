# strcmp
String comparison functions from FEBRL

```
  exact          Exact comparison
  jaro           Jaro
  winkler        Winkler (based on Jaro)  (for backwards compatibility)
  qgram          q-gram based
  bigram         2-gram based  (for backwards compatibility)
  posqgram       Positional q-gram based
  sgram          Skip-gram based
  editdist       Edit-distance (or Levenshtein distance)
  mod_editdist   Modified edit-distance (with transposition cost 1, not 2)
  bagdist        Bag distance (cheap distance based method)
  swdist         Smith-Waternam distance
  syllaligndist  Syllable alignment distance
  seqmatch       Uses Python's standard library 'difflib'
  compression    Based on Zlib compression algorithm
  lcs            (Repeated) longest common substring, improves results for
                 swapped words
  ontolcs        Ontology alignment string comparison based on longest common
                 substring, Hamacher product and Winkler heuristics.
  permwinkler    Winkler combined with permutations of words, improves results
                 for swapped words
  sortwinkler    Winkler with sorted words (if more than one), improves results
                 for swapped words
  editex         Phonetic aware edit-distance (Zobel et al. 1996)
  twoleveljaro   Apply Jaro comparator at word level, with words being compared
                 using a selectable approximate string comparison function
  charhistogram  Get histogram of characters for both strings and calculate the
                 cosine similarity between the two histogram vectors
```
