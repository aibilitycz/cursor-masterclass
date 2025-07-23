# ❓ Ask vs Manual - Kdy nechat AI rozhodnout

## Co je rozdíl mezi Ask a Manual?

### 🤖 ASK Mode
AI **samo rozhoduje** jaký model použít pro váš úkol
- Cursor analyzuje váš prompt
- Vybere nejvhodnější model
- Optimalizuje cost vs quality automaticky

### 🎮 MANUAL Mode  
**Vy vybíráte** konkrétní model
- Máte plnou kontrolu
- Platíte za to, co si vyberete
- Musíte znát charakteristiky modelů

**Analogie:** Ask = "Objednej mi něco dobrého" vs Manual = "Chci přesně tuhle konkrétní položku"

## Kdy použít ASK

### ✅ Ideální pro:

#### 🚀 Začátečníky
```
Prompt: "Napiš mi e-mail zákazníkovi ohledně zpoždění dodávky"
ASK rozhodne: GPT-3.5 Turbo (routine communication)
Vy nemusíte: Znát rozdíly mezi modely
```

#### 🔄 Smíšené úkoly
```
Prompt: "Analyzuj tato data a vytvoř z toho executive summary"
ASK rozhodne: Claude pro analýzu → GPT-4 pro summary
Vy nemusíte: Řešit chain prompting
```

#### ⚡ Rychlá práce
```
Důvod: Nechcete přemýšlet o technických detailech
Focus: Na obsah, ne na nástroj
Výsledek: Rychlejší workflow
```

#### 💰 Cost optimization (long-term)
```
ASK se učí z vašich patterns:
- Pozná vaše preference
- Optimalizuje price/performance
- Zlepšuje se over time
```

### ❌ Méně vhodné pro:

#### 🎯 Specifické požadavky
```
"Potřebuji přesně GPT-4 pro tento client deliverable"
ASK může vybrat: Claude nebo GPT-3.5
Problém: Nesplní vaše přesné požadavky
```

#### 📊 Budget kontrola
```
Situace: Tight budget na project
ASK může: Vybrat drahé modely
Lepší: Manual control nad costs
```

#### 🔬 A/B Testing
```
Cíl: Porovnat výkon různých modelů
Potřeba: Konzistentní model choice
ASK: Může měnit modely between attempts
```

## Kdy použít MANUAL

### ✅ Ideální pro:

#### 💼 Mission-critical projekty
```
Úkol: Client presentation pro $100k deal
Volba: GPT-4 (bez kompromisů)
Důvod: Quality > Cost při high stakes
```

#### 🏷️ Strict budget kontrola
```
Scenario: Startup s limited AI budget
Strategy: GPT-3.5 Turbo pro většinu úkolů
Manual: Ensures cost predictability
```

#### 🧪 Experimentování
```
Test: Jak různé modely handleují naše use cases?
Approach: Systematické testování každého modelu
Data: Performance comparison
```

#### 🎯 Specialized workflows
```
Example: Legal document review
Requirement: Claude (safety focus)
Manual: Ensures compliance with procedures
```

### ❌ Méně vhodné pro:

#### 😰 Analysis paralysis
```
Problém: 10 minut selecting model pro 2-min úkol
Lepší: ASK pro routine tasks
```

#### 📚 Nedostatek zkušeností
```
Situace: Neznáte model capabilities
Risk: Suboptimal choices
Better: Learn with ASK first
```

## Praktické rozhodovací flowchart

```
START: Mám úkol pro AI

│
├─ Je to rutinní práce?
│  YES → ASK (optimal for routine)
│  NO ↓
│
├─ Mám strict budget limit?
│  YES → MANUAL (cost control)
│  NO ↓
│
├─ Je to mission-critical?
│  YES → MANUAL (quality assurance)
│  NO ↓
│
├─ Experimentuju s modely?
│  YES → MANUAL (controlled testing)
│  NO ↓
│
└─ DEFAULT → ASK (convenience + optimization)
```

## Hybrid approach - Nejlepší z obou světů

### 🎯 Strategic Manual, Tactical Ask
```
Strategic documents: Manual (GPT-4)
Daily communications: Ask (auto-optimize)
Research tasks: Manual (Claude)
Quick edits: Ask (efficiency)
```

### 📊 Learning phase → Control phase
```
Month 1-2: Use ASK everywhere
- Learn patterns
- Understand model strengths
- Build intuition

Month 3+: Switch to Manual for important tasks
- Apply learned knowledge  
- Optimize for specific needs
- Keep ASK for routine work
```

### 💰 Budget-aware switching
```
Budget tracking:
- High remaining budget → ASK (flexibility)
- Medium budget → Manual important, ASK routine
- Low budget → Manual (GPT-3.5 focus)
```

## Real-world examples

### Scenario 1: Sales Manager Monday
```
8:00 - Pipeline review email to team
Choice: ASK
Reason: Routine, want speed

9:30 - Proposal for major client  
Choice: MANUAL → GPT-4
Reason: High stakes, need quality

11:00 - Follow-up emails (5x)
Choice: ASK  
Reason: Volume work, let AI optimize

14:00 - Competitive analysis
Choice: MANUAL → Claude
Reason: Know Claude excels at analysis

16:00 - Social media posts
Choice: ASK
Reason: Creative content, not sure best model
```

### Scenario 2: Startup Founder (limited budget)
```
MANUAL strategy:
- GPT-3.5 Turbo: 80% of tasks
- GPT-4: Only investor communications
- Claude: Monthly market analysis

Result: Predictable costs, strategic quality
```

### Scenario 3: Enterprise Marketing Team
```
ASK for:
- Daily social content
- Internal communications  
- Brainstorming sessions

MANUAL for:
- Brand campaigns (GPT-4)
- Data analysis (Claude)
- Client presentations (GPT-4)

Result: Efficiency + Control where needed
```

## Performance tracking

### ASK Mode Metrics:
```
📊 Model distribution (which models chosen when)
💰 Cost per task vs Manual equivalent
⭐ Satisfaction with auto-selected models
📈 Improvement over time (learning curve)
```

### Manual Mode Metrics:
```
🎯 Hit rate (right model for task)
⏱️ Decision time (how long to choose)
💸 Cost efficiency vs ASK
🔄 Need for model switching mid-task
```

### Comparison Dashboard:
```markdown
# Monthly AI Usage Report

## ASK Performance
- Tasks completed: [number]
- Average cost: $[amount]
- Satisfaction score: [1-10]
- Model distribution: GPT-4: [%], GPT-3.5: [%], Claude: [%]

## Manual Performance  
- Tasks completed: [number]
- Average cost: $[amount]
- Satisfaction score: [1-10]
- Decision time: [minutes per task]

## Optimization Opportunities
- Tasks to switch from Manual to ASK: [list]
- Tasks to switch from ASK to Manual: [list]
- Cost savings potential: $[amount]
```

## Pro Tips pro kombinovaný approach

### 🧠 Develop intuition with ASK
```
Use ASK for 2-3 weeks on diverse tasks
Pay attention to which models it chooses
Note when you're satisfied vs disappointed
Build mental model of AI's decision logic
```

### 🎯 Create decision rules
```
ASK Rules:
- Unfamiliar task types
- Time pressure situations  
- Learning/experimental phases
- Cost not primary concern

Manual Rules:
- Client deliverables
- Brand-critical content
- Budget constraints
- Specific quality requirements
```

### 📚 Document your learnings
```markdown
# Personal AI Model Guide

## Tasks where ASK works great:
- [List based on experience]

## Tasks where Manual is better:
- [List with preferred models]

## Cost considerations:
- Monthly budget: $[amount]
- High-cost tasks: [list]
- Cost-sensitive tasks: [list]

## Quality requirements:
- Must be perfect: [Manual with GPT-4]
- Good enough: [ASK or Manual with GPT-3.5]
```

---

**💡 Strategic tip:** Začněte s ASK pro learning, postupně přejděte na hybrid approach kde ASK řeší routine a Manual důležité úkoly!