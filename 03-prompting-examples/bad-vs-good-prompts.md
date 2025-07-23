# ❌✅ Bad vs Good Prompts - Srovnání s vysvětlením

## Příklad 1: E-mail žádost

### ❌ Špatný prompt
```
"Napiš e-mail o schůzce"
```

**Proč nefunguje:**
- Žádný kontext o účelu
- Nevíme komu píšeme
- Chybí informace o tónu
- Nespecifikovaná délka

### ✅ Dobrý prompt
```
"Jsem produktový manažer a potřebuji napsat e-mail našemu CTO o nutnosti urgentní schůzky ohledně critical bugu v produkci.

Kontext: Bug ovlivňuje 20% uživatelů a způsobuje data loss
Tón: Urgentní ale profesionální  
Délka: Krátký, max 100 slov
Zahrnout: Závažnost problému, navrhovaný čas schůzky (dnes odpoledne), seznam účastníků"
```

**Proč funguje:**
- Jasný kontext a role
- Specifické téma
- Definovaná závažnost
- Požadovaný tón a délka

---

## Příklad 2: Analýza dat

### ❌ Špatný prompt
```
"Podívej se na tyhle čísla a řekni co si myslíš"
```

**Proč nefunguje:**
- Neurčitá instrukce
- Chybí kontext dat
- Nevíme co hledáme
- Žádný požadovaný format

### ✅ Dobrý prompt
```
"Analyzuj tato čísla z našeho Q3 sales reportu:
[DATA]

Jsem sales manager a potřebuji připravit prezentaci pro vedení.
Focus na:
- Trendy oproti Q2
- Nejlepší a nejhorší performing produkty
- Geografické rozdíly
- Actionable insights pro Q4

Format: 5 bullet pointů s konkrétními čísly a doporučeními"
```

**Proč funguje:**
- Kontext dat i použití
- Specifické oblasti zájmu
- Jasný format výstupu
- Účel analýzy

---

## Příklad 3: Marketing content

### ❌ Špatný prompt
```
"Udělej reklamu na náš produkt"
```

**Proč nefunguje:**
- Neznámý produkt
- Neurčená platforma
- Chybí target audience
- Žádné požadavky na styl

### ✅ Dobrý prompt
```
"Vytvoř LinkedIn ad copy pro náš B2B projekt management nástroj 'TaskFlow'.

Target audience: IT manažeři ve firmách 50-200 zaměstnanců
USP: 40% rychlejší projekt completion díky AI automation
Konkurence: Asana, Monday.com
Budget na test: $1000

Format:
- Headline (max 25 znaků)
- Primary text (125 znaků)
- CTA button text
- 3 varianty A/B test"
```

**Proč funguje:**
- Specifický produkt a platforma
- Jasná target audience
- Unique selling proposition
- Formátové požadavky
- Testing approach

---

## Příklad 4: Meeting notes

### ❌ Špatný prompt
```
"Udělej z tohoto nějaký přehled"
[paste chaotických poznámek]
```

**Proý nefunguje:**
- Nestrukturovaná instrukce
- Chybí účel přehledu
- Neurčený format
- Žádný kontext meetingu

### ✅ Dobrý prompt
```
"Vytvoř strukturované shrnutí z těchto poznámek z product planning meetingu:
[poznámky]

Účastníci: PM, Design, Engineering, Marketing
Účel: Q4 roadmap planning

Format potřebný:
- Executive summary (3 věty)
- Klíčová rozhodnutí s owners
- Action items (kdo-co-kdy)
- Risikové faktory
- Next meeting date

Audience: Stakeholders kteří nebyli přítomni"
```

**Proč funguje:**
- Kontext meetingu
- Jasná struktura výstupu
- Identifikovaná audience
- Specifické sekce

---

## Příklad 5: Creative writing

### ❌ Špatný prompt
```
"Napi něco zajímavého o AI"
```

**Proč nefunguje:**
- Příliš široké téma
- Neurčený styl
- Chybí účel
- Žádné požadavky

### ✅ Dobrý prompt
```
"Napi blog post intro o tom, jak AI mění HR procesy v malých firmách.

Audience: HR manažeři bez tech background
Úhel: Praktické příklady, ne theoretical concepts
Tón: Accessible, optimistic ale realistic
Délka: 200 slov

Structure:
- Hook (surprising statistic)
- Problem statement
- 3 konkrétní AI use cases v HR
- Teaser na zbytek článku

Inspirace: Styl Harvard Business Review"
```

**Proč funguje:**
- Specifické téma a audience
- Jasný tón a styl
- Strukturované požadavky
- Reference point pro styl

---

## Zlatá pravidla

### ✅ Vždy zahrnout:
1. **Kontext** - Kdo jste, jaká situace
2. **Úkol** - Co přesně potřebujete
3. **Format** - Jak má výstup vypadat
4. **Audience** - Pro koho je to určeno
5. **Omezení** - Délka, styl, požadavky

### ❌ Vyvarovat se:
1. Vágních instrukcí
2. Příliš obecných témat
3. Chybějícího kontextu
4. Neurčitých požadavků
5. Očekávání perfekce na první pokus

---

**💡 Pro tip:** Představte si, že briefujete freelancera na Upworku - jaké informace by potřeboval k dokonalé práci?