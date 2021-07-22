---
stub: true
tags:
  - score v1
---

# Combo multiplier effect

Le **combo multiplier effect** est un bug du [scoreV1](/wiki/Score/ScoreV1) qui permet au [score](/wiki/Score) de compter à l'envers (le score deviendra négatif). Il s'agit d'un défaut avec les entiers signés 32 bits où (en calcul) l'entier maximum est `2 147 483 647`. Une fois ce plafond atteint, le score commencera à compter à l'envers. Le [ScoreV2](/wiki/Score#scorev2) corrige ce problème en plafonnant le score à 1 million de points, sans tenir compte des modificateurs.

Le combo multiplier effect se produit dans les modes [osu!](/wiki/Game_mode/osu!), [osu!taiko](/wiki/Game_mode/osu!taiko), et [osu!catch](/wiki/Game_mode/osu!catch). Cela se produit parce que les modes de jeu énumérés utilisent le [combo](/wiki/Glossary/Combo_(score_multiplier)) actuel du joueur dans le calcul du score. Cela signifie qu'un joueur obtiendra un meilleur score s'il a obtenu un [full combo (FC)](/wiki/Full_combo) que quelqu'un qui a joué la même beatmap avec un combo cassé.

<!--TODO: Add images and links-->
