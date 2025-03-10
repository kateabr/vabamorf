# KASUTAJASÕNASTIK EESTI KEELE MORFOLOOGILISE ANALÜÜSI JA SÜNTEESI PROGRAMMILE

## Kirjeldus
Kasutajasõnastikku otsitakse käsurealipuga **--path** määratud kataloogide loendist 
või selle puudumisel keskkonnamuutujas **PATH** loetletud kataloogidest. 
Katalooge vaadatakse läbi sellises järjekorras nagu nad loendis on. 
Kõigepealt otsitakse etteantud kataloogidest kasutajasõnastikku **et.usr.dct**, 
kui seda ei leita siis faili **et.usr.dct.utf8** ja kui seda ka ei leita siis 
faili **et.usr.dct.uc**. Programm kasutab (ainult) esimest leitud kasutajasõnastikku.

## Formaat
Kasutajasõnastik on tekstifail.

Sümboliga **#** algavaid ridu käsitletakse kommentaarina (ignoreeritakse).

Ülejäänud kasutajasõnastiku read on analoogilise formaadiga nagu 
morfoloogilise on analüsaatori väljund.

**NB! Vale tühikute, kaldkriipsude, komade jms arvu/paigutuse korral lõpetab 
morfoloogiline analüsaator töö veateatega.**

## Kodeering
Kasutajasõnastikus kasutatav kooditabel sõltub kasutajasõnastiku nimest:
* **et.usr.dct** - Windows Baltic kodeeringus lisasõnastik.
* **et.usr.dct.utf8** - UTF8 kodeeringus lisasõnastik.
* **et.usr.dct.uc** - little endian baidijärjega kahebaidises unicode kodeeringus lisasõnastik.

## Näide
**NB! Tühikute arv sõnede!**
```
l@xid    mine+sid //_V_ sid, //
r66mu    rõõm+0 //_S_ adt,//    rõõm+0 //_S_ sg p, //    rõõm+0 //_S_ sg g, //
```

## Vaata lisaks
* [Eesti keele morfloogilise analüsaatori käsureaprogramm](https://gitlab.com/tarmo.vaino/docker-elg-morf/-/blob/main/LOEMIND.md).
* [Eesti keele morfoloogiline analüsaator ELG nõuetele vastava liidesega konteineris](https://gitlab.com/tarmo.vaino/docker-elg-morf).
* [Eesti keele morfoloogilise ühestaja käsureaprogramm](https://github.com/Filosoft/vabamorf/blob/master/apps/cmdline/vmyhh/LOEMIND.md).
* [Eesti keel morfoloogiline ühestaja ELG nõuetele vastava liidesega konteineris](https://gitlab.com/tarmo.vaino/docker-elg-morf/-/blob/main/LOEMIND.md).

## Autor
Copyright © 1997-2022 OÜ Filosoft
