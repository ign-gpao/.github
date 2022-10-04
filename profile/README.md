## Projet IGN GPAO

### Introduction

Le projet GPAO est une plate-forme open-source de distribution de calculs sur plusieurs noeuds en exploitant au mieu les ressources de chaque machine. Le projet dispose d'une librairie python qui facilite la création de workflow de travail en générant des fichiers JSON directement interprétables par la GPAO. Elle dispose d'une interface web permettant de suivre et de piloter les traitements ainsi que les noeuds de calcul.
La GPAO peut-être déployée de différentes manières, soit nativement soit en utilisant la technologie docker au travers de docker-compose.

### Composition du projet

Le projet est composé de différents modules dont voici les descriptifs : 

| Module | Description |
| --- | --- |
| [Base données](https://github.com/ign-gpao/database) | Stocke les worflows au travers de postgresql |
| [API](https://github.com/ign-gpao/api) | Module écrit en NodeJS interagit avec les base de données |
| [Monitor](https://github.com/ign-gpao/monitor) | Interface web écrit en NodeJS permettant le suivi et le pilotage des traitements |
| [Client](https://github.com/ign-gpao/client) | Module python executant les différents tâche d'un projet |
| [Docker](https://github.com/ign-gpao/docker) | Module permettant le déploiement de l'ensemble des briques de la GPAO au travers de docker |
| [Builder GPAO](https://github.com/ign-gpao/builder-python) | Librairie python de création de projet de travail sous forme d'une structure JSON |

Le code ainsi qu'une documentation plus compléte de chaque module est disponible sous github dans des `repositories` différents.

### Licence

Ce projet est sous licence CECILL-B (voir [LICENSE.md](https://github.com/ign-gpao/.github/blob/main/LICENSE.md)).

[![IGN](https://github.com/ign-gpao/.github/blob/main/images/logo_ign.png)](https://www.ign.fr)


