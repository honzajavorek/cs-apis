# Jak přidávat a upravovat zápisy v `cs-apis`?

Zápisy jsou zapisovány ve formátu [YAML](https://cs.wikipedia.org/wiki/YAML)
a měly by vypadat takto:

```yaml
name: Fio banka: API Bankovnictví
description: API Bankovnictví umožňuje bezpečné automatizované zpracování výpisů a pohybů na účtech vedených u Fio banky. Se službou API bankovnictví získáte okamžitý přehled o dění na Vašich účtech, aniž byste se museli přihlašovat do Vašeho internetového bankovnictví.
url: http://www.fio.cz/bankovni-sluzby/api-bankovnictvi
technologies: [XML, MT940, OFX, GPC, CSV, JSON, HTML, PDF, ABO]
free: yes
paid: no
official: yes
keywords: [banka, fio, bankovnictví, výpis, účet]
```

Pro název souboru používejte `nejaky-vystizny-nazev.yaml`.

## Co znamenají jednotlivé položky?

- **name** - Název API.
- **description** - Popis toho, co je to za API a co nabízí.
- **url** - Odkaz na dokumentaci k API.
- **technologies** - Seznam použitých technologií.
- **free** - Zda lze z API využít nějaká data i zadarmo.
- **paid** - Zda je celé API zpoplatněno (nebo nějaká jeho část).
- **official** - Zda se jedná o oficiální API, nebo je to nezávislá iniciativa,
  která ve skutečnosti není vlastníkem autorských práv na poskytovaná data.
- **keywords** - Klíčová slova. Važte je tak, aby šlo API nějak hezky vyhledat.

## Proč je zápis v takovém formátu? Proč jsou názvy položek anglicky?

Protože je díky tomu snadněji zpracovatelný strojem a celé `cs-apis` pak
lze použít jako jedno velké API.

## Ale proč je to zrovna YAML?

Protože cílem je ručně zapisovat několik *klíč-hodnota* údajů
ve strojově čitelné formě a nezbláznit se při tom. Psát ručně XML, HTML
nebo JSON je příliš velká otrava na to, jak jednoduchá data zápis obsahuje
a navíc je problém je zapisovat bezchybně.
