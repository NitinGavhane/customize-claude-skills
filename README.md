# Custom Claude Skills

A collection of specialized skills for Claude AI that extend its capabilities for business analysis, writing enhancement, and B2B outreach.

## Available Skills

### 1. swot-business-plan
**Purpose:** Generates a deep, niche-specific SWOT analysis followed by a scalable, profitable business plan outline.

**When to use:**
- "SWOT analysis"
- "business plan"
- "analyze my business idea"
- "strengths and weaknesses of my business"
- "is my idea viable"
- "help me start a business"
- "plan my startup"
- "what's my competitive advantage"
- "business strategy for my niche"

**What it delivers:**
- Detailed SWOT analysis (Strengths, Weaknesses, Opportunities, Threats)
- Actionable recommendations (SO, WO, WT strategies)
- Streamlined business plan outline with executive summary, business model, target market, go-to-market strategy, and financial milestones

---

### 2. humanizer
**Purpose:** Removes signs of AI-generated writing from text to make it sound more natural and human-written.

**When to use:**
- "humanize this text"
- "make this sound more human"
- "fix AI writing patterns"
- "rewrite this to sound natural"

**What it does:**
- Identifies and removes 29+ AI writing patterns including:
  - Inflated symbolism and promotional language
  - Superficial -ing analyses
  - Vague attributions and weasel words
  - Em dash overuse
  - Rule of three patterns
  - AI vocabulary words (actually, crucial, pivotal, etc.)
  - Passive voice overuse
  - Generic positive conclusions
  - Filler phrases and hedging

**How to use:**
```
humanizer
[Your AI-generated text here]
```

---

### 3. linkedin-dm-angle-generator
**Purpose:** Generates a numbered bank of psychologically sharp LinkedIn cold DM conversation-opening angles, custom to your ICP, offer, and niche.

**When to use:**
- "generate LinkedIn angles"
- "help me with cold DM angles"
- "give me LinkedIn outreach angles"
- "create DM opening angles"
- "I need angles for cold outreach"
- "build me an angle bank"
- "LinkedIn cold message angles"

**What it does NOT do:**
- Does not write DM copy or templates
- Does not produce generic frameworks
- Does not proceed without complete inputs

**What it delivers:**
- Custom angle banks based on your specific ICP and psychographics
- 12 psychological territories: Pain, Desired Outcome, Humor, Absurdity, Provocation, Curiosity, Identity, Fear, Social Dynamics, Contrarian, Industry Observation, Ambition
- Each angle includes psychological reasoning and what conversation it opens

**How to use:**
```
linkedin-dm-angle-generator
[Your offer, ICP demographics, psychographics, and preferred territories]
```

---

## Installation

### For Claude Code / Opencode

Copy the `.skill` files to your skills directory:

```bash
# Claude Code
cp *.skill ~/.claude/skills/

# Opencode
cp *.skill ~/.opencode/skills/
```

### Manual Installation

1. Download the `.skill` file you want to use
2. Place it in your Claude/Opencode skills directory
3. Restart Claude or reload your session

---

## Usage Examples

### SWOT + Business Plan
```
I want to start a SaaS tool for solo law firms that helps with client intake and billing. Can you do a SWOT analysis and business plan?
```

### Humanizer
```
Humanize this text:
[paste AI-generated content here]
```

### LinkedIn Angle Generator
```
linkedin-dm-angle-generator

1. OFFER: Cold email software for B2B SaaS companies, helps with deliverability and personalization at scale

2. ICP DEMOGRAPHICS: VP of Sales or Head of Sales, 50-200 person B2B SaaS companies, US-based

3. ICP PSYCHOGRAPHICS: 
- Runs 3-5 person sales teams
- Spends Sunday nights updating pipeline because they don't trust reps
- Frustrated by tools that create more work than they save
- Quietly worried about maintaining quota in a downturn

4. NUMBER OF ANGLES: 10

5. ANGLE TYPES: ALL
```

---

## Skills Structure

Each `.skill` file is a zip archive containing:

```
skill-name.skill/
├── SKILL.md          # Main skill definition and instructions
├── README.md         # Skill-specific documentation (optional)
└── .claude/
    └── settings.local.json  # Skill configuration
```

---

## Contributing

To create a new skill:

1. Create a directory for your skill
2. Write your `SKILL.md` with clear triggers, instructions, and examples
3. Zip the directory
4. Rename to `.skill` extension
5. Submit a pull request

---

## License

MIT License - See individual skill files for specific licensing terms.