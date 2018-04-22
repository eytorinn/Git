# Git útgáfustýring og samþáttun
_Git version control system_

Ekkert er eins leiðinlegt eins og að yfirrita eða eyða kóða sem tekið hefur langan tíma að þróa og fullgera. Þetta vandamál hefur fylgt ritvinnslu á tölvum frá upphafi og margt gert til að leysa vandamálið. Yfirleitt hafa umsjónarkerfi verið miðlæg og notendur tekið út og bætt við gögnum inn á einn miðlara. Vandamálið við þá lausn er að miðlarinn getur bilað eða virkað einkennilega og mikil vinna fer þá til spillis.  Lausnin sem kynnt er hér er byggð upp á gagnadreifingu. Hver þátttakandi er með allt verkefnið á sinni tölvu og síðan er ein miðlæg útgáfa á internetinu sem tengir alla saman í gegnum GIT útgáfustýrikerfið. Kerfið hentar líka einstaklingum sem eru að vinna að þróunarverkefnum og miklu máli skiptir að hafa fulla stjórn á verkefninu frá uppahafi til enda.  

Þegar unnið er í textaskjali eða kóða er allt vinnuferlið skráð reglulega í Git. Til verksins notum við **Git Bash** skipanalínuviðmótið (_CLI_). Það fylgir með Git umsjónarkerfinu sem hægt er að sækja hér https://git-scm.com/. 

Með skráningunni ``` $ git add .' ``` og ``` $ git commit -m 'lýsing...' ``` í Git býr maður til tímamót sem mynda tímalínu. Síðar í vinnuferlinu er hægt að fara í gegnum allt vinnuferlið, byrjað aftur á öðrum tímapunkti og tekið aðra stefnu með kóðann á nýrri grein _(branch)_, hann getur síðan þróast samhliða upprunalegum kóða. Engin takmörk eru fyrir því hversu margar greinar geta verið í gangi í einu skjali en það er skynsamlegt að hafa þær fáar og blanda saman kóðanum reglulega _(merge)_ við upprunalega útgáfu _(master)_ eða eyða útgáfum sem eru ekki að ganga upp. Hér að neðan er upptalning á helstu Git skipunum sem notaðar eru við samþáttunina.

> $ git [add] [commit] [status] [push] [pull] [log] [diff] [branch] [merge]

[Sjá yfirlit yfir helstu Git skipanir hér](https://github.com/vefhonnun/Git-aefingaverkefni/blob/master/Lesefni/github-git-cheat-sheet.pdf)

[GIT hópverkefnavinna](Hópverkefnavinna.md)