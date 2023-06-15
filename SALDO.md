<a id='SALDO'></a>
## **[SALDO](https://spraakbanken.gu.se/eng/resource/saldo)**

---

SALDO is a lexical database for Swedish, developed at the Department of Swedish, University of Gothenburg. SALDO is a semantic network, where the words are connected to each other through semantic relations. [read more...](https://spraakbanken.gu.se/eng/resource/saldo)

>Every entry in SALDO—representing a word sense—is supplied with one or more
>semantic descriptors, which are themselves also entries in the dictionary. All entries in
>SALDO (...) are actually occurring
>words or conventionalized or lexicalized multi-word units of the language. [2013](#saldo_paper)


### **SALDO Structure**

SALDO is a semantic network, where the words are connected to each other through semantic relations. The database contains information about word meaning, word class, inflection, morphology, orthography, pronunciation, and frequency.

**Example of a SALDO entries for the word *bok* (book/birch):**  
```
bok..1	läsa..1	PRIM..1	bok..nn.1	bok	nn	nn_3u_bok
bok..2	träd..1	löv..1	bok..nn.2	bok	nn	nn_2u_sten
```

The primary descriptor [*läsa* or *träd*] - meaning *read* or *tree*, fulfills two requirements: 
- It is a semantic neighbor<sup id="saldo_a1">[1](#saldo_1)</sup> of the corresponding entry (*bok*) and
- It is a more general term than the corresponding entry.

The secondary descriptor [*PRIM* or *löv*] helps to further specify the sense of the keyword.

PRIM is an artificial entry, used as a placeholder for senses where so far no descriptor has been found.

The other arguments are used to help with the search and browsing interface. For example different spelling variants.

## **[SALDO: examples](https://spraakbanken.gu.se/en/resources/saldoe)**

---

SALDO: examples is a lexicon that links one or more sample sentences to an entry in SALDO.

### **SALDO: exmaples Structure**

Sense id is the same as in SALDO. The example is given in the attribute *val*. The word to be exemplified is given in [square brackets].

**Example of a SALDO: examples entry for the word *agera* (act):**  
```xml
    <LexicalEntry>
      <Lemma/>
      <Sense id="agera..1">
        <SenseExample>
          <feat att="text" val="Ofta måste det ha hänt något allvarligt för att polisen ska [agera]."/>
        </SenseExample>
      </Sense>
    </LexicalEntry>
```

&nbsp;

Links

<a id="saldo_1">1</a> Words that are *semantic neighbors* are words that have a direct semantic relation to each other (synonym, hyponym, meronym, ..) [↩](#saldo_a1)

<a id="saldo_paper">2013</a>
Lars Borin et al. (2013) SALDO: a touch of yin to WordNet's yang. Language resources and evaluation, 47 (4), 1191-121



