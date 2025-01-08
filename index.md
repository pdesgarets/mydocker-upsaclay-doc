# MyDocker@Paris-Saclay

[MyDocker@Paris-Saclay](https://mydocker.universite-paris-saclay.fr/)
est un service d'environnements virtuels permettant d'accéder à de
nombreux logiciels scientifiques (dont Jupyter) à partir d'un simple
navigateur web, notamment pour du calcul interactif, du traitement de
données, etc.

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

## Accès aux environnements

Pour accéder aux environnements, vous pouvez choisir un des liens
ci-dessous, ou accéder à la [page d'accueil de
myDocker](https://mydocker.universite-paris-saclay.fr/) pour retrouver
les environnements que vous avez déjà utilisé.

:::{admonition} [Clone de JupyterHub@Paris-Saclay](https://mydocker.universite-paris-saclay.fr/shell/join/qWsmLepfAkaFqYIQBjKL)
:class: dropdown

- Logiciels: Python et ses bibliothèques classiques, SageMath, C++, R, ...
- Interfaces: JupyterLab, Jupyter, Visual Studio Code ou environnement de bureau graphique XFCE
- Ressources: dossier personnel persistent global, 2 CPU, 4Go RAM, extinction après 20 minutes sans interaction

Cet environnement multiusage est strictement identique à celui déployé
sur l'ancien service JupyterHub@Paris-Saclay et a vocation à faciliter
la transition.

Limitation: cet environnement n'a été mis à jour que à la marge depuis
septembre 2023. Les versions des logiciels installés y sont donc un
peu vieillissante. D'autre part il peut être long à charger du fait de
sa taille. **Sauf besoin spécifique, nous recommandons l'usage d'un
des environnements plus spécialisés.**
:::


:::{admonition} [Jupyter Lab et Python](https://mydocker.universite-paris-saclay.fr/shell/join/IvvgFOBBFzGLwuGJeFSb)
:class: dropdown

- Logiciels: Python, Numpy, Scipy, MatPlotLib, Pandas
- Interface: Jupyter Lab
- Ressources: dossier personnel persistent global, 2 CPU, 4Go RAM, extinction après 20 minutes sans interaction

Cet environnement donne accès à Python et ses bibliothèques
scientifiques de base (numpy, pandas, matplotlib), dans l'interface
JupyterLab. Il est notamment utilisé pour un cours nommé
[«Introduction à la programmation avec Python et
Jupyter»](https://introductionprogrammationpython.pages.centralesupelec.fr/).

:::

:::{admonition} [Jupyter Lab, Python et bibliothèques scientifiques](https://mydocker.universite-paris-saclay.fr/shell/join/IvvgFOBBFzGLwuGJeFSb)
:class: dropdown

- Logiciels: Python, Numpy, Scipy, MatPlotLib, Pandas, Scikit-learn, ...
- Interface: Jupyter Lab
- Ressources: dossier personnel persistent global, 2 CPU, 4Go RAM, extinction après 20 minutes sans interaction

Cet environnement est basé sur l'image
[jupyter-scipy-notebook](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-scipy-notebook)
de la communauté Jupyter.

:::

:::{admonition} Jupyter Lab et pyTorch
:class: dropdown

- Logiciels: Python, Numpy, Scipy, MatPlotLib, Pandas, Scikit-learn, ...
- Interface: Jupyter Lab
- Ressources: dossier personnel persistent global, 2 CPU, 4Go RAM, extinction après 20 minutes sans interaction

Cet environnement est basé sur l'image
[jupyter/pytorch-notebook](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-pytorch-notebook)
de la communauté Jupyter.

:::

:::{admonition} Jupyter Lab et C++
:class: dropdown

- Interface: Jupyter Lab
- Logiciels: compilateurs (gcc, clang) et interpréteur (cling) C++, ...
- Ressources: dossier personnel persistent global, 2 CPU, 4Go RAM, extinction après 20 minutes sans interaction

:::

:::{admonition} [Jupyter Lab et SageMath](https://mydocker.universite-paris-saclay.fr/shell/join/gkctIyHvdZkofetGeMju)
:class: dropdown

- Interface: Jupyter Lab
- Logiciels: SageMath
- Ressources: dossier personnel persistent global, 2 CPU, 4Go RAM, extinction après 20 minutes sans interaction

:::

## À propos du service

:::{admonition} Fonctionnalités essentielles
:class: hint dropdown

- Utilisation depuis un simple navigateur web.
- **Urbanisation**: authentification via la fédération d'identité
  «Recherche et Enseignement Supérieur» de Renater, ou bien par
  intégration comme outil externe dans Moodle (ou autre LMS compatible
  LTI).
- **Environnement au choix**, basés ou non sur Jupyter  
  Avec possibilité de définir des environnements personalisés pour
  choisir finement les logiciels installés.
- **Scalabilité:** dimensionné pour plusieurs centaines (milliers?)
  d'utilisateurs simultanés pour des usages interactifs légers (quelques CPUs).  
  Pour des besoins plus lourds, notamment de GPU pour des applications
  en IA, il est possible au cas par cas d'utiliser l'[instance
  myDocker de Centrale-Supélec](https://mydocker.centralesupelec.fr/),
  dont les serveurs sont loués à la demande. Nous contacter.
- **Persistence des données**
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

:::{admonition} Remerciements
:class: hint dropdown

Ce service est copiloté par la Faculté des Sciences et Centrale
Supélec, opéré par CentraleSupélec, codévelopé par CentraleSupeléc et Illuin
cofinancé par le CMA
[SaclAI-School](https://www.dataia.eu/saclai-school) et hébergé par le
mésocentre
[DataCenter@UPSud](https://www.informatique-scientifique.u-psud.fr/").

:::


## Contacts (TODO)

## Résolution de problèmes (TODO)

## Documentation

- [ ] Comment créer son propre environnement
- [ ] Comment inclure des données dans l'environnement

## Autres services

JupyterHub, SSPCloud, no
