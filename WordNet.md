<a id='WordNet'></a>
## **[WordNet](https://wordnet.princeton.edu/)** 

---

WordNet® is a large lexical database. Nouns, verbs, adjectives and adverbs are grouped into sets of cognitive synonyms (synsets), each 
expressing a distinct concept. Synsets are interlinked by means of conceptual-semantic and lexical relations. [read more...](https://wordnet.princeton.edu/)

The main relation among words in WordNet is synonymy, as between the words *shut* and *close* or *car* and *automobile*. Each of WordNet’s ~117 000 synsets is linked to other synsets by means of a small number of “conceptual relations.” Additionally, a synset contains a brief definition (“gloss”) and, in most cases,<sup id="wn_a1">[1](#wn_1)</sup> one or more short sentences illustrating the use of the synset members.

### **WordNet Structure**

The main database consists of eight files, namely `index.pos` and `data.pos` files for noun, verb, adjective and adverb. The index files are alphabetical orderd lists of all words in WordNet with references to the synsets in which they appear. The data files are lists of the actual synsets, containing additional information about the synsets and their relations to other synsets.  ([Documentation](https://wordnet.princeton.edu/documentation/wndb5wn))

#### **index.pos**

**Strucutre**:  
`lemma pos  synset_cnt  p_cnt  [ptr_symbol...]  sense_cnt  tagsense_cnt   synset_offset  [synset_offset...]`

**Example**:  
`ebony a 1 1 & 1 0 00389231`  


#### **data.pos**

**Structure**:  
`synset_offset  lex_filenum  ss_type  w_cnt  word  lex_id  [word  lex_id...]  p_cnt  [ptr...]  [frames...]  |   gloss `

**Example**:  
`00389231 00 s 02 ebon 0 ebony 0 001 & 00386392 a 0000 | of a very dark black`

&nbsp;

Links

<a id="wn_1">1</a> According to own experiments only roughly 30% (32.923/117.659) of the synsets have examples. [↩](#wn_a1)
