---
tags: tip
title: Voi paska, pitäis kumota tiedostoon tehdyt muutokset!
id: undo-a-file
order: 8
---

```git
# etsi hash aikaisemmalle commitille enne tiedoston muuttumista
git log
# käytä nuolinäppäimiä liikkuaksei ylös ja alas päin historiassa
# kun olet löytänyt sopivan commitin, ota sen hash talteen
git checkout [commitin hash] -- path/to/file
# tiedoston vanha version löytyy hakemistostasi
git commit -m "Wow, you don't have to copy-paste to undo"
git commit -m "Vau, sinun ei tarvitse kopioida-liittää peruuttaaksesi"
```

Kun vihdoin ymmärisin tämän, se oli ISO juttu. ISO. I-S-O. Millä vitun planeetalla `checkout --` on järkevää nimi komennolle tiedoston muuttosten kumoamiseen?:shakes-fist-at-linus-torvalds:
