# Jyväskylän kaupungin ostot 2012-2021    

## Esittely

Tässä tehtävässä käytetään aineistona Jyväskylän kaupungin ostolaskuja vuosilta 2012-2021, ja sitä käsitellään ja analysoidaan Pythonin Pandas-kirjaston ja JupyterLabin avulla. Tiedot on tuotu Excel-tiedostoista, jotka on ladattu 9.5.2023 Jyväskylän kaupungin avoimen datan palvelusta osoitteesta https://data.jyvaskyla.fi/data.php. Aineistosta kerrotaan sivustolla seuraavasti: 

> Tiedoissa on mukana kaupungin kaikki toimialat ja liikelaitokset. Tiedot sisältävät ostolaskutiedot sekä luottokorttiostotiedot. Ostotiedot on poimittu ostolaskujen käsittelyjärjestelmästä ja kirjanpidosta ulkoisten palvelujen ja tarvikkeiden sekä käyttöomaisuusostojen tileiltä.
>
> Tiedot mahdollistavat kaupungin hankintojen (ostojen) tarkastelun palvelualueittain toimittaja- ja tilitasoilla. Suodattamalla tietoja voidaan vertailla ostojen toteutumia erilaisten tietojen perusteella.   
>
> Luottokorttiostotiedot eivät sisällä toimittajanumeroa ja kaikkien luottokorttiostojen osalta emme saa ostopaikkatietoja ilman yksittäisten tositteiden läpikäyntiä. Y-tunnustieto puuttuu henkilötoimittajien ja luottokorttiostojen osalta.    
>
> Ylläpitäjä ja yhteys:   
> ostotiedot[at]jkl.fi    

Aineisto ei ole täydellistä, vaan se sisältää puuttuvia arvoja ja kirjoitusvirheitä, ja ostoja on kirjattu eri vuosina hieman erinimisille vastuualueille ja tileille. Apua näiden epäselvyyksien tulkintaan on ystävällisesti antanut Jyväskylän kaupungin taloussuunnittelupäällikkö Erikka Saastamoinen. Parhaasta yrityksestä huolimatta on mahdollista, että kaupungin organisaatiorakennetta vastuualueineen ja tulosyksiköineen on tässä tulkittu paikoin väärin. Mahdolliset virheet ovat omiani.       

## Rakenne   

Tehtävä on jaettu kahteen Jupyter-tiedostoon. Ensimmäinen näistä on nimeltään *ostolaskut_aineisto*, ja siinä tuodaan ostolaskuaineisto Excel-tiedostoista, ja sitä koostetaan ja siivotaan jatkokäyttöä varten. Saatu datakehikko tallennetaan lopuksi csv-tiedostoksi, ja sitä käytetään myöhemmin analyysiosiossa. Ostolaskujen analyysi kokonaisuudessaan löytyy toisesta tiedostosta *ostolaskut_anallyysi.ipynb*.