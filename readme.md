## The ORKG-Assays Microservice - Digitalization of Bioassays in the Open Research Knowledge Graph

#### This repository hosts supplementary data to the following publication

Jennifer D'Souza, Anita Monteverdi, Muhammad Haris, Marco Anteghini, Kheir Eddine Farfar, Markus Stocker, Vitor AP Santos, and Sören Auer. [The Digitalization of Bioassays in the Open Research Knowledge Graph](https://arxiv.org/abs/2203.14574). arXiv preprint arXiv:2203.14574 (2022). The citation for our accepted paper in the DeXa 2022 proceedings is forthcoming.

### Why Digitalize Bioassays? Motivating usecases.

A biochemist wants to compare existing bioassays that have been historically performed on the SARS virus. 
Assuming the availability of bioassays represented as machine-readable logical triple statements, 
a survey over the digitalized assay KG data can, in fact, be directly computed. 
Concretely, see https://www.orkg.org/orkg/comparison/R161302/ as a survey of 
six bioassays computed over the open research knowledge graph of bioassays in the [ORKG platform frontend](https://www.orkg.org/). 
Note that such an information access mechanism not only directly addresses the information need of the biochemist but also alleviates their effort 
to otherwise have to sift through volumes of unstructured bioassay descriptions to spot the key information. 
Specifically, taking advantage of the [ORKG](https://www.orkg.org/), the biochemist could even dynamically compute other tailored surveys to meet their information need. 
E.g., they might want to gain a comprehensive view only of those bioassays for molecules tested for the SARS virus which did not elicit a significant effect against the pathology. 
From the insights in such a dynamically computed view, they can consequently avoid testing the same molecule again, 
while focusing their attention on discovering more effective molecules. 
As another example, by having an expansive view on the various bioassays already tested in the literature, 
it should be possible to easily choose whether to repeat the experiments reproducing the same conditions of another research group 
or to try a new way to test compounds efficacy changing the type of bioassay or the type of cell cultures.

Taking a broader vision, _experiment silos_ are a problem frequently raised in research 
and a comparison of experimental models among research groups is not so frequent. 
In the context of the proposed work over bioassays, the ORKG digitalization service alleviates this problem of experimental silos by connecting all bioassays in its scholarly knowledge graph. 
Such KGs makes the bioassay data precisely _findable_ in accord with the [FAIR standards](https://www.go-fair.org/fair-principles/) advocated for research information. 
Overall, this could lead to a considerable minimization of time in research --- important especially during emergencies such as the 2019 coronavirus pandemic owing to the Sars-Cov-2 virus.

### About

ORKG-Assays is a freely available AI micro-service in ORKG written in Python designed to assist scientists obtain semantified bioassays as a set of triples. 
It uses an AI-based clustering algorithm which on gold-standard evaluations over 900 bioassays with 5,514 unique property-value pairs for 103 predicates shows competitive performance.

#### Detailed Experimental Results

<img src="docs/results-1.png" width="50%" height="50%">

Figure 1: Percentage bioassay semantification results by the naive method of most frequent labels assignment


<img src="docs/results-2.png" width="50%" height="50%">

Figure 2: Bioassay semantification results by K-means clustering of bioassay vectorized representations

### Contact

For related questions, comments, feedback, and interests in collaborations, please contact me at: jennifer (dot) dsouza (at) tib (dot) eu
