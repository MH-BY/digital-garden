---
{"dg-publish":true,"permalink":"/notes/references/jablonka-gpt-3-all-you2023/","title":"Is GPT-3 all you need for low-data discovery in chemistry?","tags":["research, paper,"]}
---



# Is GPT-3 all you need for low-data discovery in chemistry?
#### (2023) - Kevin Maik Jablonka, Philippe Schwaller, Andres Ortega-Guerrero, Berend Smit
---------------------------------
- **Link**: 
- **DOI**: 10.26434/chemrxiv-2023-fw8n4
- **Zotero Link**: [Is GPT-3 all you need for low-data discovery in chemistry?](zotero://select/items/@jablonkaGPT3AllYou2023)
- **Tags**: #paper
- **Cite Key**: [@jablonkaGPT3AllYou2023]
- **Linked notes**: [[Notes/Paper Annotations\|Paper Annotations]]
----------------------------------
## Abstract
>Machine learning has revolutionized many fields and has recently found applications in chemistry and materials science. The small datasets commonly found in chemistry lead to various sophisticated machine-learning approaches that incorporate chemical knowledge for each application and therefore require a lot of expertise to develop. Here, we show that large language models that have been trained on vast amounts of text extracted from the internet can easily be adapted to solve various tasks in chemistry and materials science by simply prompting them with chemical questions in natural language. We compared this approach with dedicated machine-learning models for many applications spanning properties of molecules and materials to the yield of chemical reactions. Surprisingly, we find this approach performs comparable to or even outperforms the conventional techniques, particularly in the low data limit. In addition, by simply inverting the questions, we can even perform inverse design successfully. The high performance, especially for small data sets, combined with the ease of use, can have a fundamental impact on how we leverage machine learning in the chemical and material sciences. Next to a literature search, querying a foundational model might become a routine way to bootstrap a project by leveraging the collective knowledge encoded in these foundational models.

## Figures
![Pasted image 20230310173348.png](/img/user/Attachments/Pasted%20image%2020230310173348.png)
![Pasted image 20230310173459.png](/img/user/Attachments/Pasted%20image%2020230310173459.png)

![Pasted image 20230310173513.png](/img/user/Attachments/Pasted%20image%2020230310173513.png)
![Pasted image 20230310173528.png](/img/user/Attachments/Pasted%20image%2020230310173528.png)

## Notes
<h1>Annotations
 (3/10/2023, 5:32:30 PM)</h1> 

“In Extended Data Fig. 1, we have given the set of questions and answers we have used to fine-tune the GPT-3 model. These are questions and answers on high entropy alloys for which the phase has been experimentally determined. The model tuning takes a few minutes and gives us a new model, which takes as input "What is the phase of Tb0.5Y0.5" and gives as text completion "1", which corresponds to single-phase. This simple example already gives some remarkable results.” (Jablonka et al., 2023, p. 4) 

“We selected this example, as we can directly compare its performance with the current state-of-the-art machine learning models with descriptors specially developed to mimic the relevant chemistry for this application.14 In Extended Data Fig. 1, we show that with only around 50 data points, we get a similar performance as the model of Pei et al. 14, which was trained on more than 1000 data points.” (Jablonka et al., 2023, p. 4) 

“An interesting question is how to represent a molecule or material. Most of the literature uses IUPAC names. For ML applications, there has been a lot of effort to represent a chemical with unique line encodings (e.g., SMILES19 or SELFIES20,21). As the GPT-3 model has been developed using natural languages, one might expect that chemical names are preferred over line representations such as SMILES or SELFIES. Therefore, we investigated different representations for our molecular property prediction tasks (see also Supplementary Note 4). Surprisingly, our results (see Supplementary Note 6) show that irrespective of the representation used, good results are obtained.” (Jablonka et al., 2023, p. 5) 

“ablonka et al. 36 developed an active learning approach to design dispersants using a coarse-grained approach. This dispersant was a linear copolymer with four monomer types and a chain length between 16 and 48 units, giving a chemical design space of 58 million different dispersants. One important goal in this work was to find dispersants with the right binding free energy, i.e., which polymer length and which monomer sequence is optimal. As there is no way the GPT-3 knows about the properties or representations of the coarse-grained polymers, it is interesting to see if we can get any sensible result if we ask the question What is the adsorption free energy of coarse-grained dispersant AAAABBBBDDDDAAAACCCC or as inverse design, Give me a structure of a coarse-grained dispersant with a free energy of 17. Surprisingly, for the prediction of the adsorption free energy, the GPT-3 model outperforms the models developed by Jablonka et al. 36” (Jablonka et al., 2023, p. 10) 

“We now conduct some experiments to test how well the GPT-3 model can extrapolate to HOMO-LUMO gaps for which it has not received any training. To mimic this situation, we retrained our inverse design model using a dataset that only has molecules with HOMO-LUMO gaps smaller than 3.5 eV, and subsequently query the model with a question that requires the GPT-3 model to extrapolate. We do this by asking 1,000 times the question: What is a molecule with a HOMO LUMO gap of &lt;XX&gt;, where each time we slightly change the value of the HOMO LUMO gap, i.e., we sample XX from a Gaussian centered at 4 eV. Interestingly, the GPT-3 model does provide structures with a distribution of which our quantum calculations confirm that a significant fraction has a HOMO-LUMO gap &gt; 4.0 eV. Again this is a remarkable result.” (Jablonka et al., 2023, p. 11) 

“n many practical applications, one has more requirements than the correct HOMO-LUMO gap. Suppose we need a bromine-containing material with a well-defined HOMO-LUMO gap. Without additional training, we queried our model using What is a molecule with a HOMO-LUMO gap of 3.5 eV and Br as part of the molecule. Figure 4 shows the results of such questions for different functional groups.” (Jablonka et al., 2023, p. 14) 

“Concluding remarks Our results raise a very important question, how is it possible that a natural language model with no prior training in chemistry outperforms dedicated machine-learning models?” (Jablonka et al., 2023, p. 15) 

“In some regards, this is not that different from how an experienced chemist would design a material. Suppose a chemist sees a publication of a new material, and she or he notices that some properties are very similar to the materials that are studied for a completely different application. These similarities are often the source of inspiration to try variations of this novel material for this application. Extracting and remembering such correlations enables GPT-3 to perform (inverse) 1” (Jablonka et al., 2023, p. 15) 

“design. That GPT-3 can work with these correlations over such a large range of topics makes it so powerful.” (Jablonka et al., 2023, p. 16)