webovka pro mobilní zařízení 

Naprogramoval jsem jednoduchou testovací webovou stránku pro obchod s oblečením. Použil jsem HTML a CSS pro vytvoření rozvržení a stylu. Cílem bylo zobrazit kolekci triček ve formě gridového katalogu, který je zároveň responzivní – tedy přizpůsobí se velikosti obrazovky.
V hlavní části jsem vytvořil mřížku pomocí CSS Grid, kde jednotlivé položky (produkty) mají vlastní třídy jako clothing-column1, clothing-column2 atd. Každý z těchto boxů obsahuje obrázek trička, jeho název a cenu. Zatím jsou všechny položky stejné – tričko za 10 dolarů – protože jde o testovací data.
Na vrchu stránky je navigační lišta s logem a odkazy jako Home, About, Services, Contact a Cart. Pro mobilní zařízení jsem připravil jednoduchou verzi menu, které se schová pod ikonku – to budu později doplňovat JavaScriptem.
Stylování jsem si pohrál přes @media queries, takže při různých šířkách obrazovky se obsah automaticky přeuspořádá. Například na mobilu se zobrazují produkty jeden pod druhým, na tabletu dva vedle sebe a na desktopu třeba čtyři vedle sebe. Díky tomu je stránka přehledná a použitelná i na telefonech.
Design jsem ladil pomocí box-shadow, zarovnání a paddingu, aby každý produkt vypadal jako malá karta, která po najetí myší trochu reaguje – posune se nebo změní okraj. Je to jednoduché, ale funkční.
HTML struktura je jasná – mám kontejner .container, který obsahuje navigaci, hlavní text (<main>) a všechny produkty jako jednotlivé divy. Do JavaScriptu se zatím nepouštím, ale v budoucnu tam chci přidat např. filtrování podle kategorií nebo funkční košík.
link:https://youtu.be/YkCr7yPfAwg



















