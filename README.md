# livre-blanc-seo
Ouvert à toutes les contributions. Partager ce qu'il faut savoir pour bien référencer un site.

Pour une version plus agréable à lire, vous pouvez aller ici https://mathrobin.github.io/livre-blanc-seo

:information_source: Pour contribuer, vous pouvez soit écrire du contenu, soit :
- donner votre avis ;
- râler ;
- applaudir ;
- remonter des erreurs ;
- parler de ce projet (ou écrire sur ce projet) ;
- corriger des fautes qu'elles soient de français ou techniques, grossières ou non ;
- sûrement beaucoup d'autres choses.
Quoi que vous fassiez, ça se passe par ici : https://github.com/MathRobin/livre-blanc-seo/issues

PS : quoi qu'il en soit, d'avance : merci ! :thumbsup:

Fait avec :heart: pour toutes et tous

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

## Table des matières

* [URLs](#urls)
   * [Domaine et localisation](#domaine-et-localisation)
   * [Sous domaine](#sous-domaine)
   * [La requête](#la-requête)
      * [Usage du / terminal](#usage-du--terminal)
   * [Protocole HTTPS](#protocole-https)
   * [Protocole HTTP 2](#protocole-http-2)
* [Code](#code)
   * [Contenu](#contenu)
      * [Liens internes et externes](#liens-internes-et-externes)
      * [Ratio HTML / Texte](#ratio-html--texte)
      * [Hiérarchie de la page](#hierarchie-de-la-page)
   * [Headers](#headers)
      * [CSP](#csp)
      * [STS](#sts)
   * [Meta tags](#meta-tags)
      * [Canonical](#canonical)
      * [Description](#description)
      * [Author](#author)
      * [OpenGraph](#opengraph)
      * [Twitter Cards](#twitter-cards)
      * [Alternate Lang](#alternate-lang)
      * [Publisher](#publisher)
      * [Title](#title)
   * [JavaScript](#javascript)
   * [Ligne de flottaison](#ligne-de-flottaison)
   * [Sitemaps](#sitemaps)
   * [Schema](#schema)
   * [AMP](#amp)
   * [FIA](#fia)
   * [Favicons](#favicons)
      * [Apple Touch Icon](#apple-touch-icon)
      * [Shortcut icon](#shortcut-icon)
      * [Icon](#icon)
* [Outils](#outils)
   * [Google](#google)
      * [Google Search Console](#google-search-console)
      * [Google Analytics](#google-analytics)
      * [Embed API](#embed-api)
* [Algorithmes Google](#algorithmes-google)
    * [PageRank](#pagerank)
    * [Pénalités](#pénalités)
    * [Google Panda](#google-panda)
    * [Google Penguin](#google-penguin)
    * [Page Layout](#page-layout)
    * [PayDay Loan](#payday-loan)
   * [Bing](#bing)
      * [Bing Webmaster Tools](#bing-webmaster-tools)
   * [Mozilla](#mozilla)
      * [Mozilla Observatory](#mozilla-observatory)
   * [Indépendants](#indépendants)
* [Le monde extérieur](#le-monde-extérieur)
   * [Backlinks](#backlinks)
      * [Annuaires](#annuaires)
   * [Réseaux sociaux](#réseaux-sociaux)
      * [Page facebook](#page-facebook)
      * [Compte Twitter](#compte-twitter)
      * [Instagram](#instagram)
      * [Youtube](#youtube)

## URLs
### Domaine et localisation
Ici se situeront les conseils concernant le domaine à utiliser.

Par exemple qu'il est préférable d'utiliser un .fr pour un site qui vise le marché français et non un .com, plutôt destiné aux USA.

### Sous domaine

Ce qu'il faut savoir sur avec ou sans www, les autres sous-domaines.

Par défaut Google (quid des autres moteurs ?), considère que les domaines www.[unSite.unTld] et [unSite.unTld] doivent être des sites différents. Si vous n'avez pas prévu d'utiliser les deux sous-domaines en tant que sites indépendants, il est préférable d'en choisir un comme référence et de rediriger toute URL de l'autre via 301 vers le premier.

### La requête

Comment faire une URL proprement pour tout ce qui suit le domaine ?

#### Usage du / terminal

### Protocole HTTPS

Quid de l'usage de HTTPS face à HTTP ?

### Protocole HTTP 2

Quid de l'usage de HTTP 2 ?

## Code

Ce qu'il faut savoir côté code

### Contenu
#### Hiérarchie de la page

La hiérarchie de la page est définie comme dans tous documents, via ses "titres" : titre du document, titres des chapitres, titres des paragraphes etc en allant en décroissance d'importance.

Côté HTML, la norme considère jusqu'à 6 niveaux de profondeur, allant de H1 à H6 ("H" pour "heading"). H1 étant le titre le plus important, H6, le plus bas niveau de profondeur pris en compte.

La norme d'un point de vue SEO est d'avoir :
- un seul et unique H1, logiquement, votre document n'est pas nommé de plusieurs façons
- au moins un H2, parce que vous avez au moins un chapitre dans tout document

Précisons au passage que logiquement, votre site ne contient idéalement pas de duplicate content, et donc intrinsèquement, tous les H1 de votre site se doivent d'être uniques.

Pour aller plus loin :

http://www.webrankinfo.com/dossiers/techniques/balises-h1-h2-h3

Vidéo de Matt Cutts [_"More than one H1 on a page: good or bad?"_](https://www.youtube.com/watch?v=GIn5qJKU8VM)
Il y explique que pour lui, en soit, ce n'est pas mauvais d'avoir plusieurs H1, mais que c'est dangereux parce que compromet la bonne compréhension de la structure de la page.

#### Liens internes et externes
#### Ratio HTML / Texte

### Headers

Dans les en-têtes de vos pages, un certain nombre d'infos doivent être présentes. Surtout pour une question de sécurité.

#### CSP

Permet de réduire les risques d'attaque XSS. N'est pas un critère SEO chez Google mais on peut parier que des moteurs se préoccupant de la confidentialité soient intéressés par la présence de cette en-tête.

Pour aller plus loin :

https://content-security-policy.com/

#### STS

### Meta tags
#### Alternate Lang

Il peut être utile d’indiquer aux moteurs de recherche que votre page a une version traduite dispo en ligne. Cela se fait ainsi : ``` <link rel="alternate" hreflang="<ici le code langue>" href="<url>" /> ```
(cela peut aussi se faire via entête HTTP, sitemap)

C'est utile en cas de traduction complète, partielle (seulement le contenu et non l'interface), ou en cas de légères variations de contenu (ex: anglais vs américain, etc.).

Pour aller plus loin :

Source : https://support.google.com/webmasters/answer/189077?hl=en

#### Author

#### Canonical

La balise ``` <link rel="canonical" href="contenu de référence" /> ``` permet d'éviter de se faire taxer de "duplicate content" (contenu dupliqué : ce qui induit des pénalités sur le référencement). Elle sert à indiquer en cas de contenu dupliqué l'adresse du contenu de référence. Typiquement, cela s'applique si l'on a :

- un moteur de blog qui permet d'atteindre le même contenu depuis plusieurs URLs
- la même page produit qui se retrouve dans des catégories/chemins/URLs différents
- la même page produit qui possède des URLs dynamiques en raison de la session utilisateur et / ou de la préférence de recherche
- etc.

À noter : elle sert aussi en cas de simple rewriting, pour éviter de se faire pourrir ses adresses. Ex : un concurrent s'amuse à référencer votre billet ayant l'id 666 avec foo.com/vive_le_prOn_666 : l'adresse fonctionne, le rewriting aussi (mais il serait dommage d'être référencé ainsi, et de risquer en plus une pénalité de duplicate content). Toutefois, si vous avez mis un canonical vers foo.com/mon_bel_article_666 la vilaine tentative sera vaine.

Pour aller plus loin :

Source : https://support.google.com/webmasters/answer/139066?hl=en

Vidéo de Matt Cutts [_"Canonical Link Element"_](https://www.youtube.com/watch?v=Cm9onOGTgeM)

#### Meta-description

La meta-description est un élément clé pour attirer vos visiteurs. En soit, elle ne compte pas pour le référencement. Cette description s'affiche dans les résultats Google. Au delà des 160 caractères, le reste ne s'affichera pas et est donc inutile. Autant ne pas alourdir votre page avec du contenu en trop.

Pour chaque page, elle doit être unique et être comprise entre 150 et 160 caractères.

Pour aller plus loin :

Source : https://moz.com/learn/seo/meta-description

Vidéo de Matt Cutts [_"Is it necessary for every page to have a meta description?"_](https://www.youtube.com/watch?v=W4gr88oHb-k)

#### OpenGraph

#### Publisher

#### Twitter Cards

#### Title

Bien qu'il ne s'agit pas à proprement parler d'une balise ``` meta ``` , la balise ``` title ``` permet de donnner un titre à la page. Bien qu'elle ne s'affiche pas dans le viewport, elle est utilisée notamment par les navigateurs pour donner un titre aux onglets et par les moteurs de recherche comme titre principal dans les résultats (SERP). C'est dire son importance et le soin qu'il faut lui apporter.

Parmi les élements à retenir, le ``` title ``` devrait :

- avoir une longueur comprise entre 65 et 70 caractères,
- refléter le contenu de la page,
- contenir les mots-clés importants,
- être différent pour chaque page.

Le ``` <title> ``` devrait être placé sous la balise ``` <meta charset="utf-8"> ``` (Cf. [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate) pour plus de détails sur l'ordre des balises ``` meta ```).

Pour aller plus loin :

- [À quoi servent les balises META ?](http://www.alsacreations.com/article/lire/628-balises-meta.html)
- [Comment faire une bonne balise TITLE pour un bon référencement](http://www.webrankinfo.com/dossiers/debutants/balise-title)
- [Comment bien optimiser sa balise title et meta description ?](http://www.eskimoz.fr/balise-title-meta-description/)


### JavaScript

Ce qui est compris ou non.

### Ligne de flottaison

La ligne de flottaison est la limite virtuelle entre la partie visible et non visible de la page à son affichage.

Tout ce qui se situe au-dessus de cette ligne doit être chargé en priorité. Comme dans beaucoup de choses, la première impression est la plus importante.

Au delà d'une question de rapidité ou de priorisation d'affichage, il faut savoir que près de 80% des utilisateurs ne vont pas voir en dessous de la ligne de flottaison. Les éléments les plus importants doivent donc se situer au-dessus.

Pour aller plus loin :

http://www.seonity.com/definition-la-ligne-de-flottaison.php

### Sitemaps

Usage d'un sitemap pour les pages indexables
Usage d'un sitemap alternatif provisoire pour les redirections 301 et 302

### Schema
https://schema.org/

### AMP
https://www.ampproject.org/

### FIA
https://instantarticles.fb.com/

### Favicons
#### Apple Touch Icon
#### Shortcut icon
#### Icon

## Outils
### Google
#### Google Search Console
https://www.google.com/webmasters/tools/home

#### Google Analytics
https://www.google.fr/intl/fr/analytics/

#### Embed API
https://ga-dev-tools.appspot.com/embed-api/basic-dashboard/

####  Algorithmes Google
Google a mis en place de nombreux algorithmes pour améliorer la qualité de ses résultats : amélioration des contenus, lutte contre le spam, gestion de la publicité, performances du site, etc.

##### PageRank
Le PageRank est l'algorithme qui permet à Google de connaître le nombre de liens qui pointent vers une page donnée. Plus il existe de liens vers cette page et plus la page est populaire. En gros, on peut dire que le PageRank indique la probabilité de tomber sur une page donnée en suivant des liens. Le nombre de liens vers une page est tempéré par la qualité et le classement des liens qui pointent vers elle.

##### Pénalités
A côté du PageRank, Google a mis en place une série de pénalités pour éviter que des pages de qualité douteuse ne "trustent" les premiers résultats. Cf. http://www.webrankinfo.com/dossiers/conseils/algos-google

###### Google Panda
https://webmasters.googleblog.com/2011/05/more-guidance-on-building-high-quality.html

###### Google Penguin
https://webmasters.googleblog.com/2016/09/penguin-is-now-part-of-our-core.html

###### Page Layout
Publicité envahissante
https://webmasters.googleblog.com/2012/01/page-layout-algorithm-improvement.html

###### PayDay Loan
Antispam
http://searchengineland.com/google-pay-day-loan-algorithm-google-search-algorithm-update-to-target-spammy-queries-162941


### Bing
#### Bing Webmaster Tools
http://www.bing.com/toolbox/webmaster

### Mozilla
#### Mozilla Observatory
https://observatory.mozilla.org/

### Indépendants
- onpage.org
- woorank
- https://www.seobility.net/en/

## Le monde extérieur
### Backlinks
#### Annuaires
### Réseaux sociaux
#### Page facebook
#### Compte Twitter
#### Instagram
#### Youtube
