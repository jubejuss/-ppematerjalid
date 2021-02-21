# Õppematerjal
Markdown'i juhend:  
https://www.markdownguide.org/basic-syntax/  
## Git'i materjalid  
### git'i cheat sheet:  
https://gist.github.com/webbj74/3788509  

- git init
- git status
- git commit -m ""
- git log
- git checkout commit...
- git emote -v
- git branch
- git checkout UUSHARU
- git checkout -b UUSHARU
- git merge UUSHARU (pead olema kuskil ja siis sinna liidad UUSHARU)
- git branch -d UUSHARU (-d delete)

Alusta tööd alati pull käsuga, et sikutada remotest vajalik alla.

### Juhend oma arvutist giti tegemiseks
Kõigepealt tee oma arvutis git init.  
Siis git add . , et lisada kõik vajalik.  
Vajadusel ka .gitignore  
Siis git commit -m "siia kommentaar"  

**Siis ühenda github'iga**
- New
- Create
- Push an existing repository...
ja järgi juhiseid

Mergemisega on pisut segane, aga:
Kui soovid kaht oksa ühendada, siis mine sinna, kuhu teise tahad tõmmata ja git merge UUSHARU. Kui on erinevused, siis ta pakub võimaluse ümber kirjutada või asendada teisega emma, kumma või lisada mõlemad:  

![Image of Yaktocat](images/merge.png)

Kui mingil põhjusel ei saa, võid katkestada: git merge --abort