## Instalace

Pokud zatím nemáš nainstalovaný Python a Visual Studio Code, postupuj dle instrukcí z úvodního kurzu, konkrétně projdi tyto kapitoly:
* [Instalace jazyka Python](https://kodim.cz/programovani/uvod-do-progr-1/priprava/jazyky-nastroje/instalace-python)
* [Rozšíření VS Code pro Python](https://kodim.cz/programovani/uvod-do-progr-1/priprava/jazyky-nastroje/instalace-rozsireni-vscode)

## Instalace modulů

V rámci kurzu budeme používat modul pro práci s daty `pandas` a moduly pro tvorbu grafů `matplotlib` a `seaborn`. `pandas`, `matplotlib` a `seaborn` jsou externí moduly, které musíme nejdříve nainstalovat.

Spusťte Visual Studio Code a otevřete si nový terminál (z horní lišty vyberte **Terminal → New Terminal**).

### Windows
Napište **postupně** následující příkazy a po každém z nich stiskni **Enter**:

```shell
pip install pandas
pip install matplotlib
pip install seaborn
```

### Mac OS, Linux
Napište **postupně** následující příkazy a po každém z nich stiskni **Enter**:

```shell
pip3 install pandas
pip3 install matplotlib
pip3 install seaborn
```

`pandas` je relativně veliký modul, který obsahuje mnoho dalších modulů, takže instalace bude nějakou chvíli trvat. Terminál během instalace vypíše spoustu textu. Někde na konci bychom pak měli vidět text podobný tomuto:

```shell
Successfully installed pandas-2.1.4
```

Čísla verzí se mohou lišit, záleží na tom, jaká verze je právě aktuální.

## Ověření instalace

Instalaci si můžeš **ověřit** tím, že zkusíš moduly `pandas`, `seaborn` a `matplotlib` importovat. Otevři Python terminál (**Terminal → New Terminal** a pak příkaz `python` ve Windows a `python3` v Linuxu nebo MacOS), napiš `import pandas` a stiskni Enter. V ideálním případě Python nevypíše nic. To znamená, že modul importoval a můžeš ho začít používat.

Pokud Python reaguje chybou `ModuleNotFoundError` (viz níže), pak se instalace nepodařila.

```
>>> import pandas
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ModuleNotFoundError: No module named 'pandas'
```

Následně pomocí `import matplotlib` vyzkoušej, zda se úspěšně nainstaloval i modul `matplotlib` a pomocí `import seaborn` instalaci modulu `seaborn`.
