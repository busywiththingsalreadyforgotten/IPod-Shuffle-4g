Balabolka (komentorivisovellus), versio 1.25
Copyright (c) 2013-2015 Ilya Morozov
All Rights Reserved

WWW: http://www.cross-plus-a.com/fi/bconsole.htm
E-mail: crossa@list.ru

Lisenssi: Freeware
K�ytt�j�restelm�: Microsoft Windows XP/Vista/7/8/10
Speech API: 4.0/5.0
Microsoft Speech Platform



*** Komentorivi ***

balabolka_console.exe [options ...]


*** Komentoriviparametrit ***

-l
   N�yt� kaikki tietokoneella olevat ��net.

-g
   N�yt� kaikki saatavilla olevat audiolaitteet.

-f <tiedoston_nimi>
   Avaa tekstitiedosto.

-w <tiedoston_nimi>
   Kirjoittaa WAV-��nitiedosto. Jos t�m� parametri on sy�ty, luodaan ��nitiedosto. Jos parametria ei ole, teksti� luetaan ��neen.

-n <��nen_nimi>
   ��nen nimi (nimenosa riitt��). Jos t�t� parametria ei ole, k�ytet��n Windowsin ohjauspaneelilla valittu ��ni.
   If the option is not specified, the voice, defined by the option [-id], or the default voice of Windows will be used.

-id <luku>
   Valita tietokoneen ��ni kielitunnisteen avulla (Locale ID).
   Microsoftin kehitt�j�t my�nsiv�t sellaiset tunnisteet kaikille kielille (esimerkiksi, "1033" on englannin kielen tunniste ja "1035" � suomen kielen tunniste).
   Ohjelma valitsee listalta ensimm�isen ��nen, jonka kielitunniste vastaa tarvittavaan koodiin. Jos parametri ei ole annettu, niin k�ytet��n ��nt�, joka annettiin [�n] -parametrin avulla, tai ��nt�, joka valittiin Windowsin ohjauspaneelista.
   Tunnisteiden lista: http://msdn.microsoft.com/en-us/goglobal/bb964664.aspx

-m
   N�ytt�� valitun ��nen parametrit.

-b <luku>
   Valitse audiolaite sen numeron mukaan saatavilla olevien laitteiden listasta ��nen esitt�miseen. Oletuslaitteen numero on 0.

-c
   K�yt� leikep�yd�ss� oleva teksti.

-t <tekstin_rivi>
   K�yt� komentoriviss� oleva teksti.

-i
   K�yt� standardisy�tt�virrassa oleva teksti (STDIN).

-o
   SAPI 4: parametria ei k�ytett�viss�.
   SAPI 5 ja Microsoft Speech Platform: kirjoita ��nitieto standarditulostevirtaan (STDOUT); jos parametri on mainittu, parametri [-w] on v�litt�m�tt�.

-s <luku>
   SAPI 4: asenna ��ninopeudeksi luku 0...100 (oletusnopeutta ei ole).
   SAPI 5 ja Microsoft Speech Platform: asenna ��ninopeudeksi luku -10...10 (oletusnopeus on 0).

-p <luku>
   SAPI 4: asenna ��nens�vyksi luku 0...100 (oletuss�vy� ei ole).
   SAPI 5 ja Microsoft Speech Platform: asenna ��nens�vyksi luku -10...10 (oletuss�vy on 0).

-v <luku>
   SAPI 4: parametria ei k�ytett�viss�.
   SAPI 5 ja Microsoft Speech Platform: asenna ��nenvoimakkuudeksi luku 0...100 (oletusvoimakkuus on 100).

-e <luku>
   Asenna lauseiden v�liseksi taukopituudeksi sy�tetty luku (yksikk�n� on millisekunti). Oletuspituus on 0.

-a <luku>
   Asenna kappaleiden v�liseksi taukopituudeksi sy�tetty luku (yksikk�n� on millisekunti). Oletuspituus on 0.

-d <tiedoston_nimi>
   K�yt� sanakirja ��nt�myksen korjaamiseksi (tiedostolaajennus *.REX tai *.DIC). Komentoon voi sis�lty� muutama [-d] -parametri.

-k
   Lopettaa muiden tietokoneella toimivien konsolisovellusten toimintaa.

-ka
   Lopettaa nykyhetkess� aktiivisena olevan konsolisovelluksen toimintaa.

-q
   Lis�t� sovellus jonoon. Konsolisovellus odottaa kunnes muut ohjelmat lopettavat toimintaan.

-lrc
   SAPI 4: parametria ei k�ytett�viss�.
   SAPI 5 ja Microsoft Speech Platform: Luoda LRC-muotoinen tiedosto, jos on annettu [�w] tai [�o] �parametrit.

-sub
   SAPI 4: parametria ei k�ytett�viss�.
   SAPI 5 ja Microsoft Speech Platform: tekstin muotona on tekstitys, joka pit�� muuttaa ��nitiedostoksi ottaen huomioon annetut v�liajat.

-tray
   N�ytt�� ohjelman kuvake k�ytt�j�rjestelm�n tiedotusten alueella.
   Se antaa k�ytt�j�lle mahdollisuutta seurata operaation suorittamista, sek� lopettaa prosessi pikavalikon "Stop"-kohdan avulla.

-ln <luku>
   Selects a line from the text file by using of a line number. The line numbering starts at "1".
   The interval of numbers can be used for selecting of more than one line (for example, "26-34").
   Komentoon voi sis�lty� muutama [-ln] -parametri.

-? tai -h
   N�yt� kaikki mahdolliset parametrit.

--encoding <merkist�> tai �enc <merkist�>
   Tekstin koodaus tavallisesta sy�tt�virrasta ("ansi", "utf8" tai "unicode"). Oletuksena parametri on "ansi".

--silence-begin <luku> tai -sb <luku>
   M��ritt�� ��nitiedoston alussa olevan tauon pituus (millisekunneissa). Oletuspituus on 0.

--silence-end <luku> tai -se <luku>
   M��ritt�� ��nitiedoston lopussa olevan tauon pituus (millisekunneissa). Oletuspituus on 0.

--lrc-length <luku>
   M��ritt�� LRC-muotoisen tiedoston maksimaalinen rivin pituus (symboleissa).

--lrc-filename <tiedoston_nimi>
   LRC-muotoisen tiedoston nimi. T�m� parametri voi olla hy�dyllinen niiss� tapauksissa, kun komentoriviss� on annettu parametri [�o].

--lrc-encoding <merkist�>
   LRC-muotoisen tiedoston koodaus ("ansi", "utf8" tai "unicode"). Oletuksena parametri on "ansi".

--lrc-offset <luku>
   Antaa ajansiirto LRC-muotoiselle tiedostolle (millisekunneissa).

--lrc-artist <tekstin_rivi>
   LRC-muotoisen tiedoston tag: teoksen esitt�j�.

--lrc-album <tekstin_rivi>
   LRC-muotoisen tiedoston tag: albumi.

--lrc-title <tekstin_rivi>
   LRC-muotoisen tiedoston tag: teoksen nimi.

--lrc-author <tekstin_rivi>
   LRC-muotoisen tiedoston tag: luoja.

--lrc-creator <tekstin_rivi>
   LRC-muotoisen tiedoston tag: tiedoston luoja.

--raw
   SAPI 4: parametria ei k�ytett�viss�.
   SAPI 5 ja Microsoft Speech Platform: tallentaa ��nitiedostot RAW PCM-muotoon; tiedostot eiv�t sis�ll� WAV-muotoista otsikkoa.
   Parametria k�ytet��n [�o] -parametrin parissa.

--ignorelength
   SAPI 4: parametria ei k�ytett�viss�.
   SAPI 5 ja Microsoft Speech Platform: ei kirjoita ��nitiedoston kokoa WAV-muotoiseen otsikkoon.
   Parametria k�ytet��n [�o] -parametrin parissa.

--sub-format <tekstin_rivi>
   Tekstityksen muoto ("srt", "ssa", "ass" tai "smi"). Jos parametri ei ole annettu, niin parametri m��ritet��n tekstityksen tiedostop��tteen mukaan.

--sub-fit tai -sf
   Lis�t� automaattisesti puheen nopeutta pysy�kseen tekstityksess� annettujen v�liaikojen rajoissa.

--sub-max <luku> tai -sm <luku>
   M��ritt�� maksimaalinen puheen nopeus ��nialueella -10:st� 10:een (muuttaakseen tekstitys ��nitiedostoksi).

--deletefile tai -df
   Poistaa tekstitiedosto ��neen lukemisen tai ��nitiedoston tallentamisen j�lkeen.


*** Esimerkkej� ***

balabolka_console.exe -l

balabolka_console.exe -n "Microsoft Anna" -m

balabolka_console.exe -f "d:\Text\book.txt" -w "d:\Sound\book.wav" -n "Emma"

balabolka_console.exe -n "Callie" -c -d "d:\rex\rules.rex" -d "d:\dic\rules.dic"

balabolka_console.exe -n "Sanna" -t "Teksi luetaan hitaasti." -s -5 -v 70

balabolka_console.exe -k

balabolka_console.exe -f "d:\Text\book.txt" -w "d:\Sound\book.wav" -lrc --lrc-length 80 --lrc-title "The Lord of the Rings"

balabolka_console.exe -f "d:\Text\film.srt" -w "d:\Sound\film.wav" -n "Laura" --sub-fit --sub-max 2


Esimerkki sovelluksen k�ytt�mist� LAME.EXE �apuohjelman parissa:

balabolka_console.exe -f d:\book.txt -n Sanna -o --raw | lame.exe -r -s 22.05 -m m -h - d:\book.mp3


Esimerkki sovelluksen k�ytt�mist� OGGENC2.EXE �apuohjelman parissa:

balabolka_console.exe -f d:\book.txt -n Sanna -o --ignorelength | oggenc2.exe --ignorelength - -o d:\book.ogg


Esimerkki sovelluksen k�ytt�mist� WMAENCODE.EXE �apuohjelman parissa:

balabolka_console.exe -f d:\book.txt -n Sanna -o --ignorelength | wmaencode.exe - d:\book.wma --ignorelength


*** Konfiguraatiotiedosto ***

Parametrit voi tallentaa "balabolka_console.cfg" -nimiseen konfiguraatiotiedostoon, joka sijaitsee sovelluksen kansiossa.

Tiedoston sis�llyksen esimerkki:
===============
-f d:\Text\book.txt
-w d:\Sound\book.wav
-n Microsoft Anna
-s 2
-p -1
-v 95
-e 300
-d d:\rex\rules.rex
-d d:\dic\rules.dic
-lrc
--lrc-length 75
--lrc-encoding utf8
--lrc-offset 300
===============

Sovellus voi yhdist�� konfiguraatiotiedostossa olevat ja komentorivin parametrit.


*** Audio Clips ***

The application allows to insert links to external WAV files (audio clips) into text. Audio clip tag will look like:

{{Audio=C:\Sounds\ring.wav}}

When speaking text aloud, the program will pause when the audio clip tag is reached, play the audio clip and resume speaking.
When converting to audio files, the audio clip will be embedded in the audio file created by the application.


*** Lisenssi ***

Sovelluksen kaupallinen k�ytt�oikeus:
- toiminimelle rajoituksetta;
- oikeushenkil�it� koskevat rajoitukset on mainittu Balabolkan lisenssisopimuksessa.

Sovelluksen kaupallinen k�ytt� sallittu ainoastaan oikeudenomistajan luvasta.

###