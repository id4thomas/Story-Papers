# Characters
Works related to Character Understanding

## Main Character,Protagonist
* (ACL 08) Unsupervised Narrative Chain - Chambers, Jurafsky (Most referenced)
  +

* (NAACL 15) Movie Script Summarization as Graph-based Scene Extraction
  + Use a MLP classifier for main character detection
  + character interaction: Conversations/Relations
  + Relations: verbs whose ARG0 and ARG1 roles are character names (Semantic Role Labeling)


* (IEEE ICCP 15) Information retrieval in folktales using natural language processing
  + Propp's model of folktale domain

* (ACL 18) Temporal Event Knowledge Acquisition via Identifying Narratives
  + Narrative paragraph must have a protagonist character
  + longest three coreferent entity chains

* (Thesis 18) Automatic Extraction of Narrative Structures from Long Form Text
  + main character feature: assume main character is referent referred to by the longest coreference chain
  + main character sum  feature: how many of the top three main characters are mentioned in each sentence

* (EMNLP 20) Modeling Protagonist Emotions for Emotion-Aware Storytelling
  + Protagonist: Most frequently occurring character in a narrative

* (20) Extraction and Analysis of Fictional Character Networks: A Survey
  * Major/Minor Characters
  * Minor -> Supporting Characters / Extras
  * All the methods appearing in the literature rely on nodal topological measures (structural features?)
  * Use Narrative Content: POS, Sentiment Analysis, Co-occurrence context
