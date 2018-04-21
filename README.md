# Git útgáfustýring og samþáttun
_Git version control system_

þegar unnið er í textaskjali eða kóða er allt vinnuferlið skráð reglulega í Git. Til verksins notum við **Git Bash** skipanalínuviðmótið (_CLI_). Það fylgir með Git forritinu sem hægt er að sækja hér https://git-scm.com/.
Með skráningunni ``` $ git add .' ``` og ``` $ git commit -m 'lýsing...' ``` býr maður til tímalínu þar sem hægt að fara í gegnum allt vinnuferlið, byrjað aftur á öðrum tímapunkti og tekið aðra stefnu með kóðann á nýrri grein _(branch)_, hann getur síðan þróast samhliða upprunalegum kóða. Engin takmörk eru fyrir því hversu margar greinar geta verið í gangi í einu skjali en það er skynsamlegt að hafa þær fáar og blanda saman kóðanum reglulega _(merge)_ við upprunalega útgáfu _(master)_ eða eyða útgáfum sem eru ekki að ganga upp. Hér að neðan er upptalning á helstu Git skipunum sem notaðar eru við samþáttunina.

> $ git [add] [commit] [status] [push] [pull] [log] [diff] [branch] [merge]

[Sjá yfirlit yfir helstu Git skipanir hér](https://github.com/vefhonnun/Git-aefingaverkefni/blob/master/Lesefni/github-git-cheat-sheet.pdf)

# Git hópverkefni 

Í allri hópverkavinnu á tölvubraut á að nota GIT útgáfustjórnun og vakta verkefnin á meðan unnið er í þeim. 
Þegar unnið er í hópverkefnum á að skrá vinnuferlið reglulega  í umsjónarkerfið og alltaf uppfæra verkefnið á GitHub í lok vinnutímans ```$ git push. ```
### Afritun _„Fork“_ og speglun _„Git clone“_
Töluverður munur er á ofantöldum aðgerðum. Þegar geymsla (_repository_) er gogguð „Fork“ þá færðu _nýtt eintak_ af geymslunni sem tilheyrir þínum reikningi. Þú getur gert hvað sem er við innihald geymslunnar og það hefur engin áhrif á upprunalega geymslu. Hinsvegar ef þú villt láta höfund geymslunnar vita hvað þú ert að bralla, þá getur þú sent honum skilaboð í gegnum skilaboðakerfið **„Pull request“**. Þar getur höfundurinn borið saman kóðann sem þú ert með við upprunalegan kóða og ef þín lausn er betri þá er hún sett saman við upprunalegan kóða með skipuninni **„Merge request“**.

Þegar nemendur vinna saman í hópverkefni þá er skynsamlegt að spegla **„Git clone“** geymsluna yfir á tölvur þátttakenda þannig að allir hafa sitt eintak af verkefninu. Git sér síðan um samræmingu gagna þannig að ekkert ósamræmi er í gögnum og ekki er hægt að yfirrita gömul skjöl yfir ný. Til að nemendur geti unnið saman í einni geymslu þá verður stofnandi geymslunnar að veita aðgang að henni [sjá nánar hér.](https://github.com/vefhonnun/Git-aefingaverkefni/blob/master/Lesefni/Samstarf%20%C3%A1%20GitHub.pdf) Síðan geta allir uppfært og sent efni í sömu geymslu á GitHub. 

### Á Github geta nemendur:
* stofnað sameiginlega geymslu e. _"repository"_ um verkefni
* stofnandi geymslunnar getur bætt við notendum _contributors_ með sömu réttindum og hann sjálfur hefur á geymslunni . 
* notendur _contributors_ geta breytt og bætt við efni eins og stofnandinn. 
* öll vinnugögn hópverkefnisins eiga að vera á Github

### Æfingaverkefni  

*	**GitHub** - Afritun _(Fork)_
	*	Eftir að hafa stofnað hóp þá afritar **einn** úr hópnum þessa geymslu (_e. repository_) með <br> goggunaraðferðinni _**„Fork Repository“**_  á eigin GitHub reikning (_GitHub Account_). Síðan deilir hann aðgangi að geymslunni, [sjá nánar í lesefni/Samstarf](Lesefni/Samstarf%20á%20GitHub.pdf).
*	**Sameiginleg geymsla _(repository)_** 
	* Í _"Git Bash"_ er geymslan spegluð _**„Git clone“**_ yfir á tölvur hópsins þannig að allir eru með eigin útgáfu af henni. Dæmi: ``` $ https://github.com/ÞínGeymsla/Git-aefingaverkefni.git ``` 
	*	[Í möppunni "docs"](docs/) er vefsíða og stílsíða. Nemendur eiga að búa til fjórar greinar **_(branch)_** þar sem vefsíðan er með nýju stílsniði á hverri grein. 
	*	Farið eftir leiðbeiningum hér í ["Vefsíða tengd GitHub geymlsu.pdf"](Lesefni/Vefsíða%20tengd%20GitHub%20geymslu.pdf) og tengið vefsíðuna í docs möppunni við GitHub geymsluna.
	* 	Setjið tengil í README.md skrána sem vísar á vefinn eins og hér er sýnt.
	https://vefhonnun.github.io/Git-aefingaverkefni/
*	[Lesefni til stuðnings verkefninu](Lesefni/)
*	[Bjargir/Wiki](Bjargir.md)

Git ritþór (editor)
Til að nota Sublime ritþórinn í staðinn fyrir VIM (_default editor_) í Git Bash.

> git config --global core.editor "'c:/program files/sublime text 3/subl.exe' -w"


<!--
### Námsmat:
*	Fjórar greinar af vefsíðu unnar af báðum nemendum (2x2). 
*	Vefsíða á að vera tengd geymslunni sbr. verklýsinguna hér að ofan.

#### Allar aðgerðir og skráningar (Branches/Commits) eiga að vera í sögu skjalana ( Commits / History ) á GitHub. Ef skráningarsagan (commits) fylgir ekki með þá er engin einkun gefin fyrir verkefnið.  

> Verkefnaskil: setjið tengil sem vísar á GitHub geymsluna í _'Athugasemdir'_ **í Innu**. 
-->
