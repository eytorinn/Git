# Ágreiningur _(conflict)_
Æfingaverkefni

Það er óhjákvæmilegt í hópverkavinnu að upp komi sú staða að tvær útgáfur séu til af sama skjali. Git kemur í veg fyrir að skjöl séu yfirrituð og sýnir þess í stað ósamræmið sem er í kóða og eða texta. Til að forðast árekstra þá er það góð vinnubrögð að byrja vinnudaginn á því að tjékka hvort (_local_) heimaútgáfan sé ekki með síðustu útgáfu verksins með skipuninni ``` $ git pull ``` af GitHub geymslunni, ef allt er í lagi kemur m.a. eftirfarandi skilaboð 
``` working tree is clear, nothing to commit ```  
Ef sú staða kemur upp að tvær útgáfur eru til af sama skjali, þá sýnir git báðar útgáfurnar í Git Bash. Til að lagafæra skjölin þarf að sækja útgáfuna sem er á github ``` $ git pull ``` síðan bæta henni við local útgáfuna ``` git add . ``` og tilgreina vandræðin ``` $ git commit -m 'ágreiningur í texta' ``` þá erum við með báðar útgáfurnar heima og getum lagfært skjalið.
```
<<<<<<< HEAD
### Dæmi
í vinnslu .... þessi local útgáfa er gömul og lúinn .. :o
=======
### Dæmi 
í vinnslu .... Hér set ég texta beint í GitHub geymsluna vitandi að þessi texti 
er ekki í (local) geymslunni. ;) 
Hér finnur git að ekki er allt með feldu og sýnir báðar útgáfurnar. 
>>>>>>> 4849c518d18d8ea59b65bd063bd8d9e96bc04830
``` 
það er hægt að eyða annari hvorri útgáfunni eða búa til nýja sameiginlega leiðréttingu. Þegar því er lokið þá er skjalið uppfært í Git, ``` $ git add . ``` og ``` $ git commit -m 'ágreiningur lagfærður' ``` síðan ``` $ git push ```. 
#### Git Bash ritþór (editor) fyrir villuskilaboð 
Hægt er að skipta um ritþór og nota _Sublime_ ritþórinn í staðinn fyrir VIM (_default editor_) skráið eftifarandi kóða í _"Git Bash"_.
``` git config --global core.editor "'c:/program files/sublime text 3/subl.exe' -w" ```
Yfirlit
* [Kynning](README.md)
* [Unnið í Git](Git.md)
* [Afritun og speglun](Afritun.md)
* [Lesefni til stuðnings verkefninu](Lesefni/)
* [Bjargir](Bjargir.md)
