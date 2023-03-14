# Summary

The Indonesian-GSD treebank was originally converted from the content head version of the [universal dependency treebank v2.0 (legacy)](https://github.com/ryanmcd/uni-dep-tb) in 2015. In order to comply with the latest Indonesian annotation guidelines, the treebank has undergone a major revision between UD releases v2.8 and v2.9 (2021).


# Introduction

* The treebank consists of 5598 sentences and 122K words, and was divided into three parts:
  * Training dataset consists of around 97K words
  * Development dataset consists of around 12K words
  * Testing dataset consists of around 11K words


# Acknowledgments

* The original Indonesian-GSD treebank was developed by Ryan McDonald in 2015 based on the Indonesian treebank in a pre-UD Google treebank collection (McDonald et al. 2013).
* The treebank was converted to UD v2 guidelines by Dan Zeman in 2017.
* Lemmas, XPOS, and morphological features added by MorphInd (created by Septina Dian Larasati, run and converted by Dan Zeman, http://septinalarasati.com/morphind/), in 2018.
* Major corrections on word segmentation, LEMMA, UPOS, FEATS, and DEPREL columns by Dan Zeman and Ika Alfina, in 2021.

## References

* Ryan McDonald, Joakim Nivre, Yvonne Quirmbach-Brundage, Yoav Goldberg, Dipanjan Das, Kuzman Ganchev, Keith Hall, Slav Petrov, Hao Zhang, Oscar Tackstrom, Claudia Bedini, Nuria Bertomeu Castello and Jungmee Lee. ["**Universal Dependency Annotation for Multilingual Parsing**"](https://aclanthology.org/P13-2017.pdf). In Proceedings of ACL 2013.
* Septina Dian Larasati, Vladislav Kuboň, and Daniel Zeman, ["**Indonesian Morphology Tool (MorphInd): Towards an Indonesian Corpus**"](https://link.springer.com/chapter/10.1007/978-3-642-23138-4_8). In Proceeding of SCFM 2011.


# Changelog
* 2023-05-15 v2.12
  * Punctuation gets XPOS tag Z-- even if MorphInd failed to tag it.
* 2022-11-15 v2.11
  * Fixed the 'too-many-subjects' errors
* 2022-05-15 v2.10
  * The MISC attribute with the analysis from MorphInd renamed to Morf, as similar attributes in other UD treebanks.
  * Fixed the annotation for 'goeswith'
* 2021-11-15 v2.9
  * Numerous legacy validation errors fixed.
  * Corrections on tokenization/word segmentations:
    * The enclitics -ku, -mu, -nya, -kah, -lah, -pun, -tah separated from their host as syntactic words.
    * The proclitics ku-, kau- separated as 1Sing/2Sing subjects ('I, you').
    * Fixed tokenization of ordinal numerals.
    * Fixed tokenization of decades ('1990-an').
    * Fixed tokenization for morphemes anti-, non-, sub-, multi-, kontra-
    * Fixed tokenization for reduplicated verbs, nouns, etc.
  * Corrections on lemmas:
    * Stripped affixes from lemmas of verbs, nouns
  * Corrections on UPOS:
    * Fixed tags of ordinal numerals.
    * Fixed tags of words that should be AUX
    * Fixed numerous other incorrect tags (mislabeled NOUN as VERB, or vice-versa)
  * Corrections on features:
    * Applied new features: Abbr (value: Yes), Definite (values: Def, Ind), Mood (values: Ind, Imp), Reflex (value: Yes), Typo (value: Yes)
    * Applied new feature-values: NumType=Ord, PronType=Art, PronType=Emp
    * Removed features: Gender, Number[psor], Poss, Person[psor]
    * Removed feature-value: Degree=Pos
    * Proper nouns do not have the Number feature (unlike common nouns).
  * Corrections on dependency relations:
    * Applied 12 new subtypes for Indonesian, such as acl:relcl, advmod:emph, case:adv, cc:preconj, etc.
    * Fixed numerous incorrect DEPRELs
    * Fixed some udapi bugs (multi-subj, multi-obj, etc)
  * Added text_en (English translation of each Indonesian sentence was generated using Google Translate)
* 2021-05-15 v2.8
  * Fixed non-projective punctuation with Udapi ud.FixPunct.
  * Reduplicated plurals are now single tokens as in the other Indonesian treebanks.
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
Lemmas: automatic with corrections
UPOS: converted with corrections
XPOS: automatic with corrections
Features: automatic with corrections
Relations: converted with corrections
Contributors: McDonald, Ryan; Nivre, Joakim; Zeman, Daniel; Larasati, Septina Dian; Alfina, Ika
Contributing: here
Contact: zeman@ufal.mff.cuni.cz
===============================================================================
(Original treebank contributors: LaMontagne, Adam; Souček, Milan; Järvinen, Timo; Radici, Alessandra)
