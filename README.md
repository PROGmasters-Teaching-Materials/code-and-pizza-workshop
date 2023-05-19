# Amiről ma beszélgetni fogunk = fogalmak

**Mesterséges Intelligencia (AI)**: Ez a számítástudomány egy területe, amelynek célja olyan rendszerek létrehozása, amelyek képesek olyan feladatok elvégzésére, amelyek normális esetben emberi intelligenciát igényelnének. Ilyen feladatok a természetes nyelv értése, minták felismerése, problémák megoldása és döntéshozatal.

**Gépi Tanulás (ML)**: Ez az AI egyik része, amely az adatok alapján döntéseket vagy előrejelzéseket lehetővé tevő algoritmusok fejlesztését foglalja magában. Az explicit szabályok programozása helyett az ML rendszerek nagy mennyiségű adatból tanulnak, és az alapján hoznak előrejelzéseket vagy döntéseket.

**Generatív Előre Betanított Transzformátor (GPT)**: Ez egy olyan AI modell, amelyet az OpenAI fejlesztett ki, és amely a természetes nyelv megértését és generálását igénylő feladatokra terveztek. A GPT nagy mennyiségű szövegadaton tanul, és képes emberihez hasonló szöveget generálni a megadott feladatok alapján.

**ChatGPT**: Ez a GPT modellnek egy olyan változata, amely kifejezetten beszélgetéses célú finomhangolásra készült. Képes beszélgetéses módon válaszokat generálni a szöveges bemenetekre, ami hasznossá teszi olyan alkalmazásokban, mint a chatbotok vagy a virtuális asszisztensek.

**GPT API**: Ez egy olyan interfész, amelyet az OpenAI biztosít, és amely lehetővé teszi a fejlesztők számára a GPT modell saját alkalmazásaikban történő használatát. Az API kezeli a szöveggenerálásra vonatkozó kéréseket, és visszaadja a generált szöveget az alkalmazásban történő felhasználásra.

# A ChatGPT használata programozóként

1. Automatizálás: Szoftvermérnökként a GPT API-t számos olyan feladat automatizálására használhatja, amely természetes nyelvmegértést és generálást igényel. Például használhatja ügyféltámogatási válaszok automatizálására, tartalom generálására vagy chatbotok fejlesztésére.
2. Kódolási segítség: A GPT használható a kódírás segítésére, a kód javításának javaslatára és a hibakeresésre. Megérti a kód kontextusát és értelmes javaslatokat tehet, ami potenciálisan csökkenti a fejlesztési időt és javítja a kód minőségét.
3. Személyre szabott felhasználói élmény: A GPT-t használhatja személyre szabott felhasználói élmények létrehozására alkalmazásaiban. Például használhatja személyre szabott válaszok, ajánlások vagy tartalom generálására a felhasználói bemenet alapján.
4. Adatelemzés: A GPT segíthet nagy mennyiségű szöveges adat elemzésében és megértésében. Használható kulcsinformációk kivonására, szövegek összefoglalására és minták, trendek azonosítására.
5. Gépi tanulás fejlesztés: A GPT használható nagyobb gépi tanulási rendszerek komponenseként. Finomhangolható specifikus feladatokra, vagy előre betanított modellként használható átviteli tanulási beállításokban.
6. Skálázhatóság: Az API-ként a GPT skálázásra tervezett. Ez azt jelenti, hogy használhatja nagy mennyiségű kérés kezelésére, ami alkalmassá teszi, hogy sok szoftver és app használja egyszerre.
7. Integráció: A GPT API könnyen integrálható meglévő rendszerekbe és szoftverekbe. Ez lehetővé teszi, hogy természetes nyelv megértési és generálási képességeket adjon hozzá alkalmazásaihoz anélkül, hogy ezeket a képességeket a nulláról kellene fejlesztenie.

Ezzel szemben egy "nem-programozó" felhasználó más módon használná ki a GPT előnyeit. Felhasználhatja e-mail írásához, tartalom generálásához vagy nyelvtanuláshoz, de nem tudná kihasználni az API teljes potenciálját úgy, ahogyan egy szoftvermérnök tudná.

---
---

## Státusz ellenőrzés - GPT API, azaz tudunk-e vele éppen dolgozni

Ezen az oldalon ellenőrizheted, hogy az API éppen működőképes-e:

```
https://status.openai.com/
```

---
---

# FONTOS!!!! - rate limit

Az OpenAI API (GPT API) rendelkezik több féle rate limittel. Ez azt jelenti, hogy szabályozva van a különböző prompt típusokra (pl.: text-davinci-003) leadható percenkénti hívások száma. Szabályozva van az is, hogy adott "token"-ből adott időtartam alatt mennyit lehet elhasználni. Lényeg a lényeg, hogy ha valakinek nem ad választ a hívása és már sokszor nyomkodta, akkor érdemes új API KEY-t generálni és azzal próbálkozni.

---
---

# Sentiment Analyser - Érzelem azonosító program

Az alkalmazás kér egy mondatot a felhasználótól, és megmutatja az arra vonatkozó érzelmi elemzés eredményét.

Szükséges lépések:
1. hozz létre egy felhasználót az openai rendszerében: (ez ingyenes)
    ```
    https://platform.openai.com/
    ```
2. bejelentkezés után hozz létre (és másold is ki a vágolapra azonnal) egy API KEY-t, amivel majd meg tudod hívni az API-t:
    ```
    https://platform.openai.com/account/api-keys
    ```
3. Nyisd meg a következő jsbin linket: https://jsbin.com/qehataz/2/edit?html,js,output

4. Cseréld ki a bemásolt kódban az API_KEY változó értékét a korábban létrehozott kulcsoddal
```js
const API_KEY = "IDE MÁSOD A KULCSOT!!!";
```

5. Futtasd a programot a Run with JS gombbal

