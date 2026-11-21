# 🤾 Match des Légendes — TCG Équipe de France

Jeu de cartes (TCG) handball pour club, thème Équipe de France.

## Jouer
Site en ligne : **https://ndious.github.io/tcg-hand-equipe-de-france/**

- **Collection** : 10 joueurs des Bleus, 18 actions, 5 staff, 2 trophées.
- **Match en 2 mi-temps** : duel contre l'IA, 12 possessions alternées.

## Règles du match (v0.6)

### Mise en place
Chaque équipe respecte la compo classique du handball : **1 gardien + 2 ailiers + 2 arrières + 1 pivot + 1 demi** (gardien, pivot et demi tirés au sort).

En jeu physique : les 6 joueurs de champ sont posés **en arc de cercle, face cachée**, le gardien au centre, plus la **carte Staff** (face visible). Quand les deux équipes sont posées, on retourne tout (effectifs publics), chacun pioche **3 Action** en main secrète, et l'engagement se décide à **pile ou face**.

### Déroulé
- 2 mi-temps de **6 possessions** (3 attaques, 3 défenses par équipe, alternées).
- **Attaque** : ATQ du tireur + dé 6. Si Attaque > Défense : but ! Égalité : poteau.
- **Défense** : DEF du défenseur de champ **+1**, plus un dé **plafonné par la DEF de ton gardien**, qui reste en permanence dans les buts.
- Chaque joueur de champ ne joue qu'**une fois par mi-temps** (pivoté 90° = joué).
- **1 carte Action max par possession.** Main maintenue à **3 cartes** : à chaque Action jouée, on pioche immédiatement 1 carte.
- **Mi-temps** : tous les joueurs redeviennent disponibles, deck Action rechargé, main maintenue à 3.
- **Mulligan** : une fois par mi-temps, juste après la pioche, tu peux écarter jusqu'à 3 cartes Action et en repiocher autant (les écartées repartent sous le deck).
- **Prolongation** en cas d'égalité : 2 possessions avec effectifs et Actions rechargés.

### Les cartes Action (18 dessinées)

Charte : **+1** action de joueur sans prérequis · **+2** tactique selon le poste défensif (P1 = ailiers, P2 = arrières, P3 = pivot et demi) · **+3** spectaculaire sans condition de poste (pile ou face avant le tir : face = attaque ratée) · **Spéciale** rachat d'erreur après échec.

| Famille | Carte | Effet |
|---|---|---|
| Attaque +1 | Attaque placée | +1 dé d'attaque, non annulable |
| Attaque +2 | L'Espagnole | +2 si le défenseur adverse est en poste défensif 1 (ailier) |
| Attaque +2 | Le Yago | +2 si le défenseur adverse est en poste défensif 3 (pivot ou demi) |
| Spectaculaire +3 | Kung-fu | +3, pile ou face avant le tir |
| Spectaculaire +3 | Roucoulette | +3, pile ou face avant le tir |
| Spectaculaire +3 | Lob | +3, pile ou face avant le tir |
| Rachat d'erreur | Tir de 7 m | Si tir arrêté : dé, but si > DEF du gardien adverse |
| Rachat d'erreur | Coup franc | Si tir arrêté : relance de tous les dés |
| Rachat d'erreur | 2 minutes | Si tir arrêté : rejoue avec une carte déjà jouée |
| Rachat d'erreur | Carton jaune | Si tir arrêté : relance le dé d'attaque |
| Défense +1 | Retour placé | +1 dé de défense |
| Défense +2 | Le 5-1 | +2 si ton défenseur est en P3 (demi) |
| Défense +2 | Le 0-6 | +2 si le tireur adverse est un arrière (attaque ton P2) |
| Spectaculaire | Contre-attaque | Si tir adverse arrêté : pile ou face, face = but immédiat |
| Rachat défensif | Temps mort | Si but encaissé : relance ton dé de défense |
| Rachat défensif | Remise en jeu | Si but encaissé : relance de tous les dés |
| Rachat défensif | 2 minutes (défense) | Si but encaissé : rejoue avec un défenseur déjà joué |
| Rachat défensif | Réflexe du gardien | Si but encaissé : le gardien relance son dé plafonné, but annulé s'il dépasse |

### Deck club (34 cartes Action)

| Rareté | Cartes | Exemplaires |
|---|---|---|
| Commune | 6 cartes +1/+2 | ×3 (18) |
| Peu commune | 4 spectaculaires | ×2 (8) |
| Rare | 8 rachats d'erreur | ×1 (8) |

Principes : les joueurs = information publique, les Actions = information privée ; aucune carte ne remet un joueur en jeu ni n'en consomme un supplémentaire (seule exception symétrique : les 2 minutes).

## La carte Staff (encadrement du club)

Posée face visible avec l'équipe, **1 activation par mi-temps**, déclenchable à n'importe quel moment. Après activation, la carte pivote « engagée » comme un joueur. Aucune influence sur le duel tireur/défenseur : tout se joue sur l'information et la tactique. La main de 3 est inviolable : toute carte gagnée se paie par une défausse.

| # | Action | Effet |
|---|---|---|
| 1 | Vestiaire adverse | Révèle la main Action adverse jusqu'à la fin de la possession en cours |
| 2 | Recherche tactique | Défausse 1 carte, fouille le deck, choisis une carte tactique (+2), montre-la, ajoute-la à ta main, remélange |
| 3 | Pression sur le banc | Révèle 2 cartes de la main adverse, tu en défausses 1 au choix, l'adversaire pioche 1 |
| 4 | Changer de jeu | Défausse 1 carte de ta main, pioche 1 carte |
| 5 | Briefing renforcé | Regarde les 3 premières cartes du deck, défausse-en 1, remets les 2 autres sur le dessus dans l'ordre de ton choix |

Le coach, la direction et les bénévoles du club choisissent « leur » action pour leur carte respective : 5 profils naturels de personnalités du club. Pas d'effet passif pour l'instant.

## Déploiement
GitHub Pages via GitHub Actions (`.github/workflows/pages.yml`) : chaque push sur `main` redéploie le site.

---
Projet passion pour club de handball. Contenu illustratif, non affilié à la FFHandball.

> Dernière mise à jour : v0.8 (tactiques par poste défensif P1/P2/P3, Écran pivot retirée, spectaculaires sans condition de poste).
