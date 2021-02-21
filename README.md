# Õppematerjal
Markdown'i juhend:  
https://www.markdownguide.org/basic-syntax/  
## Git'i materjalid  
### git'i cheat sheet:  
https://gist.github.com/webbj74/3788509  
https://education.github.com/git-cheat-sheet-education.pdf 

<p>GIT Cheat sheet: <a href="materials/git-cheatsheet-EN-dark.pdf">Download PDF</a>.</p>

GIT'i vahendeid: https://education.github.com/

GIT'i seletused ja õpe: https://www.gitkraken.com/learn/git/branch

**git origin on remote originaal**  
**Git HEAD – only one branch can be checked out at a time - and this is what's called the "HEAD" branch. Often, this is also referred to as the "active" or "current" branch.**

- git init
- git status
- "git add ." või kui spetsiifiline fail siis selle nimi
- git commit -m ""
- add ja commit koos: git commit -a -m "siia commit" 
- git log
- git checkout commit... taastab vastava commiti aegse seisu
- git remote -v
- git branch - näitab kõiki oksi
- "git checkout UUSHARU" liigub vastavasse harusse
- "git checkout -b UUSHARU" teeb haru ja liigub sellesse
- "git merge UUSHARU" (pead olema kuskil ja siis sinna liidad UUSHARU)
- "git branch -d UUSHARU" (-d delete)
- "git branch -D UUSHARU" kustutab jõuga
- "git push origin --delete UUSHARU" ehk, et kustuta vastava nimeline remote oks
- Fetch https://www.atlassian.com/git/tutorials/syncing/git-fetch
- https://www.git-tower.com/learn/git/faq/difference-between-git-fetch-git-pull/

Alusta tööd alati "pull" käsuga, et sikutada remotest vajalik alla.  
Kui ei saa, siis:   
git fetch --all  
Kui ikka ei saa, siis:  
git checkout -b backup-master  
Ja seejärel:  
"git reset --hard origin/SIIAVAJALIKUBRANCHINIMI" 

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

Ühtlusta oksad nii lokaalselt kui eemaolevast:
https://www.freecodecamp.org/news/how-to-delete-a-git-branch-both-locally-and-remotely/

Kui teha uus oks ja siis commitada ja pushida, tekib nii:  

❯ git push
fatal: The current branch uusoks has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin uusoks

Test