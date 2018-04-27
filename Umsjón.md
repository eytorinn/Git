# Git umsjón og samþáttun

#### Git add [filename]
Efir að hafa opnað **Git Bash** og vísað á Git geymslu þá fylgist forritið með allri textavinnslu og breytingum á þeim. Skipanirnar ```$ git add [heiti skjals]'``` og ```$ git commit -m 'lýsing...' ``` afrita stöðu verksins og Git býr til tímamót sem hægt er að fara á síðar. Þessi aðgerð er kölluð **sviðsetning** (*staging*). Skipunin ```$ git add **.**```  tekur allar skrár sem hafa verið breytt eða bætt við á vinnusvæðinu
#### Git Commit -m ´Lýsing verkþáttar'
Eftir nokkrar skráningar höfum við myndað tímalínu og þá er hægt að fara í gegnum allt vinnuferlið, þá skiptir máli hvað var skráð í *commit* skipunina svo hægt sé að byrja aftur á öðrum tímapunkti og tekið aðra stefnu með kóðann á nýrri grein (*branch*), hann getur síðan þróast samhliða upprunalegum kóða og á einhverjum tímapunkti sameinaður (*merge*) aðalgreininni sem nefnd er **"Master"**. 
#### Tímaflakk
Til að skoða tímalínuna þá er ```git log``` skipunin notuð. Með hverri vistun fylgir skýring (*commit -m*) sem þú skráðir ásamt langri talnarunu **"04c98c7b7744c9c6e23ba28a302710513805e89a"**. Það er þessi talnaruna sem vísað er í til að komast aftur á tiltekin stað í verkferlinu. Til að komast síðan út úr log glugganum er nóg að ýta á "CTRL" + "Q". Til að fara til baka með allt verkferlið þá er skipunin ```git checkout 04c98c7b77``` Það þarf ekki að nota alla talnarununa til að Git finni rétta færslu.
#### Greinar í Git (_Branches_)
Það má sjá fyrir sér Git kerfið sem tré með stofni og greinum. Stofnin er nefndur *"Master"* og ef þú slærð inn skipunina ```git branch``` þá birtir Git lista yfir allar greinar sem eru í notkun í geymslunni. 
* Í upphafi er aðeins stofnin (*Master*) í geymslunni
* Til að búa til grein er skipunin ```git branch [heiti greinar]``` notuð. 
* Til að fara yfir á grein er skipunin ```git checkout [heiti greinar]``` notuð.

Git býður upp á möguleika að vera með margar útgáfur af sama kóða. Dæmi: þú vilt búa til nýja útgáfu af kóða sem þú ert að vinna í en byrja þar sem þú varst staddur 2 dögum fyrr. 

* ```git checkout 04c98c7b774``` -> Færir þig á eldri útgáfu af "master"
* ```git branch grein1``` -> býr til nýja útgáfu af kóðanum sem gerð var 2 dögum fyrr, hér getur þú tekið aðra stefnu með kóðann.

Til að sameina greinar þá þarftu að vera á þeirri grein sem verður eftir t.d.
* ```git checkout master```
* ```git merge grein1```

Engin takmörk eru fyrir því hversu margar greinar geta verið í gangi í einu skjali en það er skynsamlegt að hafa þær fáar og blanda saman kóðanum reglulega _(merge)_ við upprunalega útgáfu _(master)_ eða eyða útgáfum sem eru ekki að ganga upp. 

Til að eyða grein þá þarftu að vera á "master"
* ```git -d grein1```

Bjargir:
* [Yfirlit yfir helstu skipanir í Git](Lesefni/github-git-cheat-sheet.pdf)
* http://guides.beanstalkapp.com/version-control/common-git-commands.html
* https://try.github.io/levels/1/challenges/1

#### Yfirlit
* [Unnið með GIT](Git.md)
* [Git umsjón og samþáttun](Umsjón.md)
* [GIT hópverkefnavinna](Hópverkefnavinna.md)
* [Bjargir](Bjargir.md)