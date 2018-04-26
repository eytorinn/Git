# Git umsjón og samþáttun

> í vinnslu .......

Efir að hafa opnað **Git Bash** og vísað á Git geymslu þá fylgist forritið með allri textavinnslu og breytingum á þeim. Með skráningu skipana```$ git add .'``` og ```$ git commit -m 'lýsing...' ``` þá er staða verksins afrituð og Git býr til tímamót. 

Eftir nokkrar skráningar höfum við myndað tímalínu og þá er hægt að fara í gegnum allt vinnuferlið, byrjað aftur á öðrum tímapunkti og tekið aðra stefnu með kóðann á nýrri grein _(branch)_, hann getur síðan þróast samhliða upprunalegum kóða. 
#### Timaflakk
Til að skoða tímalínuna þá er ``` git log ``` skipunin notuð. Með hverri vistun fylgir skýringin sem þú skráðir ásamt langri talnarunu **"04c98c7b7744c9c6e23ba28a302710513805e89a"**. Það er þessi talnaruna sem vísað er í til að komast aftur á tiltekin stað í verkferlinu. Til að komast síðan út úr log glugganum er nóg að ýta á "CTRL" + "Q".
#### Greinar í Git
Engin takmörk eru fyrir því hversu margar greinar geta verið í gangi í einu skjali en það er skynsamlegt að hafa þær fáar og blanda saman kóðanum reglulega _(merge)_ við upprunalega útgáfu _(master)_ eða eyða útgáfum sem eru ekki að ganga upp. 

Hér að neðan er upptalning á helstu Git skipunum sem notaðar eru við samþáttunina.

> $ git [add] [commit] [status] [push] [pull] [log] [diff] [branch] [merge]

Sjá nánar á:
* [Yfirlit yfir hesltu skipanir í Git](Lesefni/github-git-cheat-sheet.pdf)
* http://guides.beanstalkapp.com/version-control/common-git-commands.html
* https://try.github.io/levels/1/challenges/1

#### Yfirlit
* [Unnið með GIT](Git.md)
* [Git umsjón og samþáttun](Umsjón.md)
* [GIT hópverkefnavinna](Hópverkefnavinna.md)
* [Bjargir](Bjargir.md)