# Beyond Edits

Skill pro Claude Code, který edituje talking head videa v appce **Edits** od Instagramu přes její MCP.
Není to styl, je to postup: drží pořadí kroků a kontroly, které platí pro každé video. Titulky, barvy a písma si volíš sám.

## Co udělá

1. **Hrubý střih:** z přepisu vybere nejlepší pokusy a ukáže ti, co zůstává a co letí
2. **Pauzy:** stříhá podle skutečného ticha ve zvuku, ne podle titulků
3. **Titulky:** generuje je až po střihu a opraví chyby přepisu
4. **Obraz:** nic nezakrývá obličej, titulky pod bradou, hook nahoře čitelný na jakémkoli pozadí
5. **Hudba:** podkres, který nepřebíjí řeč, pokryje celé video a na konci dozní
6. **Zvuk:** změří a zvedne hlas, hudbu dá pod něj a přehráním ověří, že se nic nezkresluje
7. **Kontrola:** snímky z každé části videa, uložení projektu, export až na tvůj pokyn

## Instalace jedním promptem

Zkopíruj tohle do Claude Code:

```
Nainstaluj mi skill Beyond Edits. Spusť v terminálu `claude plugin marketplace add StepanKakes/beyond-edits` a pak `claude plugin install beyond-edits@beyond-edits`. Ověř to přes `claude plugin details beyond-edits@beyond-edits`, musí tam být skill edits. Pak zkontroluj, jestli mám připojené MCP z appky Edits (nástroje metapilot-native nebo server v `claude mcp list`). Když chybí, řekni mi, ať v Edits zkopíruju prompt pro připojení ke Claudovi a vložím ho sem. Nakonec mi řekni, ať restartuju Claude Code a pak napíšu /beyond-edits:edits.
```

## Instalace ručně

**1. Připoj Edits ke Claudovi.** V appce Edits zkopíruj prompt pro připojení ke Claudovi a vlož ho do Claude Code.

**2. Přidej skill.** V Claude Code napiš:

```
/plugin marketplace add StepanKakes/beyond-edits
```

```
/plugin install beyond-edits@beyond-edits
```

**3. Restartuj Claude Code.**

## Použití

Nahraj video do Media Panelu v Edits (Claude do tvých složek v Edits nevidí) a napiš:

```
/beyond-edits:edits
```

nebo normálně „střihni mi to v Edits, video jsem tam nahrál“.

## Aktualizace

`/plugin`, záložka Marketplaces, beyond-edits, Update, pak restart Claude Code.
