---
title: Physique - Electricité en courant continu
author: Azra
layout: post
---

## - Grandeurs -

<div id="grandeurs"></div>
L’intensité $I$, en ampères (A), du courant correspond à la quantité de charges qui traverse une section d’un conducteur par unité de temps:

$$i=lim_{\delta t \rightarrow 0} ~ \frac{\delta q}{\delta t} = \frac{\mathrm{d}q}{\mathrm{d}t}$$

En régime continu :
$$I=\frac{Q}{\Delta t}$$  
	$Q$ est la charge électrique, en coulons (C)  
	$t$ est le temps, en secondes  


La tension $U$, en volts (V), est une différence potentielle entre deux points.$$U_{AB}=V_A-V_B$$  
	Mais attention, $U_{AB}$ se flèche de **$B$ à $A$.** 

 La puissance électrique, en watt (W), est égal :  
$$P=U \times I$$  

 L'énergie, en joule, se calcule ainsi de la puissance électrique, tel que :  
 $$E=P\times \Delta t$$  

## - Dipôles -

Un dipôle est un composant électrique composé de deux bornes. Il est caractérisé, dans un circuit, par l'intensité $I$ qui le traverse et la tension $U$ à ses bornes (voir [- Grandeurs -](#grandeurs)).

La **caractéristique** du dipôle est la fonction $I=f(U)$, ainsi que le graphe associé. 

Le point $M(U,I)$, est appelé point de **fonctionnement**. 

### - Propriétés -

- Un dipôle est **linéaire** si sa caractéristique est une **droite**, sinon il est dit non linéaire.

- Un dipôle est **symétrique** ou **non polarisé** si sa caractéristique est symétrique par rapport à **l'origine**, et inversement.

- Un dipôle est **passif** si sa caractéristique passe par **l'origine**. La tension aux bornes du dipôle débranchée est **nulle**. (Et inversement, s'il est actif.)

### - Conventions -

En convention **générateur**, $U$, et $I$ sont dessiné dans le même sens. Et inversement, si le dipôle est **récepteur**.

{% include image.liquid url="\conv.png" %}

### - Lois -

#### - Loi d'Ohm -
$$U=RI$$ 

Tel que :
	$R$ est la résistance en ohms ($\Omega$)
	 La caractéristique d'une résistance est une droite passante par l'origine, $I=1/R \times U$
{% include image.liquid url="\resistance.png" %}
>$P=UI=RI^2>0$ (effet Joule)

#### - Lois de Kirchhoff -

##### - Loi des nœuds -

La somme des intensités algébriques des courants qui s’approchent d’un nœud
est égale à la somme des intensités algébriques des courants qui s’en éloignent.
$$I=I_1+I_2+...+I_n$$

> Remarque : Dans un circuit, pour $n$ nœuds, il y a $n-1$ lois des nœuds indépendantes.

#### - Loi des mailles -

La somme des tensions algébriques d'une seule et même maille est toujours égale à $0$.
$$E=U_1+U_2+...+U_n$$

### - Résistance équivalente -

Dans un circuit, il est possible "de regrouper", les résistances liées en une seule. On a alors deux cas :
	Les résistances sont en **séries** : $$R_{eq}=R_1+R_2+...+R_n$$  
	Les résistances sont en **parallèles** : $$\frac{1}{R_{eq}}=\frac{1}{R_1}+\frac{1}{R_2}+...+\frac{1}{R_n} = \frac{R_1 \times R_2 \times ... \times R_3}{R_1+R_2+...+R_n}$$

### - Pont diviseur de tension - 

Le diviseur de tension est un montage électronique simple qui permet de diminuer une tension d'entrée. 
{% include image.liquid url="\diviseur.png" %}
 Pour une résistance $R_n$, la tension à ses bornes $U_{R_n}$, est : 

$$U_{R_n}=\frac{E \times R_n}{\sum R}$$
