# Unnið með Git

> í vinnslu .......

Git umsjónarkerfið er opin hugbúnaður sem hægt er að sækja hér https://git-scm.com/. Á þeirri vefsíðu er að finna ýtarlegar upplýsingar um kosti þess að nota Git. Hér er farið yfir helstu aðgerðir í Git sem auka öryggi og bætir verkferli í allri verkefnavinnu. Þegar unnið er í textaskjali eða kóða er allt vinnuferlið skráð reglulega í Git. Til verksins notum við **Git Bash** skipanalínuviðmótið (_CLI_). Það fylgir með Git hugbúnaðinum.
#### Verklag.
* Þegar þú byrjar á verkefni þá
	1. opnar þú **Git** umsjónarkerfið 
	2. stofnar geymslu (_repository_) sem heldur utan um verkefnið
	3. lætur Git vakta verkferlið 

#### Geymsla búin til (local)
og sett á github

#### Geymsla búin til (Github)
og afrituð - Git clone

#### Umsjón og samþáttun

Hér að neðan er upptalning á helstu Git skipunum sem notaðar eru við samþáttunina.

> $ git [add] [commit] [status] [push] [pull] [log] [diff] [branch] [merge]

Með skráningunni ``` $ git add .' ``` og ``` $ git commit -m 'lýsing...' ``` í Git skráum við stöðu verksins sem við eru að vinna að og Git býr til tímamót. 
Eftir nokkrar skráningar höfum við myndað tímalínu og þá er hægt að fara í gegnum allt vinnuferlið, byrjað aftur á öðrum tímapunkti og tekið aðra stefnu með kóðann á nýrri grein _(branch)_, hann getur síðan þróast samhliða upprunalegum kóða. Engin takmörk eru fyrir því hversu margar greinar geta verið í gangi í einu skjali en það er skynsamlegt að hafa þær fáar og blanda saman kóðanum reglulega _(merge)_ við upprunalega útgáfu _(master)_ eða eyða útgáfum sem eru ekki að ganga upp. 

[Sjá yfirlit yfir helstu Git skipanir hér](https://github.com/vefhonnun/Git-aefingaverkefni/blob/master/Lesefni/github-git-cheat-sheet.pdf)

https://try.github.io/levels/1/challenges/1

> Do not forget to add a comment when you commit your files. Strategic commenting in Git is as important as commenting code. If you accidentally forget to add a comment and end up in a strange screen where you can no longer enter any commands, press ESC and type :q! followed by ENTER.

#### Yfirlit
* [Kynning](README.md)
* [GIT hópverkefnavinna](Hópverkefnavinna.md)