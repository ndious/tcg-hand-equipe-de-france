# 🤾 Match des Légendes — TCG Équipe de France

Jeu de cartes (TCG) handball pour club, thème Équipe de France.

## Jouer
Site en ligne : **https://ndious.github.io/tcg-hand-equipe-de-france/**

- **Collection** : 10 joueurs des Bleus, 4 actions, 2 trophées.
- **Match en 2 mi-temps** : duel contre l'IA, 12 possessions alternées.

## Règles du match (v0.6)

### Mise en place
Chaque équipe respecte la compo classique du handball : **1 gardien + 2 ailiers + 2 arrières + 1 pivot + 1 demi** (gardien, pivot et demi tirés au sort).

En jeu physique : les 6 joueurs de champ sont posés **en arc de cercle, face cachée**, le gardien au centre. Quand les deux équipes sont posées, on retourne tout (effectifs publics), on pioche **6 Action** chacune (main secrète), et l'engagement se décide à **pile ou face**.

### Déroulé
- 2 mi-temps de **6 possessions** (3 attaques, 3 défenses par équipe, alternées).
- **Attaque** : ATQ du tireur + dé 6. Si Attaque > Défense : but ! Égalité : poteau.
- **Défense** : DEF du défenseur de champ **+1**, plus un dé **plafonné par la DEF de ton gardien**, qui reste en permanence dans les buts.
- Chaque joueur de champ ne joue qu'**une fois par mi-temps** (pivoté 90° = joué).
- **1 carte Action max par possession.**
- **Mi-temps** : tous les joueurs redeviennent disponibles, chaque équipe pioche 6 nouvelles Actions.
- **Mulligan** : une fois par mi-temps, juste après la pioche, tu peux écarter jusqu'à 3 cartes Action et en repiocher autant (les écartées repartent sous le deck).
- **Prolongation** en cas d'égalité : 2 possessions avec effectifs et Actions rechargés.

### Les cartes Action (19 dessinées)

Charte : **+1** action de joueur sans prérequis · **+2** tactique avec prérequis · **+3** spectaculaire (pile ou face avant le tir : face = attaque ratée) · **Spéciale** rachat d'erreur après échec.

| Famille | Carte | Effet |
|---|---|---|
| Attaque +1 | Attaque placée | +1 dé d'attaque, non annulable |
| Attaque +2 | L'Espagnole | +2 si le tireur est arrière ou ailier |
| Attaque +2 | Le Yago | +2 si le défenseur adverse est le demi-centre |
| Attaque +2 | L'Écran pivot | +2 si le tireur est arrière et ton pivot pas encore joué |
| Spectaculaire +3 | Kung-fu (pivot) | +3, pile ou face avant le tir |
| Spectaculaire +3 | Roucoulette (ailier) | +3, pile ou face avant le tir |
| Spectaculaire +3 | Lob (arrière) | +3, pile ou face avant le tir |
| Rachat d'erreur | Tir de 7 m | Si tir arrêté : dé, but si > DEF du gardien adverse |
| Rachat d'erreur | Coup franc | Si tir arrêté : relance de tous les dés |
| Rachat d'erreur | 2 minutes | Si tir arrêté : rejoue avec une carte déjà jouée |
| Rachat d'erreur | Carton jaune | Si tir arrêté : relance le dé d'attaque |
| Défense +1 | Retour placé | +1 dé de défense |
| Défense +2 | Le 5-1 | +2 si ton défenseur est le demi-centre |
| Défense +2 | Le 0-6 | +2 si le tireur adverse est un arrière |
| Spectaculaire | Contre-attaque | Si tir adverse arrêté : pile ou face, face = but immédiat |
| Rachat défensif | Temps mort | Si but encaissé : relance ton dé de défense |
| Rachat défensif | Remise en jeu | Si but encaissé : relance de tous les dés |
| Rachat défensif | 2 minutes (défense) | Si but encaissé : rejoue avec un défenseur déjà joué |
| Rachat défensif | Réflexe du gardien | Si but encaissé : le gardien relance son dé plafonné, but annulé s'il dépasse |

### Deck club (37 cartes Action)

| Rareté | Cartes | Exemplaires |
|---|---|---|
| Commune | 7 cartes +1/+2 | ×3 (21) |
| Peu commune | 4 spectaculaires | ×2 (8) |
| Rare | 8 rachats d'erreur | ×1 (8) |

Principes : les joueurs = information publique, les Actions = information privée ; aucune carte ne remet un joueur en jeu ni n'en consomme un supplémentaire (seule exception symétrique : les 2 minutes).

## Déploiement
GitHub Pages via GitHub Actions (`.github/workflows/pages.yml`) : chaque push sur `main` redéploie le site.

---
Projet passion pour club de handball. Contenu illustratif, non affilié à la FFHandball.