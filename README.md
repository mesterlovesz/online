# A Mesterlövész Újratöltve Online

**[Játék a böngészőben](https://mesterlovesz.online/)** · **[Letölthető változat és forráskód](https://github.com/mesterlovesz/remake)**

![Az eredeti játék főmenüje](https://mesterlovesz.online/assets/menu-preview.png)

Singleplayer kampány és közös pályák multiplayerben, karakterválasztással, fegyver- és lövésszinkronnal, valamint pályachattel. A kampányállapot és a mentések a játékos böngészőjében maradnak.

## Indítás

1. Nyisd meg a **mesterlovesz.online** oldalt friss asztali Chrome-ban vagy Edge-ben, bekapcsolt hardveres gyorsítással.
2. Kattints a **Játék előkészítése** gombra. Az első alkalommal a böngésző letölti és helyben előkészíti a játékadatokat. Saját magyar ISO-fájl és közvetlen ISO-URL is választható.
3. Válassz **Singleplayer** vagy **Multiplayer** módot. Multiban adj meg három betűt: a szerver három számjegyet rendel hozzá.
4. Később a **Korábbi játék indítása** gombbal folytathatod a helyben tárolt adatokból.

WASD: mozgás · egér: nézelődés · E: használat · Esc: menü · F11: teljes képernyő · K: karakterválasztás · M: többi játékos elrejtése · T: chat.

## Tárhely és frissítés

A webes kliens **GitHub Pagesen** fut. A meglévő Cloudflare-közvetítő kezeli a multiplayert és a chatet; a játékadatok külön tárhelyről érkeznek. ChatGPT Sites-fiók nem szükséges a weboldal frissítéséhez.

A `site.zip` a teljes, előre fordított webes kliens. A `.github/workflows/pages.yml` minden `main` ágra kerülő frissítésnél kicsomagolja és közzéteszi. A ZIP gyökerében az `index.html`, a JavaScript/CSS fájlok, az `assets/` és az `engine/` mappa található. Az ISO és a játékosok mentései nincsenek a tárolóban.

Motorfrissítéskor a WASM-részeket, a manifestet, a JavaScript-kötést és az összes `snippets/` modult együtt kell cserélni. Az `app.js` motorverzióját és az `index.html` scriptverzióját is frissíteni kell, hogy a gyorsítótár ne keverjen eltérő kiadásokat. A domain és a helyi adattárolás neve változatlan marad, ezért az átállás nem törli a meglévő mentéseket.

Ez a csomag tartalmazza a 2026-10-10-i statikus rabpozíció-javítást és a korábbi hibás pozíciót megőrző mentések kompatibilitási javítását, valamint a vendégneves pályachatet.

## Jogi megjegyzés

Nem hivatalos rajongói projekt. Az eredeti játék és minden eleme a jogtulajdonosokat illeti. Jogtulajdonosi kérésre eltávolítjuk az oldalt. Kapcsolat: **admin@mesterlovesz.online**.

Az egész projektet LLM-ek készítették; a projekt saját kódja emberi kódot nem tartalmaz.
