# 📂 Git pro dokumenty - Praktický průvodce

Git není jen pro programátory! Zde se naučíte používat Git v Cursoru pro verzování dokumentů, prezentací a jakýchkoli textových souborů.

## 📋 Obsah

- [🤔 Proč Git pro dokumenty?](#-proč-git-pro-dokumenty)
- [🎯 Git základy v Cursoru](#-git-základy-v-cursoru)
- [📝 Praktické scénáře](#-praktické-scénáře)
- [🛠️ Pokročilé Git funkce v Cursoru](#️-pokročilé-git-funkce-v-cursoru)
- [📋 Cvičení - Git v praxi](#-cvičení---git-v-praxi)
- [💡 Best Practices pro Git + dokumenty](#-best-practices-pro-git--dokumenty)
- [🎯 Pokročilé tipy](#-pokročilé-tipy)

## 🤔 Proč Git pro dokumenty?

### Bez Gitu:
```
📁 Moje dokumenty
├── prezentace_final.pptx
├── prezentace_final_v2.pptx  
├── prezentace_final_FINAL.pptx
├── prezentace_final_po_pripominkach.pptx
├── prezentace_skutecne_final.pptx
└── prezentace_tuhle_uz_nemazat.pptx
```

### S Gitem:
```
📁 Moje dokumenty
├── prezentace.md
└── .git/ (neviditelná složka s historií všech verzí)
```

**Výsledek**: Jeden soubor, kompletní historie změn, možnost vrátit se k jakékoliv verzi!

## 🎯 Git základy v Cursoru

### 1. **Otevření Git panelu**
- **Ctrl+Shift+G** (Windows/Linux)
- **Cmd+Shift+G** (Mac)
- Nebo klikněte na Git ikonu v sidebaru

### 2. **Chápání Git stavů**
Soubory mohou být ve 3 stavech:

#### 🔴 **Modified (Změněno)**
- Soubor jste upravili, ale neuložili do historie
- Zobrazuje se v "Changes" sekci
- Cursor ukáže, co přesně se změnilo

#### 🟡 **Staged (Připraveno)**
- Soubor je připravený k uložení do historie
- Kliknete na "+" u souboru
- Zobrazuje se v "Staged Changes"

#### 🟢 **Committed (Uloženo)**
- Soubor je uložen do historie s popisem
- Napíšete popis a kliknete "Commit"
- Je součástí permanentní historie

### 3. **Základní Git workflow**
```
1. Upravte dokument → 🔴 Modified
2. Klikněte "+" → 🟡 Staged  
3. Napište popis → 🟢 Committed
```

## 📝 Praktické scénáře

### Scénář 1: Týmová práce na dokumentu

#### **Situace**: 
Tým pracuje na strategickém plánu. Každý přidává svou část.

#### **Git workflow**:
```
1. Jana vytvoří základní strukturu
   Commit: "📋 Vytvořena základní struktura plánu"

2. Petr přidá market analýzu  
   Commit: "📊 Přidána analýza trhu a konkurence"

3. Milan upraví finanční projekce
   Commit: "💰 Aktualizované finanční projekce na Q2-Q4"

4. Sarah dopíše rizika a mitigation
   Commit: "⚠️ Přidána sekce rizik a jejich řešení"
```

#### **Výhody**:
- ✅ Vidíte kdo co změnil a kdy
- ✅ Můžete se vrátit k jakékoliv verzi
- ✅ Jasná historie development dokumentu

### Scénář 2: Verzování důležitých smluv

#### **Situace**:
Vyjednáváte smlouvu s klientem přes několik kol.

#### **Git workflow**:
```
Commit 1: "📄 Prvotní návrh smlouvy - základní podmínky"
Commit 2: "💼 Zapracované připomínky právníka - články 3,7,12"  
Commit 3: "🤝 Úpravy po jednání s klientem - cena a termíny"
Commit 4: "✅ Finální verze schválená oběma stranami"
```

#### **Výhody**:
- ✅ Kompletní audit trail vyjednávání
- ✅ Můžete porovnat verze
- ✅ Víte přesně co bylo kdy změněno

### Scénář 3: Iterativní vývoj prezentace

#### **Situace**:
Připravujete prezentaci, kterou budete postupně vylepšovat.

#### **Git workflow**:
```
Commit 1: "🎯 Základní outline prezentace"
Commit 2: "📊 Přidány grafy a data z Q1"
Commit 3: "🎨 Vylepšený design a flow"  
Commit 4: "💡 Přidané case studies a příklady"
Commit 5: "🔍 Review feedback zapracován"
```

## 🛠️ Pokročilé Git funkce v Cursoru

### **AI-Generated Commit Messages**
Cursor automaticky navrhne popis změn:

1. Udělejte změny v dokumentu
2. Otevřete Git panel
3. Cursor automaticky vyplní commit message
4. Můžete upravit nebo použít jak je

#### Příklady automatických zpráv:
- "Add quarterly financial projections to strategic plan"
- "Update client contact information in CRM template"  
- "Revise presentation conclusion with new recommendations"

### **Diff Viewer** 
Cursor ukáže přesně co se změnilo:

- **Zelená**: Přidaný text
- **Červená**: Odstraněný text
- **Modré**: Upravený text

### **Branch práce** (pokročilé)
Pro velké změny můžete vytvořit "branch":

1. Command Palette (`Ctrl+Shift+P`)
2. "Git: Create Branch"
3. Pojmenujte branch (např. "redesign-proposal")
4. Pracujte na změnách
5. Až budete hotovi, merge back

## 📋 Cvičení - Git v praxi

### Cvičení 1: Základní Git workflow

1. **Vytvořte nový dokument** `my-first-git-doc.md`
2. **Napište základní obsah**:
```markdown
# Můj první Git dokument

## Úvod
Toto je test Git funkcionality.

## Plány
- Naučit se Git
- Používat pro dokumenty
```

3. **Uložte soubor** (`Ctrl+S`)
4. **Otevřete Git panel** (`Ctrl+Shift+G`)
5. **Klikněte "+"** u souboru (stage)
6. **Napište commit message**: "📝 Vytvořen první Git dokument"
7. **Klikněte Commit**

### Cvičení 2: Sledování změn

1. **Upravte dokument** - přidejte novou sekci:
```markdown
## Co jsem se naučil
- Git není strašák
- Pomáhá organizovat práci
- Cursor to dělá snadné
```

2. **V Git panelu** si prohlédněte co se změnilo
3. **Stage a commit** s popisem: "➕ Přidána sekce s poznatky"

### Cvičení 3: AI commit messages

1. **Udělejte několik změn** najednou:
   - Přidejte odrážky
   - Upravte nadpisy  
   - Přidejte emoji

2. **V Git panelu** počkejte na AI návrh
3. **Upravte AI zprávu** podle potřeby
4. **Commitněte změny**

### Cvičení 4: Práce s historií

1. **Command Palette** (`Ctrl+Shift+P`)
2. **Napište "Git log"** - zobrazí historii
3. **Prohlédněte si** všechny vaše commits
4. **Kliknete na starší commit** - uvidíte jak dokument vypadal

## 💡 Best Practices pro Git + dokumenty

### ✅ Dobré commit zprávy:
- **Konkrétní**: "Přidána sekce o rozpočtu" místo "Změny"
- **Akční**: "Aktualizovat", "Přidat", "Opravit"
- **S emoji**: 📝 📊 💰 ✅ pro lepší orientaci
- **V českém jazyce**: Pokud pracujete česky

### ✅ Kdy commitovat:
- Po dokončení logické části práce
- Před velkými změnami
- Na konci pracovního dne
- Po zapracování feedback

### ✅ Co commitovat:
- Dokončené sekce dokumentů
- Finální verze po review
- Důležité milníky v práci
- Změny po připomínkách

### ❌ Co necommitovat:
- Poloviční myšlenky a nedokončené věty
- Osobní poznámky, které nemají být veřejné
- Velmi časté drobné změny (radši sbírejte změny)

## 🎯 Pokročilé tipy

### **Git pro různé typy dokumentů**:

#### **Prezentace** (Markdown):
```
Commit: "🎨 Redesign úvodních slides"
Commit: "📊 Aktualizace dat v middle section"  
Commit: "🎯 Přepracování call-to-action"
```

#### **Strategické dokumenty**:
```
Commit: "🎯 Definice cílů na Q2"
Commit: "📈 Analýza konkurence dopracována"
Commit: "💡 Přidány implementační kroky"
```

#### **Meeting notes**:
```
Commit: "📝 Notes z leadership meeting 25.1"
Commit: "✅ Action items assigned a clarified"
Commit: "📅 Přidány follow-up termíny"
```

**Pamatujte**: Git je nástroj, který vám pomůže pracovat organizovaněji a spolehlivěji. Nemusíte ho používat perfektně od začátku - důležité je začít!