---
tags: tip
title: Voi paska, vahingossa commitoin jotain masteriin, minkä olisi pitänyt mennä uuteen haaraan!
id: accidental-commit-master
order: 4
---

```git
# luo uusi haara masterin nykytilasta
git branch haaran-uusi-nimi
# poista master haarasta viimeisin committi
git reset HEAD~ --hard
git checkout haaran-uusi-nimi
# committisi elää nyt kyseisessä haarassa :)
```



Huom: tämä ei toimi jos olet jo puskenut commitin julkiseen/jaettuun haaraan. Jos olet yrittänyt ensin jotain muuta, saatat joutua suorittamaan `git reset HEAD@{number-of-commits-back}` komennon `HEAD~` sijaan. Tuhannet kiitokset ihmisille, jotka suosittelivat tapaa ratkaista tämän mahdollisimman nopeasti, en itse tiennyt tästä. Kiitokset kaikille!

Huom: tämä ei toimi, jos olet jo siirtänyt sitoumuksen julkiseen / jaettuun haaraan ja jos yritit ensin muita asioita, saatat joutua "palauttamaan HEAD @ {määrä-of-commits-back}" -kohdan sen sijaan. `PÄÄ ~`. Ääretön suru. Lisäksi monet monet monet ehdottivat mahtavaa tapaa tehdä tämä lyhyemmäksi, jota en tuntenut itseäni. Kiitos kaikille!