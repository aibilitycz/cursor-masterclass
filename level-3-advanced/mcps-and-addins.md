# 🔌 MCPs & Add-ins - Rozšíření pro power users

Tento průvodce vám ukáže jak nainstalovat a používat nejužitečnější rozšíření Cursoru pro business účely.

## 🌐 cursor.directory - Váš app store pro Cursor

### Co je cursor.directory?
Oficiální katalog rozšíření pro Cursor. Obsahuje:
- **MCPs** (Model Context Protocols) - rozšíření AI schopností
- **Templates** - hotové šablony pro různé úkoly
- **Workflows** - kompletní pracovní postupy
- **Integrations** - propojení s externími službami

### 🎯 Jak procházet cursor.directory:

#### **Filtry podle kategorie**:
- 📊 **Data & Analytics**: Excel, CSV, database rozšíření
- 📧 **Communication**: E-mail, chat, kalendář integrace
- 🎨 **Design & Media**: Grafika, layout, multimedia
- 📝 **Content & Writing**: Text processing, dokumentace
- 🔧 **Productivity**: Task management, automation

#### **Filtry podle popularitě**:
- ⭐ **Most Popular**: Nejvíce stahovaná rozšíření
- 🆕 **Recently Added**: Nejnovější přídavky
- 🔥 **Trending**: Momentálně populární

## 📊 Top MCPs pro Business Uživatele

### **1. CSV Analyzer MCP**

#### Co umí:
- Automatická analýza CSV dat
- Vytváření insights a trendů
- Export grafů a vizualizací
- Data cleaning a preprocessing

#### Installation:
```json
{
  "mcpServers": {
    "csv-analyzer": {
      "command": "npx",
      "args": ["@cursor/csv-analyzer-mcp"]
    }
  }
}
```

#### Praktické použití:
```
🎯 Input: "Analyzuj tento sales CSV soubor"

📊 Output:
- Revenue trend: +15% growth month-over-month
- Top customer: ABC Corp (25% of total revenue)  
- Seasonal pattern: Peak in Q4, drop in Q1
- Recommendations: Focus on customer retention in Q1
+ Automatically generated charts saved as PNG
```

### **2. Email Composer MCP**

#### Co umí:
- Profesionální e-mail templates
- Auto-detection příjemce typu (client/colleague/vendor)
- Tone adjustment podle kontextu
- Follow-up suggestions

#### Installation:
```json
{
  "mcpServers": {
    "email-composer": {
      "command": "npx", 
      "args": ["@cursor/email-composer-mcp"]
    }
  }
}
```

#### Praktické použití:
```
🎯 Input: "Napiš follow-up e-mail klientovi ohledně delayed projektu"

📧 Output:
Subject: Project Update - Revised Timeline for [Project Name]

Dear [Client Name],

I hope this email finds you well. I wanted to provide you with an 
important update regarding the progress of [Project Name].

[Professional explanation of delay]
[Revised timeline with specific dates]  
[Assurance of quality commitment]
[Next steps and communication plan]

Best regards,
[Your name]

💡 Suggestions:
- Schedule follow-up call in 3 days
- Send weekly progress updates
- Offer client call to discuss concerns
```

### **3. PDF Reader MCP**

#### Co umí:
- Čtení a parsing PDF dokumentů
- Extrakce klíčových informací
- Summarization dlouhých dokumentů
- Data extraction do strukturovaných formátů

#### Installation:
```json
{
  "mcpServers": {
    "pdf-reader": {
      "command": "npx",
      "args": ["@cursor/pdf-reader-mcp"]
    }
  }
}
```

#### Praktické použití:
```
🎯 Input: "Shrni mi hlavní body z tohoto 50stranového kontraktu"

📄 Output:
📋 Contract Summary:
- **Parties**: [Company A] and [Company B]
- **Duration**: 3 years (2024-2027)  
- **Value**: $2.5M total ($833k annually)
- **Key Terms**:
  • Payment: Net 30, quarterly invoicing
  • Deliverables: Monthly reports + quarterly reviews
  • Termination: 90-day notice required
- **Important Dates**:
  • Start: March 1, 2024
  • First review: June 1, 2024
  • Renewal deadline: December 1, 2026
  
⚠️ **Action Items**:
- Set calendar reminder for renewal discussion
- Prepare first quarterly report template
- Schedule kickoff meeting with stakeholders
```

### **4. Calendar Integration MCP**

#### Co umí:
- Čtení kalendáře a detekce konfliktů
- Automatické scheduling s multiple participants
- Meeting preparation suggestions
- Time zone handling

#### Installation:
```json
{
  "mcpServers": {
    "calendar-mcp": {
      "command": "npx",
      "args": ["@cursor/calendar-integration-mcp"],
      "env": {
        "CALENDAR_API_KEY": "your-api-key"
      }
    }
  }
}
```

#### Praktické použití:
```
🎯 Input: "Naplánuj review meeting s týmem na příští týden"

🗓️ Output:
📅 **Meeting Scheduled**: Project Review Meeting
- **Date**: Tuesday, February 6, 2024
- **Time**: 10:00 AM - 11:00 AM (avoided conflicts with Jana's client call)
- **Attendees**: You, Jana, Petr, Milan (Sarah declined - on vacation)
- **Location**: Conference Room B (auto-booked)

📧 **Calendar Invite Sent** with agenda:
1. Sprint progress review (15min)
2. Blockers discussion (20min)  
3. Next sprint planning (20min)
4. Action items (5min)

💡 **Prep Suggestions**:
- Review last week's action items
- Prepare sprint metrics dashboard
- Collect team feedback on current process
```

## 🔧 Top Add-ins pro Productivity

### **1. Taskmaster - AI Task Management**

#### Hlavní funkce:
- **Smart task breakdown** - Rozloží velké projekty na menší úkoly
- **Time estimation** - AI odhad času potřebného pro každý úkol
- **Dependency mapping** - Identifikuje závislosti mezi úkoly
- **Priority scoring** - Automatické prioritizace podle urgency/importance

#### Installation:
1. Extensions panel (`Ctrl+Shift+X`)
2. Search "Taskmaster"
3. Install → Reload Cursor
4. First-time setup: Define your working style preferences

#### Praktické použití:

##### **Project Breakdown**:
```
🎯 Input: "Potřebuju zorganizovat launch nového produktu do 8 týdnů"

📋 Taskmaster Output:

🚀 **Product Launch Project** (8 weeks)
┌─ **Phase 1: Planning** (Week 1-2)
│  ├─ 📊 Market research completion (8h) - Priority: High
│  ├─ 🎯 Define target audience segments (4h) - Priority: High  
│  ├─ 💰 Finalize pricing strategy (6h) - Priority: High
│  └─ 📅 Create detailed launch timeline (3h) - Priority: Medium
│
├─ **Phase 2: Content Creation** (Week 3-5)  
│  ├─ 🎨 Product messaging & positioning (12h) - Priority: High
│  │   └─ Depends on: Market research completion
│  ├─ 📸 Product photography/visuals (16h) - Priority: High
│  ├─ 📝 Website copy & landing pages (20h) - Priority: High  
│  └─ 📱 Social media content bank (10h) - Priority: Medium
│
├─ **Phase 3: Marketing Setup** (Week 4-6)
│  ├─ 📧 Email campaign sequences (8h) - Priority: High
│  ├─ 🎯 Ad campaigns setup (6h) - Priority: High
│  ├─ 🤝 Influencer outreach (4h) - Priority: Medium
│  └─ 📺 PR strategy & press kit (8h) - Priority: Medium
│
└─ **Phase 4: Launch Execution** (Week 7-8)
   ├─ 🌟 Soft launch to beta users (2h) - Priority: High
   ├─ 📊 Monitor metrics & feedback (ongoing) - Priority: High
   ├─ 🚀 Public launch event (4h) - Priority: High
   └─ 📈 Post-launch optimization (ongoing) - Priority: Medium

⚠️ **Risk Factors**:
- Product photography dependent on product availability
- PR outreach needs 2-week lead time  
- Beta feedback might require product changes

🎯 **Success Metrics**:
- 1000 signups in first week
- 50% email open rate
- 5% conversion rate from landing page
```

##### **Daily Task Optimization**:
```
🎯 Input: Taskmaster, optimize my day based on these tasks:
- Finish quarterly report (high priority)
- Review marketing proposals (medium) 
- Call supplier about delivery (urgent)
- Team 1:1 meetings (scheduled)
- Email responses (ongoing)

⏰ **Optimized Schedule**:
9:00-9:15   ☎️  Call supplier (urgent + when they're available)
9:15-11:00  📊 Quarterly report - deep work block  
11:00-11:15 ☕ Break
11:15-12:00 📧 Email responses - batch processing
12:00-13:00 🍽️ Lunch
13:00-14:30 📝 Review marketing proposals (post-lunch analysis)
14:30-16:00 👥 Team 1:1s (3x 30min slots)
16:00-17:00 📊 Finish quarterly report (if needed)

💡 **Optimization Notes**:
- Urgent call scheduled early when supplier is fresh
- Deep work (report) in morning high-energy period
- Email batching reduces context switching  
- Analysis work after lunch when energy dips
- 1:1s in afternoon when people are more reflective
```

### **2. Superdesign.dev - AI Design Assistant**

#### Hlavní funkce:
- **Auto-layout generation** pro dokumenty a prezentace
- **Brand consistency** enforcement
- **Typography optimization** pro readability
- **Color scheme suggestions** based on psychology

#### Installation:
1. Visit superdesign.dev
2. Install Cursor extension
3. Connect to your brand guidelines (optional)
4. Set design preferences

#### Praktické použití:

##### **Document Beautification**:
```markdown
<!-- Před Superdesign -->
# Quarterly Report
Revenue was up 15% this quarter. 
Here are the numbers:
- Q1: $100k
- Q2: $115k  
Customer satisfaction is good.
We had some challenges with delivery times.

<!-- Po Superdesign -->
<div class="quarterly-report-layout">
  <header class="report-header">
    <div class="company-logo"></div>
    <h1 class="report-title">Q2 Performance Report</h1>
    <div class="report-date">July 2024</div>
  </header>
  
  <section class="executive-summary">
    <div class="highlight-box success">
      <h2>📈 Revenue Growth</h2>
      <div class="stat-large">+15%</div>
      <p>Quarter-over-quarter improvement</p>
    </div>
  </section>
  
  <section class="key-metrics">
    <div class="metrics-grid">
      <div class="metric-card">
        <h3>Q1 Revenue</h3>
        <div class="metric-value">$100K</div>
      </div>
      <div class="metric-card highlight">
        <h3>Q2 Revenue</h3>
        <div class="metric-value">$115K</div>
        <div class="metric-change positive">+15%</div>
      </div>
    </div>
  </section>
  
  <section class="challenges">
    <div class="warning-box">
      <h2>⚠️ Areas for Improvement</h2>
      <ul>
        <li>Delivery time optimization needed</li>
        <li>Customer satisfaction monitoring enhanced</li>
      </ul>
    </div>
  </section>
</div>
```

##### **Presentation Makeover**:
```
🎯 Input: "Improve this presentation layout for executive audience"

🎨 Superdesign Suggestions:

**Slide Structure**:
- 🏗️ Master slide with consistent header/footer
- 📊 Data slides with max 3 key points
- 🎯 One main message per slide
- 📱 Mobile-friendly layouts

**Visual Hierarchy**:  
- Headers: 32pt, brand blue, medium weight
- Body text: 18pt, dark gray, regular weight
- Callouts: 24pt, accent color, bold weight
- Captions: 14pt, light gray, italic

**Color Psychology Applied**:
- 💙 Blue (trust) for financial data
- 💚 Green (growth) for positive metrics  
- 🟡 Yellow (caution) for risks/challenges
- ⚫ Dark gray for supporting text

**Layout Improvements**:
- Consistent 40px margins on all slides
- Grid-based alignment for professional look
- White space utilization for focus
- Progressive disclosure for complex information

**Executive-Specific Optimizations**:
- Key takeaways in first 3 slides
- Executive summary with 30-second read time
- Action items clearly highlighted
- Financial implications upfront
```

### **3. Writing Assistant Pro**

#### Hlavní funkce:
- **Advanced grammar & style** checking
- **Tone adjustment** pro různé audience
- **Readability optimization** 
- **Plagiarism detection**

#### Praktické použití:
```
🎯 Input: "Optimize this email for C-level audience"

Original: "Hey, so we had some issues with the project but I think 
we can fix them pretty quickly. Let me know what you think."

✍️ **Writing Assistant Pro Output**:

**Tone Analysis**: Too casual for C-level (Score: 2/10)
**Readability**: Good (Grade 8 level)
**Issues Found**: 
- Vague language ("some issues", "pretty quickly")
- Lacks specificity and accountability
- Missing clear next steps

**Optimized Version**:
"Good morning [Executive Name],

I'm writing to inform you of project challenges we've identified 
and our resolution plan.

**Current Situation**: 
We've encountered delivery delays due to supplier issues, 
impacting our March 15th deadline.

**Resolution Plan**:
- Alternative supplier secured (delivery by March 10th)
- Internal process adjusted to prevent recurrence
- Client communication handled proactively

**Impact**: 2-day delay, no budget implications
**Next Steps**: Status update scheduled for Friday

I'm available for immediate discussion if needed.

Best regards,
[Your name]"

**Improvements Made**:  
✅ Professional greeting
✅ Specific problem identification
✅ Clear action plan
✅ Quantified impact
✅ Proactive communication offer
✅ Executive-appropriate level of detail
```

## 🛠️ Installation Guide

### **Metoda 1: Přes cursor.directory**

1. **Navštivte** [cursor.directory](https://cursor.directory)
2. **Najděte rozšíření** které chcete
3. **Zkopírujte installation code**
4. **V Cursoru**: `Ctrl+Shift+P` → "Open Settings (JSON)"
5. **Přidejte konfiguraci** do settings.json
6. **Restartujte Cursor**

### **Metoda 2: Přes Extensions Marketplace**

1. **Otevřete Extensions** (`Ctrl+Shift+X`)
2. **Hledejte název add-inu**
3. **Klikněte Install**
4. **Povolte extension**
5. **Configure podle potřeby**

### **Troubleshooting Installation**:

#### **MCP se nenačítá**:
```bash
# Zkontrolujte logs
Ctrl+Shift+P → "Developer: Show Logs" → Extension Host

# Časté řešení:
- Restartujte Cursor
- Zkontrolujte API klíče v settings
- Ověřte network connection
```

#### **Add-in nefunguje**:
```bash
# Reset extension
Ctrl+Shift+P → "Extensions: Disable All" → Enable jen potřebné

# Zkontrolujte verzi Cursoru
Help → About → Update if needed
```

## 💡 Best Practices pro rozšíření

### ✅ Dos:
- **Začněte pomalu** - instalujte max 2-3 rozšíření najednou
- **Testujte funkce** před produkčním použitím
- **Čtěte dokumentaci** každého rozšíření
- **Updatujte pravidelně** pro bug fixes a nové funkce

### ❌ Don'ts:
- **Neinstalujte vše najednou** - může způsobit konflikty
- **Nedůvěřujte slepě** AI výstupům z rozšíření
- **Nesdílejte API klíče** v team settings
- **Nepoužívejte experimentální** rozšíření pro kritické úkoly

### 🔐 Security Tips:
- **Ověřte autora** rozšíření před instalací
- **Čtěte permissions** které rozšíření vyžaduje
- **Používejte API klíče** s omezenými právy
- **Pravidelně reviewujte** nainstalovaná rozšíření

**Pamatujte**: Rozšíření jsou mocné nástroje, ale zodpovědnost za výsledky je stále na vás!