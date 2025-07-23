# Level 2: Intermediate - Pokročilé funkce

## 📋 Obsah

- [Cíle tohoto levelu](#cíle-tohoto-levelu)
- [Model Selection: Který AI model použít?](#model-selection-který-ai-model-použít)
- [MCPs: Rozšíření schopností Cursoru](#mcps-rozšíření-schopností-cursoru)
- [📂 Git integrace: Verzování pro každého](#-git-integrace-verzování-pro-každého)
- [⚙️ Cursor Rules: Natrénujte si Cursor na míru](#️-cursor-rules-natrénujte-si-cursor-na-míru)
- [Praktická cvičení](#praktická-cvičení)
- [Checkpoint: Jste připraveni na Level 3?](#checkpoint-jste-připraveni-na-level-3)
- [Pro Tips pro Level 2](#pro-tips-pro-level-2)
- [Co dál?](#co-dál)

## Cíle tohoto levelu
- Vybrat **správný AI model** pro různé úkoly
- Nainstalovat a používat **MCPs** pro rozšíření funkcí
- Využít **Git integraci** pro verzování dokumentů
- Vytvořit **Cursor Rules** pro konzistentní výsledky

## Model Selection: Který AI model použít?

### Proč je důležité vybrat správný model?
Cursor podporuje různé AI modely, každý má své silné stránky. **Správná volba = lepší výsledky!**

### Jak změnit model:
1. **Ctrl+Shift+P** (Command Palette)
2. Napište "model" 
3. Vyberte "Cursor: Select Model"
4. Zvolte model podle úkolu

### Přehled modelů pro non-tech uživatele (2025):

#### **Claude Sonnet 4** - Nejlepší pro kód a business
- **Nejlepší pro**: Komplexní dokumenty, kód, analýzy, dlouhé texty
- **Výhody**: State-of-the-art přesnost, vynikající čeština, konzistentní
- **Nevýhody**: Dražší než základní modely
- **Použijte pro**: Kontrakty, technické dokumenty, složité analýzy

#### **GPT-4.1** - Rychlý univerzální model
- **Nejlepší pro**: Obecné úkoly, brainstorming, rychlé odpovědi
- **Výhody**: 50% rychlejší než GPT-4, 83% levnější, dobrý kontext
- **Nevýhody**: Méně přesný než Claude pro složité úkoly
- **Použijte pro**: Poznámky ze schůzí, e-maily, nápady, prezentace

#### **OpenAI o3-Pro** - Premium reasoning model  
- **Nejlepší pro**: Složité logické úlohy, analýzy, problem solving
- **Výhody**: Nejlepší reasoning schopnosti, deep thinking
- **Nevýhody**: Nejdražší, pomalejší
- **Používejte pro**: Strategické plánování, složité obchodní rozhodování

#### **Gemini 2.5 Pro** - Google's flagship
- **Nejlepší pro**: Multimodální úkoly, dlouhé kontexty
- **Výhody**: Výborný s obrázky a dokumenty, velký kontext
- **Nevýhody**: Méně populární, horší čeština
- **Používejte pro**: Analýza PDF s obrázky, multimodální obsah

### Praktické doporučení:

| Úkol | Doporučený model | Proč |
|------|------------------|------|
| **Brainstorming nápadů** | GPT-4.1 | Rychlý a kreativní |
| **Formální dokumenty** | Claude Sonnet 4 | Nejpřesnější a nejkonzistentnější |
| **Rychlé úpravy textu** | GPT-4.1 | Rychlý a levný |
| **Analýza dat/textů** | Claude Sonnet 4 | State-of-the-art analytical schopnosti |
| **Kreativní psaní** | GPT-4.1 | Nápadité a flexibilní |
| **Technické texty** | Claude Sonnet 4 | Nejlepší pro složité dokumenty |
| **Strategické plánování** | OpenAI o3-Pro | Nejlepší reasoning pro složité rozhodnutí |
| **Multimodální obsah** | Gemini 2.5 Pro | Výborný s obrázky a PDF dokumenty |

## MCPs: Rozšíření schopností Cursoru

### Co jsou MCPs a proč je potřebujete?
MCPs (Model Context Protocols) = **rozšíření**, která řeší kritická omezení Cursoru. **Cursor nativně nemůže číst PDFs, analyzovat Excel soubory, nebo se připojit k externím službám. MCPs tyto mezery vyplňují.**

### Proč MCPs nejsou "advanced" ale essential:

#### **Bez MCPs**:
```
Vy: "Vytvoř mi graf z těchto sales dat"
Cursor: "Můžu ti napsat text o datech, ale graf neumím vytvořit"
Limitation: Jen text processing
```

#### **S MCPs**:
```
Vy: "Vytvoř mi graf z těchto sales dat"  
Cursor: "Vytvořil jsem sloupcový graf a uložil jako chart.png"
Result: Skutečná business value
```

### cursor.directory - Jednoduchá instalace

**Instalace MCP za 2 minuty:**
1. Jděte na [cursor.directory](https://cursor.directory)
2. Najděte rozšíření (např. "CSV Analyzer")
3. Zkopírujte instalační kód
4. V Cursoru: `Ctrl+Shift+P` → "Cursor Settings"
5. Přidejte do MCP servers sekce
6. Restartujte Cursor

### Top Business MCPs (based on 2025 usage data):

#### **1. Excel MCP** - Universal Business Need
**Link**: [Excel MCP Server](https://github.com/haris-musa/excel-mcp-server) | [Excel Data Manager](https://playbooks.com/mcp/excel-data-manager)

**Proč Excel MCP**: Každá firma pracuje se spreadsheets - okamžitá business hodnota

Co umí Excel MCP:
- "Analyzuj data v tomto souboru a najdi trendy"
- "Vytvoř summary z této Excel tabulky"
- "Porovnej výkon mezi Q1 a Q2 podle dat"
- "Generuj report z těchto sales čísel"

**Installation**: 1 minuta (npx command)  
**Cost**: Zdarma  
**Business impact**: Automatizace reportingu a data analýzy

#### **2. Notion MCP** - Knowledge Management Powerhouse
**Link**: [Notion Official MCP](https://developers.notion.com/docs/mcp) | [Notion MCP Directory](https://cursor.directory/mcp/notion-6)

**Proč Notion MCP**: Většina firem používá Notion pro dokumentaci a project management

Co umí Notion MCP:
- "Vytvoř project page z těchto requirements"
- "Najdi všechny task related k projektu ABC"
- "Update status všech úkolů na dokončeno"
- "Shrni poznámky z posledních 5 meetingů"

**Installation**: 2 minuty (OAuth setup)  
**Cost**: Zdarma s Notion účtem  
**Business impact**: Přímá integrace s firemní knowledge base

#### **3. Google Drive & Sheets MCP** - Cloud Storage Integration
**Link**: [Google Drive MCP](https://cursor.directory/mcp/google-drive) | [Google Workspace MCP](https://cursor.directory/mcp/google-workspace)

**Proč Google Drive MCP**: Univerzální cloud storage

Use cases:
- "Analyzuj data z tohoto Google Sheets"
- "Najdi prezentaci z minulého meetingu v Drive"
- "Vytvoř summary z Docs dokumentu"

**Installation**: 3 minuty (potřeba Google OAuth)  
**Cost**: Zdarma  
**Business impact**: Přímý přístup k cloud datům


### Rychlá instalace - Krok za krokem

#### **1. Excel MCP** (nejužitečnější start!):
**Návod**: [Excel MCP Server](https://github.com/haris-musa/excel-mcp-server)
```json
// V ~/.cursor/mcp.json přidejte:
{
  "excel": {
    "command": "npx",
    "args": ["-y", "excel-mcp-server"]
  }
}
```

**Test**: Otevřete Excel soubor → "Analyzuj data v tomto souboru" → Instant insights!

#### **2. Notion MCP** (pro knowledge management):
**Návod**: [Notion Official MCP](https://developers.notion.com/docs/mcp)
```json
{
  "notion": {
    "command": "npx",
    "args": ["-y", "@notion/mcp-server"]
  }
}
```

**Setup**: OAuth s vaším Notion workspace (2 minuty setup)

#### **3. Google Drive MCP** (pro cloud access):
**Návod**: [Google Drive Setup](https://cursor.directory/mcp/google-drive)
```json
{
  "google-drive": {
    "command": "npx",
    "args": ["@isaacphi/mcp-gdrive"],
    "env": {
      "GOOGLE_CREDENTIALS_PATH": "/path/to/credentials.json"
    }
  }
}
```

**Test**: "Najdi všechny dokumenty related k projektu ABC v Drive"

### MCP Best Practices:

#### **Začněte jednoduše** (podle business hodnoty):
1. **Excel MCP** - univerzální potřeba, každý pracuje se spreadsheets
2. **Notion MCP** - pokud používáte Notion pro dokumentaci/projekty
3. **Google Drive MCP** - cloud storage integrace
4. **Specialized MCPs** - podle specifických potřeb týmu

#### **Postupné rozšiřování**:
- Týden 1: Excel MCP + data analysis workflows
- Týden 2: Notion MCP + knowledge management integration  
- Týden 3: Google Drive MCP + cloud access
- Týden 4: Domain-specific MCPs podle potřeby

#### **Užitečné odkazy**:
- **[cursor.directory](https://cursor.directory/mcp)** - hlavní katalog MCPs
- **[Awesome MCP Servers](https://mcpservers.org/)** - komunitní seznam
- **[@Cursor Documentation](https://docs.cursor.com/context/mcp)** - oficiální MCP dokumentace

#### ❌ **Nedělejte**:
- Neinstalujte 10 MCPs najednou
- Neskočte rovnou na komplexní MCPs
- Netestujte na production datech hned

## 📂 Git integrace: Verzování pro každého

### Co je Git a proč vám pomůže?
Git = systém pro sledování změn v souborech. **Představte si to jako "Track Changes" ve Wordu, ale mnohem mocnější.**

### 🎯 Základní Git workflow v Cursoru:

#### 1. **Zobrazení změn**
- **Ctrl+Shift+G**: Otevře Git panel
- Uvidíte všechny změněné soubory
- Kliknutím se podíváte co se změnilo

#### 2. **Uložení změn (Commit)**
- V Git panelu napište popis změny
- Příklad: "Přidané poznámky z meetingu 25.1."
- **Ctrl+Enter**: Uloží změny

#### 3. **AI pomoc s commit messages**
Cursor automaticky navrhne popis změn:
- Otevře Git panel
- AI automaticky vyplní rozumný popis
- Můžete upravit nebo použít jak je

### 💼 Praktické situace pro Git:

#### **Scenář 1: Týmová práce na dokumentu**
```
1. Petr vytvoří draft prezentace
2. Commit: "Vytvořena struktura prezentace Q1"
3. Jana přidá data a grafy  
4. Commit: "Přidána data a vizualizace"
5. Milan upraví závěr
6. Commit: "Aktualizace závěru a doporučení"
```

#### **Scenář 2: Verzování důležitých dokumentů**
```
- Smlouva v1: Původní návrh
- Smlouva v2: Připomínky právníka
- Smlouva v3: Finální verze po jednání
```

### 🎯 AI-powered Git funkce:

#### **Automatické commit messages**
- Cursor vidí co jste změnili
- Automaticky navrhne popis
- Příklad: "Updated meeting notes with action items and deadlines"

#### **Conflict resolution**  
- Pokud dva lidé upravují stejný soubor
- Cursor pomůže vyřešit konflikty
- AI navrhne nejlepší kombinaci změn

## ⚙️ Cursor Rules: Natrénujte si Cursor na míru

### Co jsou Cursor Rules?
Soubor instrukcí, které říkají Cursoru **jak má pracovat s vašimi dokumenty**. Jako byste měli osobního asistenta s jasnými pokyny.

### 🎯 Jak vytvořit Rules:
1. **Vytvořte soubor** `.cursorrules` v root složce
2. **Napište pravidla** v obyčejném textu
3. **Cursor je automaticky použije** ve všech dokumentech

### 💼 Příklady Rules pro business použití:

#### **Firemní komunikační styl:**
```
# Firemní komunikační pravidla

## Tón a styl:
- Používej profesionální ale přátelský tón
- Vždy používej "Vy" místo "ty" v oficiální komunikaci
- Začínej e-maily "Dobrý den" a končíj "S pozdravem"

## Formátování:
- Důležité informace dej do **tučného písma**
- Seznamy formátuj jako bullet points
- Přidávej číslování k action items

## Obsah:
- Vždy přidej konkrétní termíny k úkolům
- Jmenuj odpovědné osoby
- Přidej kontaktní informace když je třeba
```

#### **Prezentační standardy:**
```
# Pravidla pro prezentace

## Struktura:
- Začni vždy s agenda slide
- Každá sekce má max 3 klíčové body
- Končíme s "Next Steps" slide

## Styl:
- Používej aktivní místo pasivní formulations
- Čísla vždy podpoř kontextem (vs. plán, vs. předchozí období)
- Každé tvrzení podpoř příkladem

## Format:
- Nadpisy maximálně 8 slov
- Body textu max 2 řádky
- Vždy přidej slide number
```

#### **Meeting notes standardy:**
```
# Standardy pro meeting notes

## Povinné sekce:
- Datum, čas, účastníci
- Agenda/cíle meetingu  
- Klíčové rozhodnutí
- Action items s odpovědnými osobami a termíny
- Next steps

## Formátování action items:
- [ ] **ÚKol** - Odpovědná osoba - Termín - Priority (High/Medium/Low)

## Follow-up:
- Vždy přidej kdy je naplánován další meeting
- Zmíň co bude potřeba připravit
```

### 🎯 Pokročilé Rules techniky:

#### **Podmíněné pravidla:**
```
# Pokud pracuješ s dokumenty obsahujícími "marketing":
- Používej persuasivní jazyk
- Přidávej call-to-action
- Zmiň benefity pro zákazníka

# Pokud pracuješ s "financial" dokumenty:
- Buď konzervativní a přesný
- Všechna čísla podpoř zdroji
- Používej formální jazyk
```

## Praktická cvičení

### Cvičení 1: Excel MCP - Immediate Business Value
**Úkol**: Nainstalovat Excel MCP a vidět data analysis magic v akci

#### Krok 1: Rychlá instalace (1 minuta)
1. **Otevřete Cursor Settings** (`Cmd/Ctrl + ,`)
2. **Jděte na MCP sekci** (nebo vytvořte soubor `~/.cursor/mcp.json`)
3. **Přidejte tento kód**:
```json
{
  "excel": {
    "command": "npx",
    "args": ["-y", "excel-mcp-server"]
  }
}
```
4. **Restart Cursoru** - Done! ✅

#### Krok 2: Příprava testovacích dat (2 minuty)
Vytvořte jednoduchý Excel soubor nebo použijte existující s těmito daty:
```
Month    | Revenue | Customers | Churn Rate
January  | 45000   | 120       | 2.5%
February | 52000   | 135       | 1.8%
March    | 48000   | 128       | 3.2%
April    | 61000   | 156       | 2.1%
```

#### Krok 3: Test s real business queries (2 minuty)
**Data Analysis:**
- Command+L: "Analyzuj trendy v tomto Excel souboru"
- Command+L: "Který měsíc měl nejlepší performance a proč?"
- Command+L: "Vytvoř executive summary těchto čísel"

**Business Insights:**
- Command+L: "Jaký je průměrný growth rate mezi měsíci?"
- Command+L: "Identifikuj risk factors na základě těchto dat"
- Command+L: "Navrhni action items pro zlepšení churn rate"

**Proč Excel MCP?**
- **Universal business need** - každá firma má Excel data!
- **Immediate ROI** - z hodin analýzy → minuty insights
- **Real data, real value** - pracuje s vašimi skutečnými čísly
- **Scalable** - funguje s malými i velkými datasety

**Výsledek**: Místo manuální Excel analýzy → AI-powered business intelligence!

### Cvičení 2: Model Selection Master  
**Úkol**: Porovnání modelů na stejném úkolu

1. **Kreativní brainstorming** (použijte GPT-4.1):
   - Vytvořte soubor `ideas.md`
   - Command+L: "Vymysli 10 kreativních nápadů na team building event"

2. **Formální dopis** (použijte Claude Sonnet 4):
   - Vytvořte soubor `formal-letter.md`  
   - Command+L: "Napiš formální stížnost na dodavatele kvůli pozdnímu dodání"

3. **Rychlá úprava** (použijte GPT-4.1):
   - Vezměte jakýkoliv text
   - Command+K: "udělej z tohoto bullet points"

**Porovnejte výsledky** - všimnete si rozdílů?

### Cvičení 3: Git workflow pro dokumenty
1. **Vytvořte nový dokument** `team-handbook.md`
2. **Napište základní obsah** (třeba pravidla pro komunikaci)
3. **Commit**: "Initial team handbook structure"
4. **Přidejte novou sekci** (např. o remote work)
5. **Commit**: "Added remote work guidelines"  
6. **V Git panelu** si prohlédněte historii změn

### Cvičení 4: Vytvoření vlastních Rules
1. **Vytvořte soubor** `.cursorrules` ve vaší složce
2. **Napište pravidla** pro váš firemní styl:
```
# Moje firemní pravidla

Při psaní jakýchkoliv dokumentů:
- Používej náš firemní tón (profesionální ale přátelský)
- Vždy přidej datum a autora na začátek
- Action items formátuj jako checklist s termíny
- Čísla vždy uváděj s kontextem
```
3. **Otestujte Rules**: Vytvořte nový dokument a použijte Command+L na nějaký úkol
4. **Všimnite si** jak Cursor aplikuje vaše pravidla

### Cvičení 5: Kombinace všech funkcí
**Reálný scénář**: Připravte prezentaci pro vedení

1. **Nastavte Claude Sonnet 4** (pro nejlepší business kvalitu)
2. **Vytvořte Rules** pro prezentace (viz příklad výše)
3. **Vytvořte soubor** `q1-review.md`
4. **Command+L**: "Vytvoř strukturu prezentace o Q1 výsledcích pro management"
5. **Postupně rozvíjejte** každou sekci pomocí Command+K
6. **Commitujte změny** po každé významné úpravě
7. **Na závěr porovnejte** jak Rules ovlivnily finální výsledek

## Checkpoint: Jste připraveni na Level 3?

Před přechodem na Level 3 zvládnete:
- [ ] **Vybrat správný model** podle typu úkolu
- [ ] **Nainstalovat a používat** základní MCPs (PDF Reader, CSV Analyzer)
- [ ] **Používat Git** pro verzování dokumentů
- [ ] **Vytvořit basic Rules** pro svůj workflow
- [ ] **Kombinovat všechny funkce** pro reálné úkoly

### Pokročilý test:
Dokážete během 10 minut:
1. Vybrat vhodný model pro task
2. Vytvořit dokument s použitím vlastních Rules
3. Udělat smysluplný commit s AI pomocí
4. Vysvětlit proč jste vybrali právě tento model

## Pro Tips pro Level 2:

### Model Selection hacks:
- **GPT-4.1** když potřebujete kreativitu a rychlost
- **Claude Sonnet 4** když potřebujete nejvyšší přesnost a kvalitu  
- **Experimentujte** - stejný prompt, různé modely = různé výsledky

### Git best practices:
- **Commitujte často** s popisnými zprávami
- **Používejte AI commit messages** ale upravte je podle potřeby
- **Git není jen pro programátory** - funguje skvěle pro dokumenty!

### Rules optimization:
- **Začněte jednoduše** - přidávejte Rules postupně
- **Testujte Rules** na různých dokumentech
- **Updatujte Rules** když objevíte co funguje lépe

## Co dál?
Pokud máte všechny checkpointy splněné, přejděte na **Level 3: Advanced** kde objevíte MCPs, add-ins a další rozšíření, která z Cursoru udělají skutečně mocný nástroj pro vaši práci.