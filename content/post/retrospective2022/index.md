---
title: L'année 2022 dans le monde de la data science
subtitle: Rétrospective d'une année riche
toc: true
summary: |
  La _data science_ a beaucoup fait parler d'elle en 2022,
  notamment du fait des deux coups
  médiatiques d'[openAI](https://openai.com/), à savoir [`Dall-E`](https://openai.com/dall-e-2/)
  et [`chatGPT`](https://openai.com/blog/chatgpt/),
  qui ont créé un réel engouement au delà de la sphère
  des praticiens de la donnée. Cet article 
  ouvre une série de _post_ rétrospectifs sur l'année 2022
  pour faire un bilan de l'actualité de la _data science_
  et du réseau. 
# Link this post with a project
projects: [dataviz, recap2022]


# Date published
date: '2022-12-31T00:00:00Z'

# Date updated
lastmod: '2022-12-31T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: true

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - linogaliana

tags:
  - NLP
  - retrospective
  - observable
  - quarto
  - deep learning
  - infolettre

categories:
  - Insee
  - Retrospective
  - Infolettre
---

_Vous désirez intégrer la liste de diffusion ? Un mail à <ssphub-contact@insee.fr> suffit_ 



La fin de l'année est généralement synonyme de
bétisiers, _best of_ ou
rétrospectives personnalisées qui nous permettent
de nous rappeler les événements marquants de l'année.

Pour célébrer la fin de l'année 2022, la _newsletter_
de janvier adopte un format un peu spécial pour
proposer, en deux temps, deux rétrospectives.

Cette première _newsletter_ revient 
sur les principaux événements de l'année 2022 dans le monde de
la _data science_. La [seconde _newsletter_](https://ssphub.netlify.app/post/recap2022/) proposera
une rétrospective quantitative sur le
réseau des _data scientists_ de la statistique publique, à la manière
des rétrospectives personnalisées de nos applications préférées.


# Les IA créatrices de contenu à l'honneur

Si l'année 2022 a été particulièrement riche dans le domaine
de la _data science_, c'est principalement grâce à deux coups
médiatiques d'[OpenAI](https://openai.com/),
à savoir [`Dall-E`](https://openai.com/dall-e-2/)
et [`ChatGPT`](https://openai.com/blog/chatgpt/). 

Ces deux outils ont
beaucoup fait parler d'eux, au-delà
de la sphère traditionnelle de la _data science_.
Le _buzz_ a été intense sur `Twitter`
ou sur `Mastodon`, 
le réseau social dont le nombre d'utilisateurs
a nettement augmenté en réaction
au rachat de `Twitter` par Elon Musk en fin d'année.

<figure>
    <img src="https://i.chzbgr.com/full/9717138688/hC5E738A3/chatgpt-will-see-all-criticisms-its-training-data-on-next-update-some-are-not-surviving-uprising"
         alt="Illustration d'un modèle de diffusion" width="500" height="600">
</figure>


Ces innovations, parce qu'elles pourraient
avoir des effets à long terme sur la manière dont le grand public
appréhende l'intelligence artificielle, 
ont beaucoup intéressé les médias traditionnels,
notamment [_Le Monde_](https://www.lemonde.fr/economie/article/2022/12/06/chatgpt-le-logiciel-capable-d-ecrire-des-petits-textes-confondants_6153252_3234.html), 
[_The Economist_ et sa _"Nouvelle Frontière"_](https://www.economist.com/news/2022/06/11/how-a-computer-designed-this-weeks-cover) ou [le _Guardian_](https://www.theguardian.com/commentisfree/2022/dec/10/i-wrote-this-column-myself-but-how-long-before-a-chatbot-could-do-it-for-me)
qui s'interroge sur la nature des tâches que l'intelligence artificielle pourra remplacer à terme :
procédurales et régies par des règles bien définies ou bien également des activités nécessitant de la créativité et des capacités d'analyse ?

Pour une fois, il ne s'agit donc pas de souligner 
exclusivement les limites de ces modèles voire leurs
dérives ([_deep fake_](https://fr.wikipedia.org/wiki/Deepfake),
[biais racistes](https://www.washingtonpost.com/technology/2022/07/16/racist-robots-ai/)...) mais aussi
de s'enthousiasmer sur
leur [potentiel créatif](https://www.platformer.news/p/how-dall-e-could-power-a-creative).
Il est difficile de rester insensible à certaines des créations
artistiques des modèles [`Dall-E`](https://dalle2.gallery/#search-random), [`Stable Diffusion`](https://stablediffusion.fr/gallery), [Midjourney](https://www.midjourney.com/showcase/recent/) et consorts
ou de résister à la tentation de tester la capacité
de `ChatGPT` à répondre à des questions complexes
Les chercheurs, et pas des moindres (notamment [Andrew Ng](https://twitter.com/andrewyng/status/1600284752258686976?lang=fr) ou [Gaël Varoquaux](https://theconversation.com/beau-parleur-comme-une-ia-196084)) se sont également saisis de cette question et ont
souligné
les biais de raisonnement et excès de confiance de ces IA. 

![https://github.com/Stability-AI/stablediffusion](https://raw.githubusercontent.com/CompVis/stable-diffusion/2ff270f4e0c884d9684fa038f6d84d8600a94b39/assets/stable-samples/txt2img/merged-0006.png)

Si vous désirez utiliser `Python` de manière créative pour générer du contenu avec `Stable Diffusion`,
vous pouvez consulter [ce tutoriel](https://pythonds.linogaliana.fr/dalle/) qui fonctionne
sur le [`SSPCloud`](https://www.sspcloud.fr/) ou sur `Google Colab`.

<figure>
    <img src="https://i.chzbgr.com/full/9717140480/hD779E54E/writing-shit-like-elon-musk-suicide-note-and-robert-ebert-goncharov-review-please-stop-need-sleep"
         alt="Illustration d'un modèle de diffusion" width="500" height="600">
</figure>




# Le succès des modèles de diffusion

Ces [IA génératrices de contenu](https://pub.towardsai.net/generative-ai-and-future-c3b1695876f2)
reposent toutes, à plusieurs niveaux, sur
des réseaux de neurone.

Le premier étage de la fusée est
un [modèle de langage](https://en.wikipedia.org/wiki/Language_model) (_large language model_)
qui synthétise un langage en un ensemble complexe de paramètres. 
Les plus connus sont [BERT](https://en.wikipedia.org/wiki/BERT_(language_model))
et [GPT-3](https://en.wikipedia.org/wiki/GPT-3). 
L'inflation dans le nombre de paramètres n'est pas prête de s'arrêter.
Si les ressources nécessaires à entraîner en 2018 le modèle BERT (110 millions de paramètres)
avaient déjà [été critiquées](https://arxiv.org/abs/1906.02243) en raison
de leur coût financier et environnemental, cette complexité
a encore augmenté depuis. Le modèle `GPT-3`, sorti en 2020, et qui sert de base à
`Dall-E` et `ChatGPT` intègre 175 milliards de paramètres. Un chiffre qui apparaît minime
par rapport aux 17O trillions de paramètres attendus pour le modèle `GPT-4` en 2023.

En ce qui concerne les IA créatrices de contenu visuel, 
le deuxième étage de la fusée est un modèle d'analyse d'image qui apprend à associer
des images à une description textuelle afin de détecter des structures communes entre
des mots ou des séquences de mots et des formes sur des images. 
Il s'agit de déconstruire une forme en une structure minimale de pixels qui permet de
l'identifier. 


<figure>
    <img src="https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fdb4ef038-9c72-42b5-9383-26952d95aea0_740x141.jpeg"
         alt="Illustration d'un modèle de diffusion">
    <figcaption><i>Source: <a href="https://magazine.sebastianraschka.com/p/ahead-of-ai-1-a-diffusion-of-innovations" target="_blank">Sebastian Raschka</a></i></figcaption>
</figure>



Ensuite, pour générer une image à partir d'une description inédite intervient
le [modèle de diffusion](https://en.wikipedia.org/wiki/Diffusion_model)
qui reconstruit une image à partir du mélange de l'ensemble des pixels qui traduisent
les concepts principaux d'une instruction.
L'une des explications les plus pédagogiques
pour comprendre le fonctionnement de ces modèles 
vient du [_Washington Post_](https://www.washingtonpost.com/technology/interactive/2022/ai-image-generator/).

Sinon, on peut demander directement à `ChatGPT` de nous expliquer:

![](diffusion.png)

# L'actualité dans le monde du _deep learning_

Si le succès d'estime de ces IA génératrices consacre les modèles de 
diffusion, l'année du _deep learning_ ne se réduit pas à cette actualité.

L'année a notamment été marquée par la compétition
entre les librairies et
écosystèmes [`TensorFlow`](https://www.tensorflow.org/?hl=fr), développé par
`Google`, et [`PyTorch`](https://pytorch.org/) projet initié par `Facebook/Meta`. 
`PyTorch`, plus récent, bénéficie d'une dynamique plus ascendante que `TensorFlow`.
Le [succès d'`HuggingFace`](https://twitter.com/huggingface/status/1609162974626779136?s=20&t=XUCGBC_PL60IdHjia8wXNA),
plateforme de mise à disposition de modèles, et
où les [implémentations `PyTorch` sont systématiques alors que celles en `TensorFlow` sont rares](https://www.assemblyai.com/blog/pytorch-vs-tensorflow-in-2022/#pytorch-vs-tensorflowmodel-availability) a participé à la diffusion de `PyTorch`. 

Preuve du succès de `PyTorch`, cet écosystème est dissocié de `Meta` depuis septembre afin de devenir un outil généraliste [géré par la `Linux Foundation`](https://www.linuxfoundation.org/blog/blog/welcoming-pytorch-to-the-linux-foundation). À l'inverse,
[`Google` semble se détacher graduellement de `TensorFlow`](https://twitter.com/ylecun/status/1538419932475555840) pour privilégier son nouvel écosystème `JAX`. 

# Du changement côté `RStudio`

Depuis quelques années, `RStudio` a fait le choix
de devenir un écosystème de _data science_
généraliste et non plus exclusivement attaché au langage `R`. 

Cette année, cela s'est traduit par
la publication, très commentée, de [`Quarto`](https://quarto.org/)
qui vise à proposer, dans de nombreux langages de programmation,
des fonctionalités de publications reproductibles
équivalentes à
l'un des produits emblématiques de `RStudio`, à savoir
[`R Markdown`](https://rmarkdown.rstudio.com/).
Rien de mieux pour être
convaincu de l'intérêt de cet outil que
d'observer [la galerie d'exemples](https://quarto.org/docs/gallery/),
d'explorer [la documentation très riche](https://quarto.org/),
ou de [tester soi-même](https://quarto.org/docs/get-started/hello/rstudio.html) sur un exemple.
Cet été, `RStudio` a également annoncé que `Shiny`, un autre produit emblématique,
serait maintenant disponible sous [`Python`](https://shiny.rstudio.com/py/), 
comme alternative à [`Dash`](https://dash.plotly.com/) ou [`Streamlit`](https://streamlit.io/).


L'année 2022 a été l'occasion, pour `RStudio`, d'un autre changement, symbolique celui-ci.
Afin de détacher son image du langage `R`,
l'entreprise a en effet changé de nom pour devenir [`posit`](https://posit.co/). 
L'entreprise n'a néanmoins pas abandonné son activité foisonnante dans `R` puisque
Hadley Wickham a commencé à publier de nouveaux chapitres pour
une nouvelle édition augmentée de
l'ouvrage de référence [_R For Data Science_](https://r4ds.had.co.nz/).

# `Observable` devient un incontournable dans le monde de la dataviz

Pour permettre des visualisations interactives,
cela fait plusieurs années que `JavaScript` est un incontournable et
que le [_web assembly_](https://fr.wikipedia.org/wiki/WebAssembly)
retient [de plus en plus d'attention](https://twitter.com/solomonstre/status/1111004913222324225).

Les journaux traditionnels utilisent ainsi de plus en plus
le _data scrollytelling_ , cette technique de narration
qui consiste à présenter des informations sous forme de récit interactif, 
en utilisant une combinaison de texte et de graphiques qui apparaissent et
disparaissent en fonction des actions du lecteur.
L'un des exemples les plus réussis des dernières années a sans doute été 
la visualisation du [_New York Times_ _"How the virus got out"_](https://www.nytimes.com/interactive/2020/03/22/world/coronavirus-spread.html). Cette approche a également été adoptée par
le Ministère de l'Agriculture pour diffuser les 
chiffrés clés du [recensement agricole](https://vizagreste.agriculture.gouv.fr/). 
Nos voisins anglais ne sont pas en reste puisque les derniers résultats du
recensement sont proposés sur un [site web remarquable de fluidité](https://www.ons.gov.uk/census/maps/choropleth/population/age/resident-age-3a/aged-16-to-64-years). 

Afin de permettre une diffusion accrue de visualisations en `JavaScript`,
[Mike Bostock](https://en.wikipedia.org/wiki/Mike_Bostock), déjà créateur 
de la librairie de dataviz de référence [`D3.js`](https://en.wikipedia.org/wiki/D3.js),
est à l'origine de la plateforme [`observable`](https://observablehq.com/), sorte de 
`Github` de la _dataviz_ permettant du partage et de la réutilisation de _notebooks_ réactifs. 
En cette année 2022, la plateforme a connu un véritable _boom_ et est devenu un incontournable
dans le domaine. L'une des raisons est l'ajout de fonctionalités qui permettent d'étendre
le public cible au delà des développeurs _web_, déjà accoutumés à `Javascript`.
Parmi les 
fonctionalités les plus remarquables,
la possibilité depuis Novembre
d'utiliser des [requêtes SQL](https://observablehq.com/@ericmauviere/duckdb-redonne-nouvelle-vie-sql)
grâce à [`DuckDB`](https://observablehq.com/@observablehq/duckdb)
permet aux habitués de `R` ou de `Python` de
retrouver des manipulations auxquels ils sont habitués. 
La librairie [`Plot`](https://observablehq.com/@observablehq/plot) offre
une [grammaire proche de `ggplot2`](https://observablehq.com/@observablehq/plot-from-ggplot2).

La communauté des cartographes a été particulièrement active sur `Observable`, notamment 
à l'occasion du [#30daymapchallenge](https://observablehq.com/collection/@observablehq/30-day-map-challenge).
[Nicolas Bertin (`neocarto`)](https://observablehq.com/@neocartocnrs), dont on ne peut
que recommander l'[introduction à `Observable`](/talk/presentation-dobservable-par-nicolas-lambert/) faite pour le réseau,
ou [Eric Mauvière](https://observablehq.com/@ericmauviere) font partie des
comptes à suivre dans la communauté
francophone. 

`Observable`, en tant que langage construit sur `JavaScript`,
est également disponible pour les utilisateurs de [`Quarto`](https://quarto.org/docs/interactive/ojs/),
ce qui permet de mettre à disposition des visualisation réactives sans passer nécessairement par la plateforme [observablehq.com](https://observablehq.com/)
pour mettre à disposition des visualisations réactives, ce qui constitue une alternative intéressante aux applications qui nécessitent un serveur en arrière plan, comme `Shiny` ou `Dash`.

![](/talk/presentation-dobservable-par-nicolas-lambert/observable1.png)
![](/talk/presentation-dobservable-par-nicolas-lambert/observable2.png)


# Les autres actualités en France

Le rapport du conseil d'État
pour la [construction d'une IA de "confiance"](https://www.conseil-etat.fr/content/download/175739/file/Etude%20%C3%A0%20la%20demande%20du%20PM%20-%20IA%20et%20action%20publique.pdf)
a donc été publié en une année 2022 où les avancées techniques des dernières années commencent 
à être accessibles grâce à des outils plus grand public, ce qui va nécessairement soulever des enjeux
éthiques et juridiques. 

Le [projet `Onyxia`](https://www.onyxia.sh/), qui vise à proposer une infrastructure de _data science_
à l'état de l'art pour _data scientists_, a organisé son deuxième _Openlab_. L'occasion de 
revenir sur le projet, sa philosophie, ses dernières avancées mais aussi d'échanger sur les perspectives
de réutilisation dans de multiples environnements et de nouer des partenariats qui 
permettront au projet de grandir encore  en 2023. 

<!-----
- onyxia
- IA: rapport conseil d'Etat: https://www.conseil-etat.fr/content/download/175739/file/Etude%20%C3%A0%20la%20demande%20du%20PM%20-%20IA%20et%20action%20publique.pdf + UNECE Adasmm
- Ryanair v lastminute.com, j’ai grossièrement résumé le cas page 85 dans le support
- Data scientist 10 ans après
------->
