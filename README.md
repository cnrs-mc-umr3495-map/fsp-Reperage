# Datasets NDP-Collapsed Arch

This repository gathers the datasets access of the Digital Twin for the Notre-Dame de Paris cathedral collapsed arch reconstruction for the purpose of Open Science dataset publishing. The corresponding three datasets are :

1. [Reconstruction dataset](### Reconstruction Dataset)
2. [Hybrid Hypothesis 3d viewer](#anchors-in-markdown)
3. [Archeological remains viewer](#anchors-in-markdown)

## Liminary
Wip...

## Datasets
### Reconstruction Dataset
The reconstruction dataset is shared as a table `reconstruction-dataset-1f.xlsx` and graph-structured RDF data `reconstruction-dataset-1f.ttl` using CIDOC-CRM (ISOxxx) as an ontological basis.

The collected data relates to the two study assets and the two study processes. They stem from the physical elements and their linked digital elements (measures, models, etc.). Until the full disclosure of the lapidary reports and Notre Dame de Paris cathedral datas, the provided information are limited to the one essential for reproducibility of the Digital Twin Experiment and REPERAGE project.

The study assets are the nave collapsed transverse arch, and the corresponding voussoir of which it is composed.

The study processes are the physical anastylosis observations and solutions, and the milestone reconstruction hypothesis depending on the chosen methodology.


#### Table `reconstruction-dataset-1f.xslx`
The table is divided in 4 sheets,
+ **Voussoirs :** datas for the voussoirs collected and computed from the archeological observation, physical anastylosis, reverse-engineering and results from the REPERAGE spation-temporal tracking ;
+ **Slot_Locations** : datas and informations on the collapsed arch as _slot locations_ collected and computed from the physical anastylosis and reverse enginneering activities ;
+ **Input_physical_anastylosis** : physical anastylosis hints for the reconstruction problem. As the hypothesis from physical anastylosis underwent heavy changes, the sets are dated and only milestones sets are considered ;
+ **Hypothesis_milestones** : dated milestones hypothesis, as pairing of _slot location_ and voussoir.


#### Graph `reconstruction-dataset-1f.ttl`
The graph-structured RDF dataset is modeled using pattern-based modeling. Thus, it can be described through the involved ontologies, the involved thesauruses, and the patterns for the described assets and processes. 

The CIDOC-CRM (ISOxxx) is employed as an ontological basis in its Erlangen version for the rdf-graph, it relies on the following ontologies :

| prefix | full name | uri | description |
|---|---|---|---|
| ecrm | Erlangen CRM 211015 | http://erlangen-crm.org/211015/ | Erlangen CRM is an OWL implementation of the CIDOC CRM v7.1.1 |
| crmsci | CIDOC CRM sci |  |  |
| uo | Units of Measure Ontology |  |  |

And the following thesauruses :

| prefix | full name | uri | description |
|---|---|---|---|
| aat | Art & Architecture Thesaurus | https://www.getty.edu/research/tools/vocabularies/aat/ | The Getty Art & Architecture Thesaurus© (AAT) is a structured vocabulary for describing and indexing the visual arts and architecture. |
| th | notredamethesaurus |  |  |
| xxx | xxx |  |  |

The patterns employed to describe the are : [pattern list]. The exhaustive description is published online at : http://reperage.map.cnrs.fr/patterns


### Hybrid Hypothesis 3d viewer
The hybrid hypothesis is the resulting solution from the Digital Twin experiment issued from the assembly of the processes (i.e. physical anastylosis, reverse engineering, REPERAGE photogrammetric-based spatio-temporal tracking, operational research).

In addition to its _dict-like_ publication presented in the reconstruction dataset as the last milestone hypothesis, this hypothesis is visualisable in the [3d viewer based](https://www.notre-dame.science/plateforme-de-centralisation-des-donnees/) on [Potree library](https://github.com/potree/potree), directly on the pre-disaster TLS point cloud : https://nd.aioli.map.cnrs.fr:42000/index.php#

#### Steps for visualization
Wip...

### Archeological remains viewer
In this study, the archeological remains seen in a reconstruction perspective as the voussoirs composing the collapsed transverse arch. The 3d viewer is based on [3D-HOP app](https://github.com/cnr-isti-vclab/3DHOP) : http://



## Acknowledgements
This work was supported by the project Repérage and funded by the Fondation des Sciences du Patrimoine, France. The authors, Antoine Gros, Anaïs Guillem, Livio de Luca, Élise Baillieul, Benoit Duvocelle, Lise Leroux, Olivier Malavergne, Thierry Zimmer wish to acknowledge the help and collaborative support from: the chief architects of historical monuments in charge, Philippe Villeneuve, Pascal Prunet and Rémi Fromont, the Établissement public chargé de la conservation et de la restauration de la cathédrale Notre-Dame de Paris, and the heritage conservators. The authors thank the numerous scientific partners and collaborators, with special recognition for the Stone and Digital Data workgroups; particularly, Véronique Vergès-Belmin from the Laboratoire de Recherche des Monuments Historiques, Dorothée Chaoui-Derieux from the Service Régional d’Archéologie of the Direction Régionale des Affaires Culturelles d’Île de France, Cédric Moulis from the HisCant-MA laboratory, Violette Abergel from the MAP-ARIA, and Marco Callieri at VCL of CNR-ISTI.
