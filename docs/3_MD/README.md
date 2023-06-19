---
sort: 3
---

# Table of Contents
1. [Ambiguous constructions](#ambiguous-constructions)
	* [CAUS_MOT vs. TRAN_RES](#caus_mot-vs-tran_res)
	* [DITRAN vs. CAUS_MOT](#ditran-vs-caus_mot)
	* [PASSIVE vs. ATTR](#passive-vs-attr)

2. [Ambiguous arguments-construction combinations](#ambiguous-arguments-construction-combinations)	
	* [INTRAN_MOT: verb "enter" + location](#intran_mot-verb-enter--location)
	* [TRAN_S: reflexive object](#tran_s-reflexive-object) 
	* [TRAN_RES: figurative preposition/particle](#tran_res-figurative-prepositionparticle)
	* [TRAN_RES: verb "keep/prevent"](#tran_res-verb-keepprevent)

3. [Difficult grammatical structures](#difficult-grammatical-structures)
	* [Inverted/Fronted word order](#inverted-fronted-word-order)
	* [Dealing with L2 usage](#dealing-with-l2-usage)
	* [Multi-word lexical units](#multi-word-lexical-units)
	* [Light verb constructions](#light-verb-constructions)

4. [Skipped structures](#skipped-structures)
	* [Modal and semi-modals](#modal-and-semi-modals)
	* [Some discourse markers](#)

# Detailed discussion

## Ambiguous constructions


### CAUS_MOT vs. TRAN_RES

CAUS_MOT typically contains a non-stative verb and **a directional phrase**.
The following are some example sentences (Goldberg, 1995, p.152)
```
- They laughed the poor guy out of the room.
- Frank sneezed the tissue off the table.
- Mary urged Bill into the house.
- Sue let the water out of the bathtub.
- Sam helped him into the car.
- They sprayed the paint onto the wall.
```

CAUS_MOT is associated with a category of related verb senses (Goldberg, 1995, pp. 161-162)
1. X CAUSES Y to MOVE Z
```
- Frank pushed it into the box.
- Frank kicked the dog into the bathroom.
- Frank sneezed the tissue off the nightstand.
- Sam shoved it into the carton.
- Pat crammed the pennies into the jar.
```

2. Sometimes the construction can be related to force-dynamic verbs (Talmy 1985b) that encode a communicative verb.
(In this case, the motion ins not strictly entailed.)
```
- Sam ordered him out of the house.
- Sam asked him into the room.
- Sam invited him out to her cabin.
- Sam beckoned him into the room.
- Sam urged him into the room.
- Sam sent him to the market.
```

3. X ENABLES Y to MOVE Z: This class includes force-dynamic verbs that encode the removal of a barrier.
```
- Sam allowed Bob out of the room.
- Sam let Bill into the room.
- Sam freed the bird out of the cage.
```

4. X PREVENTS Y from MOVING Z: This class imposes a barrier, causing the patient to stay in a location.
```
- Harry locked Joe into the bathroom.
- He kept her at arm's length.
- Sam barricaded him out of the room.
```

5. X HELPS Y to MOVE Z: This case involves ongoing assistance to move in a certain direction.
```
- Sam helped him into a car.
- Sam assisted her out of the room.
- Sam guided him through the terrain.
- Sam showed him into the livingroom.
- Sam walked him to the car.
```

In TRAN_RES constructions, a non-stative verb is typically accompanied by a patient argument that experiences a change of state due to the verb's action (Boas, 2002). 
- If the change in state pertains solely to **a change of location**, CAUS_MOT will be assigned. 
- However, if a prepositional phrase is present and describes **a change of state**, then TRAN_RES will be assigned.
- We will categorize lexically causative verbs, such as *make*, *have*, and *let*, as TRAN_RES.

The following are some example sentences (Boas, 2002; Goldberg, 1995).

```
- Claire painted the house red.
- Pat broke the vase (in)to pieces. (check)
- Chris drank himself silly.
- Carol danced Jim tired.
- Rachel swept the floor clean.
- He wiped the table clean.
- He talked himself blue in the face.
- She coughed herself sick.
- She slept herself sober.
- He made the metal safe.
- He made her a queen.
```

### DITRAN vs. CAUS_MOT 

One of the questions is how to treat cases involving dative alternation (i.e., the alternation between a prepositional indirect-object construction (e.g., *I gave the book to him*) and a double-object construction (e.g., *I gave him the book*)). 

The object of the *to* preposition can cover a wide range of argument types (semantically), including recipients (possessional goals, e.g., *She handed a letter **to me***) and spatial goals (e.g., *He kicked a ball **to the target***) (Haspelmath, 2003; Hovav & Levin, 2008; Newman, 1996). Sometimes, it can even include arguments that are not clearly goals, as seen in examples like *conform to*, *submit to* (more likely to be phrasal verbss). 
In this annotation project, we will include every **prepositional indirect-object construction** when the argument following the *to* preposition is either a recipient (possessional goal) or a spacial goal, and tag it as a **CAUS_MOT**.


### PASSIVE vs. ATTR

Merely examining the surface structure, it is sometimes challenging to differentiate between PASSIVE and ATTR constructions, especially when the verb lies on a continuum between the past participle form of a verb and an adjective.

The following are two examples, which appear very similar in terms of their surface structures.

<img width="585" alt="image" src="https://github.com/hksung/ASC-annotation-guidelines/assets/84297888/bfc85d7d-e989-4a44-abe6-6767d290f76a">

We are going to rely on POS tags. The simple rule is as follows: (1) if the element following the 'be' verb is marked as VERB (in the 4th column), tag it as PASSIVE on the 'verb'; (2) if this element is marked as ADJ (or any other POS tag that's not VERB), tag it as ATTR on the 'be' verb.

## Ambiguous arguments-construction combinations

### INTRAN_MOT: verb "enter" + location
This should get INTRAN_MOT tag, because we have a theme as a subject and a destination after the verb.

```
- enter the classroom
- reach the summit
- approach the city
- visit the museum
```

### TRAN_S: reflexive object

### TRAN_RES: figurative preposition/particle

### TRAN_RES: verb "keep/prevent"


## Difficult grammatical structures


### Inverted/Fronted word order

#### Fronted theme (theme+agent+verb+recipient)

e.g., (# text = I am writing to reply **your letter you wrote me** on 10 June.) 

At this stage, we do not differentiate the ASCs that have different word order (We plan to address this after the first round of ASC annotation work is completed). Because we can identify all necessary arguments for the ditransitive construction in this example, we are going to assign the DITRAN tag for this case.

### Dealing with L2 usage
Often, errors can be found in sentences or utterances, especially in an L2 dataset. Building on the earlier two projects related to L2 English UD treebank (Berzak et al. 2016 & Kyle et al., 2022), we will annotate the ASCs based on their realized form, not their intended meaning, to eliminate any potential interpretation from the annotators and keep consistency (Wittenberg et al., 2014). 

#### INTRAN_S vs. TRAN_S

- Example: *explain about* 
  
  <img width="730" alt="image" src="https://user-images.githubusercontent.com/84297888/235237515-11124a79-5f70-4fab-904c-1e2f8426519d.png">
  
  The issue lies with the use of the preposition "about" in this context. In English, when you explain something, you typically use "explain" without a preposition, as it is a transitive verb that takes a direct object. However, in terms of ASC tagging, we rather rely on the realized form and tag it as "INTRAN_S" for the purpose of annotating the L2 dataset based on its actual structure, rather than attempting to infer the intended meaning.


### Multi-word lexical units

We will assign a single ASG tag to a multi-word lexical unit (i.e., a sequence of words which functions as a single grammatical unit), as the meaning of the multi-word unit derives from the combination of the words, not from the individual meanings of the parts (Biber et al., 1999, p.58).

```
Categorized four major kinds of multi-word combination (Biber et al., 1999, p.403),
which comprise relatively idiomatic units and function like single verbs:

- verb + adverbial particle: phrasal verbs (e.g., pick up)
- verb + preposition: prepositional verbs (e.g., look at)
- verb + particle + preposition: phrasal-prepositional verbs (e.g., get away with)
- other multi-word verb constructions
  - verb + noun phrase (+ preposition) (e.g., take a look (at))
  - verb + prepositional phrase, (e.g., take into account)
  - verb + verb (e.g., make do)
```
- Example: *call for*

  <img width="740" alt="image" src="https://user-images.githubusercontent.com/84297888/235262826-79a83080-3995-4fcd-80d9-0252da971a00.png">


### Light verb constructions

Light verb constructions are intricate predicates where the verb loses its semantic meaning. In a sentence like "Henry took a walk," the subject's character isn't acquiring a tangible object, as in "Henry took a spoon." Instead, "take a walk" represents the same event as the verb "walk." Thus, we don't assign "TRAN_S" but rather use "INTRAN_S" in this case (Wittenberg et al., 2014).

- Example: *hitch a ride back* 

  <img width="740" alt="image" src="https://user-images.githubusercontent.com/84297888/235262173-3651bf91-74fa-459a-9a81-d89f32668645.png">


## Skipped structures

### Modal and semi-modals

We will not tag modal auxiliary verbs because they serve a grammatical function rather than providing semantic content (Similarly, the project does not encompass the tagging of tense-related aspects). The following provides more information on English modals and semi-modals based on Biber et al. (1999, pp.483-484). 

- Nine central modal auxiliary verbs for modality: *can, could, may, might, shall, should, will, would, must*
- Marginal auxiliary verbs (behave like modals in taking auxiliary negation and *yes-no* question inversion): *need (to), ought to, dare (to), used to*
- Semi-modals (i.e., a number of fixed idiomatic phrases with functions similar to those of modals): *(had) better, have to, (have) got to, be supposed to, be going to*

We will include some of the ver phrases with the force of a hedge (in certain contexts) (pp.944-945): *happen to, tend to be, appear to, (there) is said to be*.
- Example: *happen to*

  <img width="736" alt="image" src="https://user-images.githubusercontent.com/84297888/236060250-958f28c5-936d-412d-9f07-3e957f8c403d.png">

  ### Some discourse markers
