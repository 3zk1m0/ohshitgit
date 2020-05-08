---
tags: tip
title: Voi paska, yritin suorittaa Diff komennon, mutta mitään ei tapahtunu?!
id: dude-wheres-my-diff
order: 6
---

Jos olet varma että olet tehnyt muutoksia tiedostoon, mutta `diff` on silti tyhjä. Olet luultavasti lisännyt (`add`) tiedostosi jo stagelle, jolloin tarviteset erillisen lipun.

```git
git diff --staged
```

Tämä kuuluu kategoriaan &macr;\\\_(ツ)\_/&macr; (Kyllä, tiedän että tämä on ominaisuus eikä bugi. Mutta se on silti vitun hämmentävää ja epäselvää, kun se tapahtuu ensimmäistä kertaa!)
