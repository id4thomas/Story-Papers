# Story-Papers
Collection of Papers related to Computational Storytelling
WIP

## Conferences to Follow
* (AIIDE) The Artificial Intelligence for Interactive Digital Entertainment Conference
    * https://sites.google.com/view/aiide2021/
* (ICIDS) International Conference on Interactiate Digital Storytelling
    * https://link.springer.com/conference/icids
* (NUSE-ACL Workshop) Workshop on Narrative Understanding, Storylines, and Events
    * https://sites.google.com/view/nuse
* (IEEE COG) IEEE Conference on Games
    * https://ieee-cog.org/2021/index.html

## Table of Contents
- [Story Generation](#story-generation)
    - [Symbolic Story Generation](#symbolic-story-generation)
    - [Neural Story Generation](#nerual-story-generation)
        - [Storyline Generation](#storyline-(plot)-generation)
        - [Realization](#realization)
        - [Evaluation](#evaluation)
- [Story Analysis](#story-analysis)
    - [Plot Understanding](#plot-understanding)
    - [Character Understanding](#character-understanding)
    - [Narrative Techniques](#narrative-techniques)

## Story Generation
### Symbolic Story Generation
Planning Algorithms
(Separate File)
[Symbolic Story Generation](story_generation/symbolic_story_gen/README.md)
### Neural Story Generation
#### Storyline (Plot) Generation
##### With Explicit Outline
Explicit outlines can be in the form of Structured Format (ex. SRL Tags - Predicate,Argument Form)
Sentence
Keywords (Event, Emotion, Sentiment,...)

* Fan, Angela et al. “Strategies for Structuring Story Generation.” ACL (2019).
    + Prompt -> SRL Role Plan
* Wang, L. et al. “Plan-CVAE: A Planning-Based Conditional Variational Autoencoder for Story Generation.” CNCL (2020).
    + RAKE Keywords as outline
* Goldfarb-Tarrant, Seraphina et al. “Content Planning for Neural Story Generation with Aristotelian Rescoring.” EMNLP (2020).
    + SRL tag plot -> Rescorer for better plot
* Xu, Peng et al. “MEGATRON-CNTRL: Controllable Story Generation with External Knowledge Using Large-Scale Language Models.” EMNLP (2020).
    + Keywords as outline, Knowledge Retrieval using keywords
* Brahman, Faeze and S. Chaturvedi. “Modeling Protagonist Emotions for Emotion-Aware Storytelling.” EMNLP (2020).
    + Generate text that adheres to title & emotion arc
    + Doesn't generate emotion arc
* Ammanabrolu, Prithviraj et al. “Automated Storytelling via Causal, Commonsense Plot Ordering.” ArXiv abs/2009.00829 (2020): n. pag.
    + Plot infilling between major plot points (plot points as context)
    + Forward, backward plot graph branching using COMET
* Lin, Shih-ting et al. “Conditional Generation of Temporally-ordered Event Sequences.” ArXiv abs/2012.15786 (2020): n. pag.
    + Event infilling given event sequence (Event Deletion)

##### Without Explicit Outline
* Peng, Nanyun et al. “Towards Controllable Story Generation.” (NAACL WS 2018).
    + Ending Valence Control
* Fan, Angela et al. “Hierarchical Neural Story Generation.” ACL (2018).
* Yao, Lili et al. “Plan-And-Write: Towards Better Automatic Storytelling.” AAAI (2019).
* Ippolito, Daphne et al. “Toward Better Storylines with Sentence-Level Language Models.” ACL (2020).
    + Predict sentence embedding for continuation & select from candidates
* Polceanu, Mihai et al. “Narrative Plan Generation with Self-Supervised Learning.” AAAI 2020 (2020).
    + Forward search PDDL domains to generate target plans
    + Generate novel plan by decoding noise given as latent vector using Regularzed AE

### Realization
* Peng, Nanyun et al. “Towards Controllable Story Generation.” (NAACL WS 2018).
    + Storyline Control (keyword -> story)
* Fan, Angela et al. “Strategies for Structuring Story Generation.” ACL (2019).
    + Entity modelling (Placeholder prediction)
    + Coreference-based entity reference generation: different string given context & previous prediction for same placeholder
* Tu, Lifu et al. “Generating Diverse Story Continuations with Controllable Semantics.” NGT@EMNLP-IJCNLP (2019)
    + Generate story text given controllable value
* Xu, Peng et al. “MEGATRON-CNTRL: Controllable Story Generation with External Knowledge Using Large-Scale Language Models.” EMNLP (2020).
    + Experiement controllability of story text with antonyms

### Evaluation (?)
Evaluate generated story
perplexity? diversity?

## Story Analysis
### Plot Understanding
* Unsupervised learning of narrative event chains
* Movie Script Summarization as Graph-based Scene Extraction
* CaTeRS
* Automatic Identification of Narrative Diegesis and Point of View
* StoryFramer
* Story Understanding with External Knowledge Based Attention
* Automatic Extraction of Narrative Structure from Long Form Text
* Learning to Predict Explainable Plots for Neural Story Generation
* Movie Plot Analysis via Plot Identification
* Modelling Suspense in Short Stories as Uncertainty Reduction over Neural Representation
* Automatic Extraction of Personal Events from Dialogue
* GLUCOSE
* Multi-view Story Characterization from Movie Plot Synopses and Reviews

#### Summarization
#### Extraction / Representation
#### Identification / Classification
#### Evaluation
* Story Quality as a Matter of Perception
* UNION: An Unreferenced Metric for Evaluating Open-ended Story Generation


### Character Understanding
[Character Understading](./characters.md)
* Character-based kernels for novelistic plot structure
* Character-to-Character Sentiment Analysis in Shakespeare’s Plays
* Character-to-Character Sentiment Analysis in Shakespeare’s Plays Film Characters
* A Bayesian Mixed Effects Model of Literary Character

### Narrative Techniques
Narrative Diegesis, Focalization, ...
