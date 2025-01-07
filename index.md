# MyDocker@Paris-Saclay

MyDocker@Paris-Saclay est un service d'environnements virtuels
permettant d'accéder à de nombreux logiciels scientifiques (dont
Jupyter) à partir d'un simple navigateur web, notamment pour du calcul
interactif, du traitement de données, etc.

Ce service est ouvert aux étudiants et personnels de l'Université
Paris-Saclay. À titre expérimental, il est ouvert plus généralement
aux établissements de la fédération d'identité «Recherche et
Enseignement Supérieur» de Renater); nous contacter avant tout usage
intensif.

% Les activités ci-dessous donnent quelques exemples d'environnements
% disponibles sur myDocker. Si vous souhaitez obtenir de l'aide sur
% l'utilisation ou la création d'environnements myDocker (notamment en
% urgence pour des TPs commençant dans la zone de turbulence actuelle à
% Paris-Saclay), vous pouvez contacter Nicolas Thiéry.

:::{admonition} Remerciements
:class: hint dropdown

Ce service est copiloté par la Faculté des Sciences et Centrale
Supélec, opéré par CentraleSupélec, codévelopé par CentraleSupeléc et 
cofinancé par le CMA
[SaclAI-School](https://www.dataia.eu/saclai-school) et hébergé par le
mésocentre
[DataCenter@UPSud](https://www.informatique-scientifique.u-psud.fr/").

:::

:::{admonition} Fonctionnalités essentielles
:class: hint dropdown

% TODO Persistence des données

- Utilisation depuis un simple navigateur web.
- Authentification via la fédération d'identité «Recherche et
  Enseignement Supérieur» de Renater, ou bien par intégration comme
  outil externe dans Moodle (ou autre LMS compatible LTI).
- **Environnement au choix**, basés ou non sur Jupyter  
  Avec possibilité de définir ses propres environnements pour choisir
  finement les logiciels installés.
- Dimensionné pour plusieurs centaines (milliers?) d'utilisateurs
  simultanés pour des usages interactifs légers (quelques CPUs).  
  Pour des besoins plus lourds, notamment de GPU pour des applications
  en IA, il est possible au cas par cas d'utiliser l'[instance
  myDocker de Centrale-Supélec](https://mydocker.centralesupelec.fr/),
  dont les serveurs sont loués à la demande. Nous contacter.
- **Hébergement souverain**.

:::

:::{admonition} Historique myDocker@Paris-Saclay et JupyterHub@Paris-Saclay
:class: hint dropdown

% TODO: Réécrire comme mini historique; voir mails envoyés

Le service myDocker@Paris-Saclay est né de la convergence entre les
services 

myDocker, originellement développé par et pour Centrale Supélec, est
de nature similaire au service JupyterHub@Paris-Saclay. En 2024, les
deux équipes ont travaillé à leur
convergence. myDocker@CentraleSupelec remplace maintenant
JupyterHub@Paris-Saclay, avec une migration essentiellement
transparente pour les utilisateurs. Il apporte une plus grande
scalabilité (nombre d'utilisateurs simultanés), la possibilité pour
les enseignants de construire leur propres environnements, et une
empreinte écologique réduite.

:::

## Accès aux environnements

% TODO
% - Ajout lien ouvrir la page d'accueil
% - Reformatage avec liste de logiciels, interface, persistance

:::::{grid} 2
::::{grid-item-card}
:::{admonition} [Clone de JupyterHub@Paris-Saclay](https://mydocker.universite-paris-saclay.fr/shell/join/qWsmLepfAkaFqYIQBjKL)
:class: dropdown

Cet environnement multiusage est strictement identique à celui déployé
sur l'ancien service JupyterHub@Paris-Saclay. Il inclue notamment
Python et ses bibliothèques classiques, SageMath, C++, R, avec choix
d'interface entre JupyterLab, Jupyter, Visual Studio Code et
l'environnement de bureau graphique XFCE.

Limitation: cet environnement n'a été mis à jour que à la marge depuis
septembre 2023. Les versions des logiciels installés y sont donc un
peu vieillissante. D'autre part il peut être long à charger du fait de
sa taille.

Cet environnement multiusage a pour vocation de faciliter la
transition depuis le précédent service Jupyter@Paris-Saclay. Il offre
une copie conforme des logiciels qui y était installés Python et ses
bibliothèques classiques de calcul scientifique, SageMath, C++, R,
etc, avec choix d'interface entre JupyterLab, Jupyter, Visual Studio
Code et l'environnement de bureau graphique XFCE.

Limitation: cet environnement n'a été mis à jour que à la marge depuis
septembre 2023. Les versions des logiciels installés y sont donc un
peu vieillissante. D'autre part il peut être long à charger du fait de
sa taille. **Sauf besoin spécifique, nous recommandons l'usage d'un
des environnements plus spécialisés.**

:::
::::


::::{grid-item-card}
:::{admonition} [Python et JupyterLab](https://mydocker.universite-paris-saclay.fr/shell/join/IvvgFOBBFzGLwuGJeFSb)
:class: dropdown

Cet environnement donne accès à Python et ses bibliothèques
scientifiques de base (numpy, pandas, matplotlib), dans l'interface
JupyterLab. Il est notamment utilisé pour un cours nommé
[«Introduction à la programmation avec Python et
Jupyter»](https://introductionprogrammationpython.pages.centralesupelec.fr/).

:::

::::

::::{grid-item-card}
:::{admonition} pyTorch et JupyterLab
:class: dropdown

Cet environnement est basé sur l'image
[jupyter/pytorch-notebook](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-pytorch-notebook)
de la communauté Jupyter.

:::
::::

::::{grid-item-card}
:::{admonition} C++ et JupyterLab
:class: dropdown

- Interface: JupyterLab
- Logiciels: compilateurs et interpréteurs C++

:::

::::

## Résolution de problèmes
