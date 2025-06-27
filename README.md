# finite-state-transducers

This program has two transductors that work with Bribri verbs in eight different verbal forms. They serve the following purpose: 

1.  The first transductor outputs morpheme boundaries of the input word (Example of morpheme boundary in English : cooked > cook-ed, The same for Bribri is aleH > al-eH ).
   
2.  The second transductor outputs morpheme-by-morpheme glossing in English (Example of glossing : aloqFk > cook-INF, -INF represents that -oqFk indicates the infinitive form of the verb). The meaning is encoded following the Leipzig glossing rules described here in the website of the Max Plank Institute : [https://www.eva.mpg.de/lingua/resources/glossing-rules.php.]

### The verbs used for testing are:

1. aloqFk (to cook) : used as the main verb of testing
2. tsakok (to pop (a bubble))
3. biok (to dig)


### The eight different verbal forms with morpheme boundaries, morpheme-by-morpheme gloss in English) and English Translation: 

#### Active voice: 

1. Imperfective (-IPFV): al-eH ; cook-IPFV, I cook, I used to do cook
2. Perf. Improspective (-THEME.PFV.IMPROSP): al-i' ; cook-THEME.PFV.IMPROSP ; I cooked [before today]
3. Infinitive (-INF): al-oqFk ; to cook
4. Imperative (-IMP) : al-oqF : (you) cook!
5. Desiderative (-DESIDERATIVE) : al-a'kux ; I want to cook

#### Mid voice: 

1. Imperfective (-THEME.MID.IPFV) : al-iHr ; It is being cooked, people cook it
2. Perf. Improspective (-THEME.MID-PFV.IMPROSP) : al-iHn-ex ; It became cooked, It was cooked [before today]
3. Infinitive (-THEME.MID-INF) : al-iHn-uxk ; to be cooked


### Files in this repository

The finite-state-transducer-code.ipynb file has the code for the two transducers. Morph.gv is the pdf output of the first transducer and translate.gv is the pdf output of the second one. 


### Relevant links

1. The transductor uses the `openfst` and `graphviz` packages:
http://www.openfst.org/twiki/bin/view/FST/PythonExtension
https://graphviz.readthedocs.io/en/stable/manual.html
2. Learn more about Bribri, a language of Costa Rica: https://en.wikipedia.org/wiki/Bribri_language
