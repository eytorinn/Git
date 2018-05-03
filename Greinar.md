# Greinar í Git (_Branches_) :deciduous_tree:

Git býður upp á möguleika að vera með margar útgáfur af sama kóða. Dæmi: þú vilt búa til nýja útgáfu af kóða sem þú ert að vinna í en byrja þar sem þú varst staddur 2 dögum fyrr. 
* ```git log``` Git birtir lista með öllum færslum (*commits*). Veldu fyrstu 7 tölurnar úr þeirri talnarunu sem passar við færsluna sem þú vilt komast á.
*	ýttu á takkann "q" til að komast úr listanum
* ```git checkout 04c98c7``` -> Færir þig á eldri útgáfu af "master"
* ```git branch grein1``` -> býr til nýja útgáfu af kóðanum sem gerð var 2 dögum fyrr, hér getur þú tekið aðra stefnu með kóðann.

Til að sameina greinar þá þarftu að vera á þeirri grein sem verður eftir t.d.
* ```git checkout master```
* ```git merge grein1``` greinin er sameinuð "master"

Engin takmörk eru fyrir því hversu margar greinar geta verið í gangi í einu skjali en það er skynsamlegt að hafa þær fáar og blanda saman kóðanum reglulega _(merge)_ við upprunalega útgáfu _(master)_ eða eyða útgáfum sem eru ekki að ganga upp. 

Til að eyða grein þá þarftu að vera á "master"
* ```git -d grein1``` greininni er eytt, það hefur ekki áhrif á stöðu "master" eða annara greina.

### Æfingaverkefni :running: :running:
Nú höldum við áfram með skjalið sem þú bjóst til (Git_svör.md), Skoðaðu allar færslurnar í skjalinu ```git log``` í Git Bash og afritaðu (*copy*) talnarununa sem fylgir **5. svarinu** (Fyrstu 7 tölurnar)
1. Skráðu síðan ```git checkout 1234567``` (*paste* tölurnar 7)
2. Búðu til nýja grein ```git branch [heiti greinar]``` 
3. Farðu yfir á greinina ```git checkout [heiti greinar]```
	* Bættu við eftirfarandi texta aftan við 5. svarið
	<pre>Lorem ipsum .... </pre>
4. Sendu nýju greinina yfir á GitHub

* [Git vinnuferlið](Vinnuferli.md)
* [Git greinar]()

Bjargir:
* https://try.github.io/levels/1/challenges/1
* http://guides.beanstalkapp.com/version-control/common-git-commands.html
* https://git-scm.com/book/en/v2/Getting-Started-Git-Basics
* https://git-scm.com/docs
* [Listi yfir helstu skipanir í Git](Lesefni/github-git-cheat-sheet.pdf)

#### Yfirlit
* [Kynning](README.md)
* [Unnið með GIT](Git.md)
* Git umsjón og samþáttun
* [GIT hópverkefnavinna](Hópverkefnavinna.md)
* [Bjargir](Bjargir.md)