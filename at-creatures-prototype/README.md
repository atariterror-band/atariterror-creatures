# AT Creatures — funkční prototyp

Samostatný front-endový prototyp fanouškovské aplikace Atari Terror ve vizuálním směru Industrial. Otevřete `index.html` v prohlížeči nebo spusťte lokální statický server v této složce.

## Co funguje

- Výběr až pěti skladeb nebo přeskočení výběru.
- Úvodní obrazovka s proměnlivými ručně kreslenými tvářemi na texturovaném kobaltově modrém pozadí; po omezení pohybu v systému zůstane animace vypnutá.
- Katalog 26 skladeb z alb Part 3: Final Warning a Part2: Attention!, s přímými odkazy na konkrétní skladby na Spotify. Tlačítko „Skladbu ještě neznám, pusť mi“ otevře náhodnou skladbu katalogu na Spotify.
- Každá skladba má interpretační profil v `song-profiles.js`, včetně odkazu na zdroj a údaje, zda byl její text dostupný. Dostupné texty jsou převedené do původních stručných interpretací, nikoli ukládané doslova. Nedostupné texty mají hypotetický motiv odvozený z názvu. Výběr ovlivňuje archetyp, popis, barvu a kreslené motivy výsledné bytosti.
- Volba podoby, věkové kategorie a osobnostního ladění.
- Lokální generování názvu, frakce, popisu a vzhledu bytosti; výsledek lze znovu vygenerovat.
- Výsledné bytosti a karty mají vlastní vektorovou ilustraci v syrovém, ručně kresleném fanzinovém duchu. Galerie používá jen artwork bytostí, bez portrétních fotografií.
- Galerie uložených obrázků obsahující výhradně karty; galerie umožňuje kartu stáhnout nebo odebrat.
- Veřejná ukázková galerie pod úvodní obrazovkou. Zobrazuje čtyři demo karty a karty uložené v tomto prohlížeči; kliknutím se karta zvětší.
- Stažení karty a znaku jako SVG, s odkazy na vybrané skladby přímo v kartě. Výsledek lze připravit jako PNG pro Instagram (feed 4:5, příběh 9:16, čtverec) nebo Facebook (příspěvek 1,91:1, příběh 9:16, čtverec). Součástí sdílení je popisek s odkazy na zvolené skladby, aplikaci a oficiální profil kapely podle vybrané sítě.
- Ve sdílecím dialogu lze dopsat vlastní text, který se zobrazí na obrázku i v připraveném popisku. Patička odkazuje na náhled kapelního dashboardu v `dashboard.html`; přihlašovací pole jsou prázdná, přihlášení není aktivní a náhled lze otevřít bez něj.
- Prototyp lokálně zaznamenává začátek tvorby, dokončení bytosti, výběry skladeb, odchozí kliknutí na Spotify a fanouškem potvrzená sdílení rozdělená podle sítě. Dashboard tyto události zobrazuje pouze z aktuálního prohlížeče.
- Výtvarná bible světa je v `ATARI_TERROR_WORLD.md`.
- Odkaz na existující náhled AT Shopu.
- Responzivní zobrazení pro mobil i desktop.

## Záměrná omezení prototypu

- Sdílecí obrázek obsahuje viditelné adresy profilů a názvy zvolených skladeb; klikací odkazy jsou dostupné v digitální SVG kartě a v připraveném popisku. Samotný PNG obrázek sociální sítě klikací odkazy nepřenáší.
- Generování probíhá lokálně v prohlížeči. Aplikace neposílá volby ani osobní údaje na server.
- Lokální měření není společná analytika; kliknutí na Spotify nepotvrzuje přehrání skladby. Sdílení podle sítě jsou potvrzení fanouška, protože aplikace bez propojení s účty sociálních sítí nemůže ověřit zveřejněný příspěvek.
- Galerie ukládá karty do místního úložiště prohlížeče; zobrazí je pouze na zařízení a v profilu daného prohlížeče.
- Veřejné karty napříč návštěvníky vyžadují serverovou databázi a výslovný souhlas autorů. V tomto prototypu jsou čtyři ukázkové karty a lokálně uložené karty.
- Plakát je náhled a koncertní QR karta je dekorativní ukázka, nikoli platná vstupenka či slevový kód.
- Pro ostrý provoz bude potřeba doplnit katalog a ověřit práva k motivům, produkční generování/tisk, objednávky, platby a případné skutečné QR kódy.
