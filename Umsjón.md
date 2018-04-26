# Git umsjón og samþáttun

> í vinnslu .......

Efir að hafa opnað **Git Bash** og vísað á Git geymslu þá fylgist forritið með allri textavinnslu og breytingum á þeim. Skipanirnar ```$ git add .'``` og ```$ git commit -m 'lýsing...' ``` afrita stöðu verksins og Git býr til tímamót sem hægt er að fara á síðar. 

Eftir nokkrar skráningar höfum við myndað tímalínu og þá er hægt að fara í gegnum allt vinnuferlið, byrjað aftur á öðrum tímapunkti og tekið aðra stefnu með kóðann á nýrri grein _(branch)_, hann getur síðan þróast samhliða upprunalegum kóða. 
#### Tímaflakk
Til að skoða tímalínuna þá er ```git log``` skipunin notuð. Með hverri vistun fylgir skýring (*commit -m*) sem þú skráðir ásamt langri talnarunu **"04c98c7b7744c9c6e23ba28a302710513805e89a"**. Það er þessi talnaruna sem vísað er í til að komast aftur á tiltekin stað í verkferlinu. Til að komast síðan út úr log glugganum er nóg að ýta á "CTRL" + "Q". Til að fara til baka með allt verkferlið þá er skipunin ```git checkout 04c98c7b77``` Það þarf ekki að nota alla talnarununa til að Git finni rétta færslu.
#### Greinar í Git
Git býður upp á möguleika að vera með margar útgáfur af sama kóða. Til þess þurfum við að vista kóðann á hliðargrein. 
Dæmi: þú vilt búa til nýja útgáfu af kóða sem þú ert að vinna í en byrja þar sem þú varst staddur 2 dögum fyrr. 
* ```git checkout 04c98c7b774``` -> Færir þig á eldri útgáfu af "master"
* ```git branch grein1``` -> býrð til nýja útgáfu af kóðanum, hér getur þú tekið aðra stefnu með kóðann.

Til að sameina greinar þá þarftu að vera á þeirri grein sem verður eftir
* ```git checkout master```
* ```git merge grein1```

Engin takmörk eru fyrir því hversu margar greinar geta verið í gangi í einu skjali en það er skynsamlegt að hafa þær fáar og blanda saman kóðanum reglulega _(merge)_ við upprunalega útgáfu _(master)_ eða eyða útgáfum sem eru ekki að ganga upp. 

Sjá nánar á:
* [Yfirlit yfir helstu skipanir í Git](Lesefni/github-git-cheat-sheet.pdf)
* http://guides.beanstalkapp.com/version-control/common-git-commands.html
* https://try.github.io/levels/1/challenges/1

#### Yfirlit
* [Unnið með GIT](Git.md)
* [Git umsjón og samþáttun](Umsjón.md)
* [GIT hópverkefnavinna](Hópverkefnavinna.md)
* [Bjargir](Bjargir.md)