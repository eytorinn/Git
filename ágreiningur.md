# Ágreiningur _(conflicts)_
Æfingaverkefni

Það er óhjákvæmilegt í hópverkavinnu að upp komi sú staða að tvær útgáfur séu til af sama skjali. Git kemur í veg fyrir að skjöl séu yfirrituð og sýnir þess í stað ósamræmið sem er í kóða og eða texta. Til að forðast árekstra þá er það góð vinnubrögð að byrja vinnudaginn á því að tjékka hvort local útgáfan sé ekki með síðustu útgáfu verksins með skipuninni ``` $ git pull ``` af GitHub geymslunni, ef allt er í lagi kemur m.a. eftirfarandi skilaboð ``` working tree is clear, nothing to commit ```  

### Dæmi um ágreining
í vinnslu .... Hér set ég texta beint í GitHub geymsluna vitandi að þessi texti er ekki í (local) geymslunni. Síðan breyti ég skjalinu sem er í heimageymlunni. Hér finnur git að ekki er allt með feldu og sýnir báðar útgáfurnar. 

Nú skoðum við báðar útgáfurnar og eyðum annari hvorri útgáfunni eða búum til nýja sameiginlega leiðréttingu.  

#### Git Bash ritþór (editor) fyrir villuskilaboð 
Hægt er að skipta um ritþór og nota _Sublime_ ritþórinn í staðinn fyrir VIM (_default editor_) skráið eftifarandi kóða í _"Git Bash"_.

``` git config --global core.editor "'c:/program files/sublime text 3/subl.exe' -w" ```

Yfirlit
*	[Afritun og speglun](afritun.md)
*	[Ágreiningur](ágreiningur.md)
*	[Lesefni til stuðnings verkefninu](Lesefni/)
*	[Bjargir](Bjargir.md)
