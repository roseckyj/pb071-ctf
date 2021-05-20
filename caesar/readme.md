# Ave Caesar, špatné zprávy

> "Ave Caesar, dorazil posel z Galie, prý je to naléhavé a přísně tajné!"
>
> "Sem s tím dopisem!"
>
> *Posel podáva Caesarovi dopis*
>
> "Podivné to psaní, takovýhle jazyk jsem ještě neviděl, ale předám to svým dvorním jazykovědcům a mistrům v šifrování, však oni si s tím budou vědět rady"
>
> "Nebo je dám předhodit lvům," dodal si pro sebe...

Pokud se nechcete stát lví pochoutkou, měli byste se dát hned do rozšifrovávání... ale kde začít?

Pokud jste nikdy neslyšeli o [Caesarově šifře](https://cs.wikipedia.org/wiki/Caesarova_%C5%A1ifra), pak se vám rychle pokusím shrnout, jak tato šifra funguje. Jedná se o jednoduchý posun znaků. Jedná-li se tedy o Caesarovu šifru s posunem o 3, šifrujeme zvednutím hodnoty znaku o 3 a odšifrováváme snížením hodnoty znaku o 3:

Šifra s posunem o 3:

`"Ahoj"` -- zašifrování (+3) --> `"Dkrm"` -- rozšifrování (-3) --> `"Ahoj"`

V našem případě neposouváme jen v rámci abecedy, ale v rámci celé tisknutelné části ASCII tabulky (tedy mezi znaky `32` (= mezera) a `126` (= vlnka) decimálně). Pokud bychom měli tedy šifrovat posunem o 1 znak `'~'`, dostáváme se zpět na znak `' '`.

Nepříjemné je, že nám posel neřekl, jak velkým posunem se autor při šifrování řídil. Nezbývá tedy, než vytáhnout hliněné destičky a použít hrubou sílu... A nezapomeňte, co hledáte!

Tik, tak... lvi už čekají

## Přílohy
[> dopis.txt](dopis.txt)