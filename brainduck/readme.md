# What does the duck say?

> Už nějakou dobu pozoruji, že se na místě, kde chodím krmit kachny děje něco divného. Většina kachen se hned rozběhne s vidinou plného žaludku ke mě. Ale skupinka několika kačerů mě úplně ignoruje. Stojí v kroužku, jako při nějakém podivném rituálu a vydávají si ty své nesrozumitelné zvuky. Dneska už moje zvědavost přerostla únosnou hranici a rozhodl jsem se, že tomu přijdu na kloub. Pořídil jsem nahrávku, kterou jsem doma poctivě přepsal a myslím, že už jsem na to přišel!

Kachní zpráva je ve skutečnosti program v jazyce [Brainf*ck](https://cs.wikipedia.org/wiki/Brainfuck). Pokud jste o něm nikdy neslyšeli, tak nezoufejte, je skutečně jednoduchý. Pro naše účely jsem kachní modifikaci nazval Brainduck.

Paměť Brainduckového stroje je jednosměrně "nekonečná" (pro naše účely stačí 1000 buněk) páska, kde na každý znak můžeme uložit nezáporné číslo 0-255 (`unsigned char`).

Brainf*ck používá pro programování jen 8 různých znaků, které si ale naše kachny trochu upravily... jejich zobáky hold nezvládnou vydat zvuk `[`, nebo `+`
- `A` (= `>`) - posun datového ukazatele o jednu buňku doprava
- `a` (= `<`) - posun datového ukazatele o jednu buňku doleva
- `R` (= `+`) - zvýšení hodnoty aktivní buňky o 1 (buňky, nad kterou je ukazatel), neřešte přetečení, it's not a bug, it's a feature
- `r` (= `-`) - snížení hodnoty aktivní buňky o 1, neřešte podtečení, also a feature
- `W` (= `.`) - výpis hodnoty aktivní buňky na standardní výstup. Pro výpis se používá ASCII znak podle hodnoty aktivní buňky
- `w` (= `,`) - uložení hodnoty ze vstupu do aktivní buňky (ASCII)
- `G` (= `[`) - pokud je hodnota aktivní buňky rovna nule, provede přesun instrukčního ukazatele doprava za nejbližší `g`(= `]`)
- `g` (= `]`) - pokud je hodnota aktivní buňky různá od nuly, provede přesun instrukčního ukazatele doleva na nejbližší `G`(= `[`)

Stačí už jen poslední krok k odhalení kachní záhady!

*Pozn.: Pro tuto úlohu je zakázáno použít jakýkoli interpreter Brainf\*cku, který si sami nenapíšete*

## Přílohy
[> prepis.bd](prepis.bd)
