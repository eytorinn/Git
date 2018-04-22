# Git hópverkefnavinna
Git er hannað til að halda utanum verkefni með dreifðri útgáfustjórn _(Distribute Version Control)_. Það þýðir að þátttakendur í hópverkefni eru allir með eintak af öllu verkefninu. Git sér um að hindra árekstra og eyðingu gagna sem eru í vinnslu. Mikið öryggi fellst í dreifingu verksins vegna þess að ekki er hægt að eyða öllum útgáfunum í einu eða öll vinnsla stöðvist vegna þess að miðlari _(server)_ fer á hliðina vegna álags eða kerfishruns.

> Í allri hópverkavinnu á tölvubraut á að nota GIT útgáfustjórnun og vakta verkefnin á meðan unnið er í þeim. 
Þegar unnið er í hópverkefnum á að skrá vinnuferlið reglulega  í umsjónarkerfið og alltaf uppfæra verkefnið á GitHub í lok vinnutímans ```$ git push. ```

### Afritun _„Fork“_ og speglun _„Git clone“_
Töluverður munur er á ofantöldum aðgerðum. Þegar geymsla (_repository_) er gogguð „Fork“ þá færðu _nýtt eintak_ af geymslunni sem tilheyrir þínum reikningi. Þú getur gert hvað sem er við innihald geymslunnar og það hefur engin áhrif á upprunalega geymslu. Hinsvegar ef þú villt láta höfund geymslunnar vita hvað þú ert að bralla, þá getur þú sent honum skilaboð í gegnum skilaboðakerfið **„Pull request“**. Þar getur höfundurinn borið saman kóðann sem þú ert með við upprunalegan kóða og ef þín lausn er betri þá er hægt að setja hana saman við upprunalegan kóða með skipuninni **„Merge request“**.

Þegar nemendur vinna saman í hópverkefni þá er skynsamlegt að spegla **„Git clone“** geymsluna yfir á tölvur þátttakenda þannig að allir hafa sitt eintak af verkefninu. Git sér síðan um samræmingu gagna þannig að ekkert ósamræmi er í gögnum og ekki er hægt að yfirrita gömul skjöl yfir ný. Til að nemendur geti unnið saman í einni geymslu þá verður stofnandi geymslunnar að veita aðgang að henni [sjá nánar hér.](https://github.com/vefhonnun/Git-aefingaverkefni/blob/master/Lesefni/Samstarf%20%C3%A1%20GitHub.pdf) Síðan geta allir uppfært og sent efni í sömu geymslu á GitHub. 

### Æfingaverkefni
* [Afritun og speglun](afritun.md)
* [Ágreiningur](ágreiningur.md)

#### Ýtarefni
* [Lesefni til stuðnings verkefninu](Lesefni/)
* [Bjargir](Bjargir.md)

Yfirlit
* [GIT kynning](Git/)
<!--
### Námsmat:
*	Fjórar greinar af vefsíðu unnar af báðum nemendum (2x2). 
*	Vefsíða á að vera tengd geymslunni sbr. verklýsinguna hér að ofan.

#### Allar aðgerðir og skráningar (Branches/Commits) eiga að vera í sögu skjalana ( Commits / History ) á GitHub. Ef skráningarsagan (commits) fylgir ekki með þá er engin einkun gefin fyrir verkefnið.  

> Verkefnaskil: setjið tengil sem vísar á GitHub geymsluna í _'Athugasemdir'_ **í Innu**. 
-->
