---
tags: tip
title: Voi paska, commitoin jo, mutta tajusti että pitäsi tehdä vielä pieni muutos!
id: change-last-commit
order: 2
---

```git
# tee muutoksesi
git add . # tai yksittäiset tiedostot
git commit --amend --no-edit
# nyt viisimin committisi sisältää kyseisen muutoksen!
# Varoitus: älä koskaan ammendoi julkista committia
```

Itselleni käy usein näin kun commitoin, testejä/lintteriä ajaessa huomaan etten laittanut välilyönti yhtäkuin merkin jälkee. Voit myös tehdä muutokset uutena committina ja suorittaa `rebase -i` yhdistääksesi kummatkin, mutta ammendointi on pirusti nopeampi.


*Varoitus: Älä koskaan ammendoi committia mikä on puskettu  julkiseen/jaettuun haaraan! Ammendoi vain paikallisia committeja, muuten tulet aiheuttamaan ongelmia.

