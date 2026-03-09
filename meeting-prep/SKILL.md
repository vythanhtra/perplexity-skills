# Skill: Meeting Preparation

## Overview
This skill enables Perplexity AI to conduct comprehensive pre-meeting research and generate structured briefing documents, helping professionals walk into every meeting fully informed and ready to add value.

## Skill Metadata
- **Skill ID:** meeting-prep
- **Category:** Productivity & Communication
- **Complexity:** Intermediate
- **Estimated Time:** 5-20 minutes per meeting
- **Output Format:** Meeting Briefing Document (Markdown)

## Capabilities

### 1. Participant Research
- Professional background and career history
- Current role, responsibilities, and tenure
- Published articles, interviews, and public statements
- LinkedIn activity, interests, and expertise areas
- Mutual connections and shared experiences

### 2. Company Intelligence
- Company overview, size, funding stage, and industry
- Recent news, press releases, and announcements
- Products, services, and business model
- Key challenges and strategic priorities
- Competitors and market position

### 3. Agenda & Context Preparation
- Meeting objective clarification
- Relevant background context for discussion topics
- Prior meeting notes and action item follow-ups
- Industry trends relevant to meeting topics
- Potential pain points and opportunities to address

### 4. Question & Talking Point Generation
- Thoughtful questions to ask participants
- Key points to communicate or advocate for
- Potential objections and responses
- Success criteria for the meeting

### 5. Post-Meeting Setup
- Template for meeting notes
- Follow-up action item tracker
- Next steps document structure

## Input Requirements

```yaml
required_inputs:
  - meeting_type: "sales|interview|partnership|team|board|vendor|networking"
  - participants: "Names and companies of key participants"
  - meeting_objective: "What you want to achieve"

optional_inputs:
  - agenda_items: "Specific topics to be discussed"
  - prior_context: "Previous interactions or relevant history"
  - your_role: "Your position and what you're representing"
  - meeting_duration: "Length of the meeting"
  - prep_depth: "quick|standard|deep"
```

## Step-by-Step Workflow

### Phase 1: Participant Intelligence (5-10 min)

**Step 1: Individual Research**
```
For each key participant, research:
- Current title and company
- Career background (last 3-5 years)
- Educational background
- Published content or notable quotes
- Recent activity (posts, articles, speaking engagements)
- Any awards or recognition
```

**Step 2: Identify Conversation Hooks**
```
Look for:
- Shared connections or alma maters
- Common interests or expertise areas
- Recent milestones (promotions, company news)
- Their stated priorities or challenges
- Projects they are publicly excited about
```

### Phase 2: Company & Context Research (5-10 min)

**Step 3: Company Deep-Dive**
```
Research areas:
- Founding story and mission
- Current product/service offerings
- Business model and revenue approach
- Recent funding, M&A, or major announcements
- Key customers and use cases
- Technology stack (if relevant)
- Culture and values signals
```

**Step 4: Industry Context**
```
Gather:
- Current trends affecting their business
- Regulatory or market changes
- Competitor landscape overview
- Analyst reports or expert opinions
- Macroeconomic factors relevant to their sector
```

### Phase 3: Meeting Strategy (2-5 min)

**Step 5: Objective Alignment**
- Clarify primary goal (inform, persuade, explore, decide)
- Identify secondary goals
- Define success criteria
- Anticipate their objectives and expectations

**Step 6: Question Preparation**

| Question Type | Purpose | Example |
|--------------|---------|--------|
| Discovery | Understand their situation | "What is your biggest challenge with X?" |
| Qualifying | Assess fit/readiness | "How are you currently handling Y?" |
| Vision | Explore future state | "Where do you want to be in 12 months?" |
| Validation | Confirm understanding | "Did I capture that correctly?" |
| Next Steps | Drive action | "What would need to happen for us to move forward?" |

## Output Template

```markdown
# Meeting Brief: [Meeting Title]
**Date & Time:** [Date] at [Time]
**Duration:** [X] minutes
**Location/Platform:** [In-person/Zoom/Teams]
**Prepared by:** [Your Name]
**Objective:** [One sentence goal]

---

## Participants

### [Participant Name] - [Title] at [Company]
- **Background:** [2-3 sentences on career history]
- **Current Focus:** [What they are working on now]
- **Notable:** [Interesting fact, recent achievement, or connection point]
- **LinkedIn:** [URL]

---

## Company Overview: [Company Name]
- **Founded:** [Year] | **Size:** [Employees] | **Stage:** [Startup/Growth/Enterprise]
- **What they do:** [One sentence description]
- **Recent news:** [Key recent development]
- **Key challenge:** [Known pain point or strategic priority]

---

## Agenda & Talking Points

### Topic 1: [Agenda Item]
- Background context: [Relevant info]
- Your key message: [What to communicate]
- Questions to ask: [2-3 questions]

### Topic 2: [Agenda Item]
- Background context: [Relevant info]
- Your key message: [What to communicate]
- Questions to ask: [2-3 questions]

---

## My Key Messages
1. [Most important point to communicate]
2. [Second key message]
3. [Third key message]

## Questions to Ask
1. [High-priority question]
2. [Discovery question]
3. [Future-state question]
4. [Follow-up based on research]

## Potential Objections & Responses
| They might say... | I will respond with... |
|------------------|----------------------|
| [Objection 1] | [Response] |
| [Objection 2] | [Response] |

## Success Criteria
- [ ] [Primary outcome to achieve]
- [ ] [Secondary outcome]
- [ ] [Relationship goal]

---

## Notes Template
_Use during meeting:_

**Key points discussed:**
-

**Decisions made:**
-

**Action items:**
| Action | Owner | Due Date |
|--------|-------|----------|
| | | |

**Next meeting:** [Date/Topic]
```

## Meeting Type Variations

### Sales Meeting Prep
- Research prospect's tech stack and tools
- Identify budget signals and buying process
- Find champion vs. economic buyer
- Review similar customer case studies
- Prepare ROI talking points

### Job Interview Prep
- Study job description deeply
- Research interviewer's background
- Prepare STAR method stories
- Research company culture and values
- Prepare thoughtful questions about the role

### Partnership/BD Meeting
- Map complementary capabilities
- Identify overlap and white space
- Research their existing partner ecosystem
- Prepare mutual value proposition
- Understand their integration/partnership process

### Board/Executive Presentation
- Know the audience's priorities and concerns
- Prepare data-driven supporting materials
- Anticipate tough questions
- Have backup slides for deep dives
- Practice concise executive summaries

## Perplexity-Specific Tips

- Search "[Person Name] [Company]" for quick professional overview
- Use **Focus: News** for recent company announcements
- Search "[Company] challenges 2024" for pain point intelligence
- Use **Spaces** to save meeting preps for recurring meetings
- Enable **Pro Search** for deeper LinkedIn and web coverage
- Export briefing document before the meeting

## Time-Based Prep Guides

### 5-Minute Quick Prep
1. Google participant name + company
2. Check company LinkedIn page
3. Write 2 questions to ask
4. Review your talking points

### 15-Minute Standard Prep
1. Research all participants (3 min each)
2. Company overview and recent news
3. Prepare 5 questions
4. Write key messages
5. Set success criteria

### 30-Minute Deep Prep
1. Full participant research with hooks
2. Company deep-dive including competitors
3. Industry context gathering
4. Prepare full briefing document
5. Practice key talking points
6. Prepare for likely objections

## Success Metrics
- Meeting objective achievement rate
- Time saved vs. manual research (target: 60% reduction)
- Quality of questions asked (self-rated)
- Follow-up conversion rate (for sales meetings)
- Participant feedback on meeting value
