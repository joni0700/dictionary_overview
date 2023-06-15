<a id='eukalyptus'></a>
## **[Eukalyptus](http://demo.spraakdata.gu.se/gerlof/Eukalyptus/)**

---

Eukalyptus is a Collection of Swedish sense annotated data. The collection consists of five different genres:
- Blogg (annotated blog posts)
- Europarl (annotated EU parliament proceedings)
- Nyheter (annotated news articles)
- Romaner (annotated novels)
- Wikipedia (annotated Wikipedia articles)

### **Eukalyptus Structure**

The structure of the data depends on the type. It is stored in XML format. The data is distinguished between terminal and non-terminal.

**Example of the Eukalyptus XML structure, displaying the beginning of the file *Eukalyptus_Europarl.xml* (terminal):**  
```xml
    <subcorpus name="Eupa_00-01-17">
      <s id="Eupa_00-01-17.1">
        <graph root="Eupa_00-01-17.1.0">
          <terminals>
            <t 
              id="Eupa_00-01-17.1.1001" 
              word="Återupptagande" 
              read_as="" 
              pos="NN" 
              msd="NN.NEU.SIN.IND" 
              msd2="-.-.-" 
              lemma="återupptagande" 
              saldo="" 
              sense="återupptagande..1" 
              sense_ann=";;återupptagande..1;;" 
              sense_quality="2" 
              connected="neither"/>
            <t id="Eupa_00-01-17.1.1002">
            ...
          </terminals>
```
Definition of the attributes (according to the Eukalyptus documentation):
- **id**: word identifier [obligatory]
- **word**: word form [obligatory]
- **read_as**: how the annotator interpreted the word form in the annotation (typically for typos, non-standard orthography, etc) [optional]
- **pos**: part-of-speech [obligatory]
- **msd**: part-of-speech specific morpho-syntactic features [obligatory]
- **msd2**: general morpho-syntactic features [obligatory]
- **lemma**: lemma [obligatory], unlemmatized POS-categories get value "_"
- **saldo**: Saldo (v2.0) identifier [optional]
- **sicid**: sic identifier for blog tokens [optional]
- **sense**: Saldo sense identifier [optional]
- **sense_quality**: A confidence value for 'sense' (4-0)
- **sense_ann**: sense annotations [optional]
- **connected**: whether there is non-white space material directly preceding and/or following the token [obligatory]

&nbsp;

**Example of the Eukalyptus XML structure, displaying a non-terminal section:**  
```xml
    <nonterminals>
      <nt 
        id="Eupa_00-01-17.2.7" 
        cat="ENM">
          <edge 
            label="ME" 
            idref="Eupa_00-01-17.2.1008"/>
          <secedge 
            label="ME" 
            idref="Eupa_00-01-17.2.1009"/>
            ...
      </nt>
      ...
    </nonterminals>
```
Definition of the attributes (according to the Eukalyptus documentation):
- **nt id**: nonterminal (phrase) identifier [obligatory]
- **nt cat**: phrase label [obligatory]
- **edge label**: function label [obligatory]
- **edge idref**: child identifier [obligatory]
- **secedge idref**: secondary edge child identifier [obligatory]
- **secedge label**: secondary edge function label [obligatory]
