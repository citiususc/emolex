# EmoLex Ontology

**EmoLex** is an OWL ontology designed to represent **emotional and related psycholinguistic annotations of words** in a structured and interoperable way. It provides a semantic model to publish and integrate multiple emotion lexica as RDF KG, serving as the conceptual backbone for the [Emotional Words Knowledge Graph (EmoW-KG)](https://kg.app.citius.gal/data/emofinder/sparql/) and the [semantic emoFinder platform](https://kg.app.citius.gal/emofinder/).

EmoLex follows a lexicographic modelling approach based on **OntoLex-lemon**: words are represented as `ontolex:LexicalEntry`, which can evoke `skos:Concept`s. Emotional (and related) scores are represented as annotations linked to lexical entries. In particular, `emolex:Annotation` captures the association between a word and a given variable (e.g., valence, arousal, dominance, basic emotions, behavioral measures), and is linked to the target entry via `emolex:affects`. Numeric values such as mean and standard deviation can be expressed using RiverBench metadata properties (e.g., `rb:mean`, `rb:standardDeviation`).  


<p align="center">
  <img title="logo" alt="YATTER" src="https://raw.githubusercontent.com/citiususc/emolex/main/diagrams/emolex.jpg"  width="300" height="300"/>
</p>

## Main namespace

- **Ontology IRI:** `https://w3id.org/def/emolex`
- **Namespace:** `https://w3id.org/def/emolex#`
- **Suggested prefix:** `emolex:`

## Reused vocabularies (selected)

- OntoLex-lemon (`ontolex:`), SKOS (`skos:`)
- Dublin Core Terms (`dcterms:`), BIBO (`bibo:`)
- LexInfo (`lexinfo:`), LIME (`lime:`) 