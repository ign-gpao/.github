# Projet IGN GPAO

## Introduction

Le projet GPAO est une plate-forme open-source de distribution de calculs sur plusieurs nœuds en exploitant au mieux les ressources des machines allouées.

Les traitements sont effectués par des nœuds de calculs gérés par les clients GPAO installés sur une ou plusieurs machines. La GPAO dispose d'une interface Web permettant de suivre et de piloter les traitements (appelés jobs et regroupés en projets) ainsi que les nœuds de calcul des machines (sessions et hosts). Le projet GPAO dispose également d'une librairie python qui facilite la création de workflow en générant des fichiers JSON directement interprétables comme jobs et projets.  

La GPAO peut être déployée de différentes manières, soit nativement soit en utilisant la technologie Docker au travers de Docker Compose. 

<div style="width:100px">
![schéma GPAO](https://github.com/ign-gpao/.github/blob/main/images/gpao_doc.png)
</div>

## Composition du projet

Le projet est composé de différents modules dont voici les descriptifs et les versions de la dernière release stable 3.3.0 :  

| Module | Description | Version |
| --- | --- | --- |
| [Base données](https://github.com/ign-gpao/database) | Base de données PostgreSQL qui stocke les workflows | 0.9.0 |
| [API](https://github.com/ign-gpao/api) | Module développé en Node.js qui connecte les bases de données et les autres briques de la GPAO | 1.14.0 |
| [Monitor](https://github.com/ign-gpao/monitor) | Interface web développée en Node.js permettant le suivi et le pilotage des traitements | 1.30.0 |
| [Client](https://github.com/ign-gpao/client) | Module python exécutant les différents jobs d'un projet | 0.13.2 |
| [Docker](https://github.com/ign-gpao/docker) | Module permettant le déploiement de l'ensemble des briques de la GPAO au travers de Docker | 0.6.0 |
| [Builder GPAO](https://github.com/ign-gpao/builder-python) | Librairie python de création de projet de travail sous forme d'une structure JSON | 0.9.0 |

Le code ainsi qu'une documentation plus complète de chaque module est disponible sous GitHub dans des `repositories` différents.

## Licence

Ce projet est sous licence CECILL-B (voir [LICENSE.md](https://github.com/ign-gpao/.github/blob/main/LICENSE.md)).

[![IGN](https://github.com/ign-gpao/.github/blob/main/images/logo_ign.png)](https://www.ign.fr)


