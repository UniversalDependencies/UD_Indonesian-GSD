# Summary

The Indonesian UD is converted from the content head version of the [universal
dependency treebank v2.0 (legacy)](https://github.com/ryanmcd/uni-dep-tb).


# Introduction

Lemmas, XPOS and morphological features added by MorphInd
(created by Septina Dian Larasati, run and converted by Dan Zeman,
http://septinalarasati.com/morphind/).

# Changelog

* 2019-11-15 v2.5
  * Google gave permission to drop the "NC" restriction from the license.
    This applies to the UD annotations (not the underlying content, of which Google claims no ownership or copyright).
* 2018-03-01 v2.2
  * Added lemmas and morphological features from MorphInd.
* 2017-03-01 v2.0
  * Converted to UD v2 guidelines (Dan Zeman).
  * Reduplicative plurals are now connected neither with mwe nor with fixed,
    but with compound:plur
    (https://github.com/UniversalDependencies/docs/issues/238)
* 2015-05-01 v1.1
  * Initial release (Ryan McDonald).



```
===================================
Universal Dependency Treebanks v2.0
(legacy information)
===================================

=========================
Licenses and terms-of-use
=========================

For the following languages

  German, Spanish, French, Indonesian, Italian, Japanese, Korean and Brazilian
  Portuguese

we will distinguish between two portions of the data.

1. The underlying text for sentences that were annotated. This data Google
   asserts no ownership over and no copyright over. Some or all of these
   sentences may be copyrighted in some jurisdictions.  Where copyrighted,
   Google collected these sentences under exceptions to copyright or implied
   license rights.  GOOGLE MAKES THEM AVAILABLE TO YOU 'AS IS', WITHOUT ANY
   WARRANTY OF ANY KIND, WHETHER EXPRESS OR IMPLIED.

2. The annotations -- part-of-speech tags and dependency annotations. These are
   made available under a CC BY-SA 4.0. GOOGLE MAKES
   THEM AVAILABLE TO YOU 'AS IS', WITHOUT ANY WARRANTY OF ANY KIND, WHETHER
   EXPRESS OR IMPLIED. See attached LICENSE file for the text of CC BY-NC-SA.

Portions of the German data were sampled from the CoNLL 2006 Tiger Treebank
data. Hans Uszkoreit graciously gave permission to use the underlying
sentences in this data as part of this release.

Any use of the data should reference the above plus:

  Universal Dependency Annotation for Multilingual Parsing
  Ryan McDonald, Joakim Nivre, Yvonne Quirmbach-Brundage, Yoav Goldberg,
  Dipanjan Das, Kuzman Ganchev, Keith Hall, Slav Petrov, Hao Zhang,
  Oscar Tackstrom, Claudia Bedini, Nuria Bertomeu Castello and Jungmee Lee
  Proceedings of ACL 2013

=======
Contact
=======

ryanmcd@google.com
joakim.nivre@lingfil.uu.se
slav@google.com
See https://github.com/ryanmcd/uni-dep-tb for more details
```



=== Machine-readable metadata =================================================
Data available since: UD v1.1
License: CC BY-SA 4.0
Includes text: yes
Genre: news blog
Lemmas: automatic
UPOS: converted from manual
XPOS: automatic
Features: automatic
Relations: converted from manual
Contributors: McDonald, Ryan; Nivre, Joakim; Zeman, Daniel; Larasati, Septina Dian
Contributing: to be adopted
Contact: zeman@ufal.mff.cuni.cz
===============================================================================
(Original treebank contributors: LaMontagne, Adam; Souček, Milan; Järvinen, Timo; Radici, Alessandra)
