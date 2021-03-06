# Unnið með Git

Git umsjónarkerfið er opin hugbúnaður sem hægt er að sækja hér https://git-scm.com/. Á þeirri vefsíðu er að finna ýtarlegar upplýsingar um kosti þess að nota Git. Hér er farið yfir helstu aðgerðir í Git sem auka öryggi og bætir verkferli í allri verkefnavinnu. 

Þegar unnið er í textaskjali eða kóða er allt vinnuferlið skráð reglulega í Git. Til verksins notum við **Git Bash** skipanalínuviðmótið (_CLI_) í Windows stýrikerfum. Git Bash fylgir með Git hugbúnaðinum. Í Mackintosh og Linux kerfum heitir skipanalínuviðmótið **"Terminal"**  og er til staðar í stýrikerfunum. Það sem *Git Bash* gerir m.a. er að túlka Linux skipanir yfir í Windows skipanir . Það auðveldar okkur vinnuna við umsjónarkerfið að nota aðeins eitt skipanakerfi óháð stýrikerfum.

#### Verklag 
* Stofna reikning á [GitHub](https://github.com/) :octocat:
   	* Þegar reikningur er stofnaður á GitHub þá er staðfesting send á tölvupóstfangið sem tilgreint er í umsókninni. 
   	* Eftir að hafa staðfest umsóknina þá er hægt að nota github reikningin til að búa til geymslur, afrita geymslur frá öðrum og verið í samstarfi við aðra notendur á GitHub. 

#### Geymsla búin til á vinnusvæði (_local_) og færð yfir á GitHub :two_women_holding_hands:
Þegar þú byrjar á verkefni þá:
1. opnar þú **Git Bash** CLI 
2. stofnar geymslu (_**repository**_) sem heldur utan um verkefnið
3. lætur Git vakta vinnuferlið 

Skráðu inn eftirfarandi skipanir (*Commands*) í *Git Bash*, þegar þú ýtir á [*return*] takkann þá framkvæmir Git skipunina. 
* Til að geta sent gögn yfir á GitHub frá tölvunni þinni þarftu að skrá eftrifarandi skipanir í Git Bash
 	* ```git config --global user.name "nafnReiknings" ```
 	* ```git config --global user.email "þinn@Tolvupos.tur" ```

* Hvar á geymslan að vera á tölvunni? 
	* ```cd``` er CLI skipun og stendur fyrir *"Change Directory"*
* Dæmi: 
	* ```cd Desktop/``` Þá verður geymsla búin til á skrifborði tölvunnar. [Sjá fleiri CLI skipanir](https://github.com/vefhonnun/Git/blob/master/Git.md#linux-cli-ums%C3%BDsluskipanir)

```
$ echo "# Geymsla" >> README.md
$ git init
$ git add README.md
$ git commit -m "útskýring á framkvæmd"
$ git remote add origin https://github.com/þinnReikningur/Geymsla.git
$ git push -u origin master
``` 
Hér að ofan eru sýndar 6 skipanir til að búa til Git geymslu.
Hvað gera svo þessar skipanir
1. mappa búin til **echo "#**(_sem heitir Geymsla_)" og skjal búið til **>>** sem heitir _README.md_ inn í möppunni
2. **git init** býr til umsjónarkerfi fyrir nýju geymsluna. Kerfið er í möppu sem er falin (*hidden*). Hægt er að skoða hana með því að stilla *Explorer - View - [x] Hidden items* (Ekki eiga neitt við gögnin sem eru í .git).
3. **git add .**  Git skrásetur stöðu verkefnisins á þessum tímapunkti það má kalla það sviðsetningu.
4. **git commit -m "útskýring"** Til að geta skoðað stöðuna síðar verður útskýring að fylgja sviðsetningunni.
5. **git remote add origin** Hér er "Geymsla.git" vísað á GitHub reikning þinn
6. Í fyrsta sinn sem geymslunni er ýtt úr höfn þá verður **-u origin master** að fylgja með **git push**. 
 
Eftir að geymsla hefur verið stofnuð og afriti komið fyrir á GitHub þá er næsta skref að vísa *Git Bash* á geymsluna til að vakta verkefnið, dæmi:  ```cd Desktop/geymsla/``` . Síðan er hægt að vinna í verkefninu og senda gögn á milli vinnusvæðis og GitHub með því að nota  ```git push``` til að senda gögn og ```git pull```  til að sækja gögn. Sjá nánar á [Git umsjón](Umsjón.md).

#### Geymsla búin til á GitHub og spegluð (*clone*) á (*local*) vinnusvæði :two_men_holding_hands:
Í Upplýsingatækniskólanum eru allir að vinna á innra neti skólans og milli þess og internetsins er *eldveggur*. Það þýðir að ekki er hægt að stofna geymslu á H: drifinu og senda síðan á GitHub eins og lýst er hér að ofan. Ástæðan er að GitHub miðlarinn getur ekki sótt nauðsynlegar upplýsingar um sendandann, (*öll sund eru lokuð*). Lausnin á vandamálinu er einföld. Við byrjum á því að stofna geymsluna á GitHub og speglum (*clone*) hana síðan yfir á vinnusvæðið okkar á H: drifinu. Github miðlarinn hefur þá allar upplýsingar um geymsluna og er ekki að flækjast fyrir.

#### Verklag
* Búa til geymslu á GitHub reikning -> [**New repository**]
* Það er mikilvægt að haka við **"Create repository with README.md"** einnig er skynsamlegt að velja **.gitignore** og **Licence** í leiðinni,
* Spegla (*clone*) geymsluna yfir á vinnusvæði þitt
	* [Speglun lýst myndrænt hér](Lesefni/UppsetningGithubGeymslu.pdf)
	* Þar er einnig sýnt hvernig hægt er að senda og sækja gögn (*push/pull*) 
<span id="CLI"></span>

#### Linux CLI umsýsluskipanir 
* ```pwd``` *print working directory* Sýnir staðsetningu Git Bash
* ```ls```  *list items* Sýnir öll gögn í viðkomandi möppu
* ```cd```  *change directory* Skipt um staðsetningu
* ```cd  mappa1/``` Farið ofaní möppu 1
* ```cd  mappa1/mappa2``` Farið ofaní möppu 2 sem er inn í möppu 1
* ```cd  ../``` Farið upp úr möppu
* ```cd  ../../``` Farið upp úr 2 möppum
* ```cd  ..```  Farið uppúr öllum möppum [User]
* [Yfirlit Unix/Linux skipanir](Lesefni/unixref.pdf)

#### Yfirlit
* [Git útgáfustjórnun](README.md)
* [Unnið með GIT](Git.md)
* [Git umsjón og samþáttun](Umsjón.md)
	* Verkefni: [Unnið með Git](Vinnuferli.md) og [Greinar](Greinar.md)
* [GIT samvinna](Samvinna.md)
	* Verkefni: [Hópverkefni](Hópverkefnavinna.md)
* [Bjargir](Bjargir.md)