# Datasets NDP-Collapsed Arch
This repository gathers the datasets access of the Digital Twin for the _Notre-Dame de Paris Cathedral Collapsed Arch Reconstruction_ for the purpose of Open Research Data (ORD) publishing. The corresponding three datasets are :

1. [Reconstruction dataset](#reconstruction-dataset)
2. [Hybrid Hypothesis 3d viewer](#hybrid-hypothesis-3d-viewer)
3. [Archeological remains viewer](#archeological-remains-viewer)

![Notre Dame de Paris point cloud and hybrid hypothesis](https://user-images.githubusercontent.com/104318232/197739328-ec665a8a-76dc-4fa9-995b-c48642071e45.png)
*Screenshot of the last hybrid hypothesis for Notre-Dame de Paris Cathedral Collapsed Arch Reconstruction ((c)V. Abergel, A.Gros)*

## Liminary
The Digital Twin application is framed by the [Scientific Site for Notre Dame de Paris Cathedral](https://www.notre-dame.science/), more specifically the "Stone" and "Digital Ecosystem" workgroups. Its engineering is a part of the [REPERAGE Project](http://www.sciences-patrimoine.org/projet/reperage/), where physical and digital methods for hypothesis building and reconstruction have met in a coherent assembly.

## Datasets
Please, note that due to the embargo on data during the Notre-Dame de Paris reconstruction period, access to the viewers is by reasoned request in accordance with the current data policy.

### Reconstruction Dataset
The reconstruction dataset is shared as a table `reconstruction-dataset-1f.xlsx` and graph-structured RDF data `reconstruction-dataset-1f.ttl` using CIDOC-CRM (ISOxxx) as an ontological basis.

The collected data relates to the two study assets and the two study processes. They stem from the physical elements and their linked digital elements (measures, models, etc.). Until the full disclosure of the lapidary reports and Notre Dame de Paris cathedral datas, the provided information are limited to the ones essential for reproducibility of the Digital Twin Experiment and REPERAGE project. The study assets are the nave collapsed transverse arch, and the corresponding voussoir of which it is composed. The study processes are the physical anastylosis observations and solutions, and the milestone reconstruction hypothesis depending on the chosen methodology.


#### Table `reconstruction-dataset-1f.xslx`
The table is divided in 4 sheets,
+ **Voussoirs :** datas for the voussoirs collected and computed from the archeological observation, physical anastylosis, reverse-engineering and results from the REPERAGE spation-temporal tracking ;
+ **Slot_Locations** : datas and informations on the collapsed arch as _slot locations_ collected and computed from the physical anastylosis and reverse enginneering activities ;
+ **Input_physical_anastylosis** : physical anastylosis hints for the reconstruction problem. As the hypothesis from physical anastylosis underwent heavy changes, the sets are dated and only milestones sets are considered ;
+ **Hypothesis_milestones** : dated milestones hypothesis, as pairing of _slot location_ and voussoir.


#### Graph `reconstruction-dataset-1f.ttl`
The graph-structured RDF dataset is modeled using pattern-based modeling. Thus, it can be described through the involved ontologies, the involved thesauruses, and the patterns for the described assets and processes. 

The CIDOC-CRM (ISOxxx) is employed as an ontological basis in its Erlangen version for the rdf-graph, it relies on the following ontologies :

| prefix | full name | namespace | description |
|---|---|---|---|
| ecrm | Erlangen CRM 211015 | http://erlangen-crm.org/211015/ | Erlangen CRM is an OWL implementation of the CIDOC CRM v7.1.1 |
| crmsci | CIDOC CRM sci | http://www.cidoc-crm.org/cidoc-crm/CRMsci/ | The Scientific Observation Model (CRMsci) is a formal ontology intended to be used as a global schema for integrating metadata about scientific observation, measurements and processed data in descriptive and empirical sciences |
| uo | Units of Measure Ontology | http://www.ontology-of-units-of-measure.org/resource/om-2/ | The Ontology of units of Measure (OM) 2.0 models concepts and relations important to scientific research. It has a strong focus on units, quantities, measurements, and dimensions. |

And the following thesauruses :

| prefix | full name | uri | description |
|---|---|---|---|
| aat | Art & Architecture Thesaurus | https://www.getty.edu/research/tools/vocabularies/aat/ | The Getty Art & Architecture Thesaurus© (AAT) is a structured vocabulary for describing and indexing the visual arts and architecture. |
| th | Thésaurus nDame | https://frollo.notre-dame.science/opentheso/?idt=th13 | The nDame thesaurus hosts the vocabularies for the Notre Dame de Paris scientific workgroups |

<!-- The patterns employed to describe the are : [pattern list]. The exhaustive description is published online at : http://reperage.map.cnrs.fr/patterns -->


### Hybrid Hypothesis 3d viewer
The hybrid hypothesis is the resulting solution from the Digital Twin experiment issued from the assembly of the processes (i.e. physical anastylosis, reverse engineering, REPERAGE photogrammetric-based spatio-temporal tracking, operational research).

The last hypothesis described in the table and graph is visualisable in the [3d viewer based](https://www.notre-dame.science/plateforme-de-centralisation-des-donnees/) on [Potree library](https://github.com/potree/potree), directly on the pre-disaster TLS point cloud. Steps for the visualisation are : a) in _Contenus de la scène_, check _Restitutions_ and uncheck _Charpente_ ; b) Pick (double-click) a reference slot from the list _Références F29F30_ or a claveau from the list _Claveaux Numérisés_ ; c) Orbit and pan the camera around the reconstruction hypothesis with left and right click ; d) Advanced visualization are available on the left-pane menu.

### Archeological remains viewer
In this study, the archeological remains seen in a reconstruction perspective as the voussoirs composing the collapsed transverse arch. The 3d viewer is based on [3D-HOP app](https://github.com/cnr-isti-vclab/3DHOP). 


## Acknowledgements
This work was supported by the project Repérage and funded by the Fondation des Sciences du Patrimoine, France. The authors, Antoine Gros, Anaïs Guillem, Livio de Luca, Élise Baillieul, Benoit Duvocelle, Lise Leroux, Olivier Malavergne, Thierry Zimmer wish to acknowledge the help and collaborative support from: the chief architects of historical monuments in charge, Philippe Villeneuve, Pascal Prunet and Rémi Fromont, the Établissement public chargé de la conservation et de la restauration de la cathédrale Notre-Dame de Paris, and the heritage conservators. The authors thank the numerous scientific partners and collaborators, with special recognition for the Stone and Digital Data workgroups; particularly, Véronique Vergès-Belmin from the Laboratoire de Recherche des Monuments Historiques, Dorothée Chaoui-Derieux from the Service Régional d’Archéologie of the Direction Régionale des Affaires Culturelles d’Île de France, Cédric Moulis from the HisCant-MA laboratory, Violette Abergel from the MAP-ARIA, and Marco Callieri at VCL of CNR-ISTI.
