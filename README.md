# ASC-annotation-guidelines

## 1. Purpose
Every instance of corpus annotation involves making decisions (Gerdes & Kahane, 2016). In this document, we discuss the rationale behind our choices in categorizing Argument Structure Construction (ASC) within an English corpus.

## 2. Basic unit

- We are interested in ASC annotations. By ASC annotation, we mean an annotation based on a syntactic/lexicogrammatical construction, wherein a verb and its argument structure consitute a form that corresponds to a propositional meaning (e.g., Diessel, 2004; Fillmore, Kay, & O’Connor, 1988; Goldberg, 1995; 2003; 2006; Jackendoff, 2002).

- For the annotation project, we used data, which is structured in the <a href="https://universaldependencies.org/format.html" target="_blank">CoNLL-U format</a>, which presents each sentence in a vertical arragement. In this format, the columns are presented in the following order:

```
    1. ID: Word index.
    2. FORM: Word form or punctuation symbol.
    3. LEMMA: Lemma or stem of word form (currently empty).
    4. UPOS: Universal part-of-speech tag.
    5. XPOS: Language-specific part-of-speech tag; underscore if not available.
    6. FEATS: List of morphological features from the universal feature inventory (currently empty).
    7. HEAD: Head of the current word, which is either a value of ID or zero (0).
    8. DEPREL: Universal dependency relation to the HEAD (root iff HEAD = 0).
    9. DEPS: Enhanced dependency graph in the form of a list of head-deprel pairs.
    10. MISC: Any other annotation.
```

- Among the columns, `4`, `8`, and `10` are crucial, as we will tag the ASC in the 10th column for every `VERB` that appears in the `4th` column. In most cases, this overlaps with the `root` found in the `8th` column. 

- In exceptional cases, annotators may encounter situations where (1) a different element (e.g., AUX) should be considered the basic unit of analysis instead of the VERB, (2) the verb itself may not be suitable as the fundamental unit, or (3) there is no appropriate unit to tag. Annotators should remain vigilant and consider the following factors when faced with these scenarios.

  - (1) Consider an auxiliary (AUX) verb as the basic unit of analysis, particularly when it functions as a copular verb.  
  
    <img width="740" alt="image" src="https://user-images.githubusercontent.com/84297888/235016296-5ecde96b-b565-40fc-bf01-97cbfd8eb082.png">
  - (2) In certain cases, some verbs function as modifiers rather than serving as the basic unit for ASC tagging. By examining the 8th column, annotators may identify modifier-related tags, such as 'amod' (adjectival modifier) or 'acl' (clausal modifier of noun). When encountering verbs with these roles, they should not be treated as the basic unit for ASC annotation.
  
    <img width="740" alt="image" src="https://user-images.githubusercontent.com/84297888/235016264-3a7c14f6-fb8c-45ab-9833-fa419e0191e0.png">

  - (3) Occasionally, a sentence may have a root but no verb, particularly when the data originates from spoken discourse. In such examples, we will not assign any ASC tag to the sentence.

    <img width="740" alt="image" src="https://user-images.githubusercontent.com/84297888/235021327-8e6e8fa2-1d75-42a6-81c6-24799e910a91.png">

## 3. Simple and concise guidelines

For an efficient annotation process, our preliminary guidelines (for annotators) focus on simplicity, minimality, and concision, as proposed by Gerdes & Kahane (2016). We offer a tag set consisting of nine fundamental ASC tags, accompanied by a decision tree to enable efficient, succinct, and swift searching while avoiding redundancies.

### ASG tag set

| **ASC tag**    | **Syntactic frame (example)**                      | **Semantic frame (example)**                                                |
|----------------|----------------------------------------------------|-----------------------------------------------------------------------------|
| **`ATTR`**       | Subj-V<sub>copular</sub>-NP                        | X<sub>theme</sub> is Y<sub>attribute</sub>                                  |
| **`INTRAN_S`**   | Subj-V                                             | X<sub>agent</sub> acts                                                      |
| **`INTRAN_MOT`** | Subj-V-Adverbial Particle/PP                       | X<sub>theme</sub> moves Y<sub>path</sub>                                    |
| **`INTRAN_RES`** | Subj-V-NP/AdjP                                     | X<sub>patient</sub> becomes Y<sub>result</sub>                              |
| **`TRAN_S`**     | Subj-V-Obj                                         | X<sub>agent</sub> acts on Y<sub>patient</sub>                               |
| **`DITRAN`**     | Subj-V-Obj<sub>indirect</sub>-Obj<sub>direct</sub> | X<sub>agent</sub> causes Y<sub>recipient</sub> to receive Z<sub>theme</sub> |
| **`CAUS_MOT`**   | Subj-V-Obj-PP                                      | X<sub>agent</sub> causes Y<sub>theme</sub> to move Z<sub>path/goal</sub>    |
| **`TRAN_RES`**   | Subj-V-Obj-NP                                      | X<sub>agent</sub> causes Y<sub>theme</sub> to become Z<sub>state</sub>      |
| **`PASSIVE`**    | Subj-auxV<sub>past participle</sub>(-*by*-PP)      | X<sub>theme</sub> undergo V (*by* Y<sub>agent</sug>)                        |

### ASC decision tree

<img width="1467" alt="image" src="https://user-images.githubusercontent.com/84297888/235018103-aa2be4da-146a-4693-add0-38fb8f887df8.png">

