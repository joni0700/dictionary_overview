<a id='semcor'></a>
## **[SemCor/SemCor+OMSTI)](http://lcl.uniroma1.it/wsdeval/)**

---

SemCor and SemCor+OSTI are a corpora of English sentences that have been annotated with WordNet synsets. Each dataset consists of a data file [dataset].data.xml and a gold file [dataset].gold.key.txt.

### **WSD-data Structure**

The .data.xml file contains a list of sentences. Every token in these sentences is enclosed in a `<wf>` or `<instance>`. Tokens enclosed in `<instance>` have an id which can be found in the .gold.key.txt file. The .gold.key.txt file contains a list of instance ids and gold answers. [read more...](https://sapienzanlp.github.io/xl-wsd/docs/data/)

#### **`[dataset].data.xml`**

**Example of *semcor.data.xml* entry:**  
```xml 
    <sentence id="d000.s005">
        <wf lemma="be" pos="VERB">Is</wf>
        <wf lemma="it" pos="PRON">it</wf>
        <instance id="d000.s005.t000" lemma="reach" pos="VERB">reaching</instance>
        <wf lemma="these" pos="DET">these</wf>
        <instance id="d000.s005.t001" lemma="goal" pos="NOUN">goals</instance>
        <wf lemma="?" pos=".">?</wf>
    </sentence>
```

#### **`[dataset].gold.key.txt`**

**Example of *semcor.gold.key.txt* entry:**  

`d000.s005.t000 reach%2:38:06::`
