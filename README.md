═══════════════════════════════════════════════════════════════════════════════
    GEMINI ORCHESTRATOR - CAREER NETWORK EXTENSION
═══════════════════════════════════════════════════════════════════════════════

✅ WHAT YOU HAVE:

1. GEMINI.md
   └─ The orchestrator/hub for the entire Career Network
   └─ Listens, delegates to agents, synthesizes, manages context
   └─ Token-efficient design (summarizes, stores in CAREER_LOG.md)

2. GEMINI_EXTENSION_STRUCTURE.md
   └─ Complete setup guide for file structure
   └─ How to configure in Gemini CLI
   └─ Workflow examples and token management

Plus: 7 agents (from previous GEM_AGENTS_YAML_GEMINI_CLI.md)

═══════════════════════════════════════════════════════════════════════════════

📁 FILE STRUCTURE FOR GEMINI CLI:

~/.gemini/extensions/career-network/
├── GEMINI.md                           ← Orchestrator (load this)
├── CAREER_LOG.md                       ← Auto-created on first run
└── agents/
    ├── career-futurist.md              ← Agent 1
    ├── career-strategist.md            ← Agent 2
    ├── learning-architect.md           ← Agent 3
    ├── tech-drill-sergeant.md          ← Agent 4
    ├── psych-advisor.md                ← Agent 5
    ├── cv-specialist.md                ← Agent 6
    └── case-simulator.md               ← Agent 7

═══════════════════════════════════════════════════════════════════════════════

🤖 THE ORCHESTRATOR (GEMINI.md)

What it does:
✓ Listens to user input
✓ Identifies which agent(s) you need
✓ Delegates using @agent-name syntax
✓ Brings back key insights concisely
✓ Saves important findings to CAREER_LOG.md
✓ Manages context to prevent token bloat
✓ Guides you to the next logical step

Key behaviors:
- Summarizes agent outputs (2-3 bullets, not full transcripts)
- Stores strategic findings in CAREER_LOG.md
- Reads CAREER_LOG.md when relevant
- Resets context when conversations get long
- References past work: "Last session we identified..."

═══════════════════════════════════════════════════════════════════════════════

7️⃣ THE AGENTS (Specialized Experts)

@career-futurist
  → Discovers Blue Ocean opportunities
  → Market validation and industry analysis
  → When: You need direction and vision

@career-strategist
  → Maps technical gaps
  → Ranks roles by achievability
  → When: You have target roles defined

@learning-architect
  → Designs 14-day skill-building sprints
  → Creates progressive problem sets
  → When: You're ready to learn

@tech-drill-sergeant
  → Timed challenges under pressure
  → Diagnoses failure root-cause
  → When: You're testing your skills

@psych-advisor
  → Cognitive reframes after failures
  → Momentum and confidence management
  → When: You're struggling or doubting

@cv-specialist
  → Resume translation and optimization
  → ATS keyword injection
  → When: Preparing to apply

@case-simulator
  → System design interview cases
  → Architectural thinking challenges
  → When: Preparing for senior interviews

═══════════════════════════════════════════════════════════════════════════════

🎯 USER JOURNEY (No Time Constraints)

The orchestrator doesn't enforce timeframes. Instead, it recognizes where you are:

Phase 1: Discovery
  → Need direction? Delegate to @career-futurist

Phase 2: Analysis
  → Know what you want? Delegate to @career-strategist

Phase 3: Building
  → Ready to learn? Delegate to @learning-architect
  → Concurrent: @tech-drill-sergeant for pressure testing

Phase 4: Support
  → Struggling? Delegate to @psych-advisor anytime

Phase 5: Positioning
  → Applying soon? Delegate to @cv-specialist

Phase 6: Interviewing
  → In interviews? Delegate to @case-simulator

Note: Users don't move linearly. They cycle, loop, and work on multiple phases
simultaneously. The orchestrator helps them navigate where THEY are.

═══════════════════════════════════════════════════════════════════════════════

⚡ TOKEN MANAGEMENT (Key Innovation)

The orchestrator prevents token bloat by:

1. Summarization Rule
   ✓ Agent provides 500 words
   ✓ Orchestrator extracts 2-3 key bullets
   ✓ User gets insight, not transcript

2. Persistent Storage
   ✓ Important findings → CAREER_LOG.md
   ✓ Conversation stays lean
   ✓ Context focused on current task

3. Session Compaction
   ✓ Long conversations get summarized
   ✓ "Should I save our findings and start fresh?"
   ✓ Keeps each session efficient

4. Selective Reading
   ✓ Only reads CAREER_LOG.md when needed
   ✓ Strategic, not reflexive
   ✓ "Let me check where we left off..."

═══════════════════════════════════════════════════════════════════════════════

🚀 QUICK START

1. Create directory structure:
   mkdir -p ~/.gemini/extensions/career-network/agents

2. Copy GEMINI.md to:
   ~/.gemini/extensions/career-network/GEMINI.md

3. Copy 7 agents to:
   ~/.gemini/extensions/career-network/agents/[agent-name].md

4. Load extension:
   gemini load-extension ~/.gemini/extensions/career-network/GEMINI.md

5. Start conversation:
   "Hey! I have 11 years in SAP and I'm pivoting to modern tech. Where should I start?"

═══════════════════════════════════════════════════════════════════════════════

📋 CAREER_LOG.md (Persistent Progress)

Auto-created on first interaction. Contains:

✓ Strategic Direction (opportunities identified)
✓ Gap Analysis (blockers identified)
✓ Learning Progress (skills being built)
✓ Interview Preparation (practice results)
✓ Resume Versions (tailored documents)
✓ Resilience Notes (confidence trends)
✓ Next Actions (what's coming up)

This file persists across sessions. The orchestrator reads it to provide continuity.

═══════════════════════════════════════════════════════════════════════════════

💡 KEY DIFFERENCES FROM AGENTS

Orchestrator (GEMINI.md):
- Central hub
- Routes to specialists
- Synthesizes insights
- Manages context
- Maintains log
- Guides journey
- No timeframes

Agents:
- Deep expertise
- Specialized knowledge
- Execute specific tasks
- Detailed outputs
- Focused scope
- Technical excellence

═══════════════════════════════════════════════════════════════════════════════

✅ FILES YOU NEED

New files:
+ GEMINI.md                        ← Orchestrator
+ GEMINI_EXTENSION_STRUCTURE.md    ← Setup guide
+ This README.txt                  ← Quick reference

From previous:
+ GEM_AGENTS_YAML_GEMINI_CLI.md    ← All 7 agents

═══════════════════════════════════════════════════════════════════════════════

🎓 GETTING STARTED

1. Read: This file (2 minutes)
2. Read: GEMINI_EXTENSION_STRUCTURE.md (5 minutes for details)
3. Copy: Files to ~/.gemini/extensions/career-network/
4. Load: Extension in Gemini CLI
5. Talk: "I'm ready to pivot. Help me figure out my path."

═══════════════════════════════════════════════════════════════════════════════

📞 EXAMPLE FIRST INTERACTION

You: "I have 11 years in SAP and I'm trying to pivot to modern tech. 
     I've started learning Python and RAG but I'm not sure what roles 
     to target or where this background creates real advantages."

Orchestrator: "Got it. Let me connect you with our futurist agent to 
             explore where your unique background creates unfair 
             advantages in emerging industries."

@career-futurist: [Detailed analysis of Blue Ocean opportunities]

Orchestrator: "Excellent! The futurist has identified 3 emerging industries 
             where your systems expertise is desperately needed. Should 
             we save these to your career progress file and explore one 
             deeper?"

═══════════════════════════════════════════════════════════════════════════════

That's it! Your orchestrator is ready.

Questions? See GEMINI_EXTENSION_STRUCTURE.md

Ready to go! 🚀