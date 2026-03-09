# Skill: Sales Prospecting

## Overview
This skill enables Perplexity AI to identify, research, and qualify potential sales prospects, building targeted prospect lists and personalized outreach intelligence to accelerate pipeline development.

## Skill Metadata
- **Skill ID:** sales-prospecting
- **Category:** Sales & Revenue
- **Complexity:** Advanced
- **Estimated Time:** 10-30 minutes per prospect or list
- **Output Format:** Prospect Profile + Outreach Brief (Markdown)

## Capabilities

### 1. Ideal Customer Profile (ICP) Research
- Define target company characteristics (industry, size, stage, geography)
- Map buying signals and trigger events
- Identify technology stack indicators
- Research budget and spending signals
- Validate ICP fit against known customer profiles

### 2. Prospect Identification
- Company discovery based on ICP criteria
- Contact identification (decision makers, champions, influencers)
- Organizational mapping and buying committee research
- Signal-based prospecting (funding, hiring, news events)
- Competitor customer identification

### 3. Account Intelligence
- Company financials and growth indicators
- Recent news and strategic announcements
- Technology stack and tool usage
- Key initiatives and strategic priorities
- Pain points and challenges based on public information

### 4. Contact Research
- Decision maker background and career history
- Published content, talks, and thought leadership
- Trigger events (promotions, company changes, new roles)
- Communication preferences and activity patterns

### 5. Personalized Outreach Intelligence
- Hyper-personalized email hooks
- Relevant talking points for cold calls
- Value proposition alignment to prospect's context
- Timing recommendations based on signals
- Multi-touch sequence recommendations

## Input Requirements

```yaml
required_inputs:
  - product_service: "What you are selling"
  - icp_criteria: "Ideal customer profile definition"
  - prospecting_goal: "List building|Single account research|Contact identification"

optional_inputs:
  - target_industry: "Specific industries to focus on"
  - company_size: "Employee count range"
  - geography: "Target regions or markets"
  - persona: "Job titles and roles to target"
  - trigger_events: "Signals to prioritize (funding, hiring, news)"
  - competitors: "Competitors whose customers to target"
  - exclusion_list: "Companies or domains to exclude"
```

## Step-by-Step Workflow

### Phase 1: ICP Definition and Validation

**Step 1: ICP Criteria Documentation**
- Firmographic: Industry, company size, revenue stage, geography, business model
- Technographic: Current tools they use, technologies that indicate fit
- Behavioral: Buying signals (funding rounds, hiring plans), trigger events

**Step 2: ICP Validation**
- Cross-reference against 5-10 best existing customers
- Identify common patterns and attributes
- Rank criteria by predictive value
- Define minimum viable fit threshold

### Phase 2: Prospect Discovery

**Step 3: Company Discovery**

Search strategies:
- "[Industry] companies [location] [size range]"
- "[Competitor] customers alternatives"
- "[Technology] users companies"
- "Series B/C funding [industry] 2024"
- "[Job title] hiring [company type]"

Sources to mine:
- Crunchbase for funded companies
- LinkedIn for company and contact search
- G2/Capterra for technology users
- Industry directories and associations
- Conference and event attendee lists

**Step 4: Contact Identification**

Buying committee roles to find:
- Economic Buyer: Final budget authority
- Champion: Internal advocate for your solution
- User Buyer: Daily user of the product
- Technical Buyer: IT/security evaluator
- Gatekeeper: EA/coordinator managing access

### Phase 3: Account Intelligence Gathering

**Step 5: Account Deep-Dive**
1. Company overview and recent performance
2. Strategic initiatives and priorities
3. Technology stack from job postings and reviews
4. Key challenges from press, reviews, forums
5. Recent news and trigger events
6. Competitive landscape they face

**Step 6: Buying Signal Detection**

| Signal Type | What to Look For | Priority |
|------------|-----------------|----------|
| Funding | New funding round | High |
| Leadership | New C-suite hire | High |
| Growth | Rapid hiring in target dept | High |
| Expansion | New market or product launch | Medium |
| Pain Signal | Negative reviews of competitor | Medium |
| Content | Published content on your topic | Low |

### Phase 4: Outreach Personalization

**Step 7: Personalization Research**
- Recent post, article, or talk to reference
- Company news relevant to your solution
- Specific challenge they have mentioned
- Connection or shared experience
- Timing trigger that makes outreach relevant now

**Step 8: Outreach Brief Creation**
For each prospect:
- One-sentence personalization hook
- Relevant value proposition alignment
- Specific pain point to address
- Proposed next step and CTA
- Best channel for outreach (email/phone/LinkedIn)

## Output Templates

### Prospect List Template
```
# Prospect List: [Campaign Name]
Created: [Date] | ICP: [Brief description] | Goal: [Number]

## Tier 1 Prospects (Best Fit)
| Company | Contact | Title | Signal | Score |
|---------|---------|-------|--------|-------|

## Tier 2 Prospects (Good Fit)
| Company | Contact | Title | Signal | Score |
|---------|---------|-------|--------|-------|
```

### Individual Account Profile Template
```
# Account Profile: [Company Name]
Researched: [Date] | Tier: 1/2/3 | Owner: [Rep Name]

## Company Snapshot
- Industry: [Sector] | Size: [Employees] | Stage: [Startup/Growth/Enterprise]
- Website: [URL]

## Why They Fit Our ICP
- [Specific ICP criterion 1 and evidence]
- [Technology or behavior signal]

## Recent Intelligence
- [Most recent relevant news or development]
- [Known challenge or pain point]

## Buying Signals
- [Signal 1]: [Details and date]

## Key Contacts
### [Name] - [Title]
- Role in buying: [Economic/Champion/User/Technical]
- Background: [2-3 sentences]
- Outreach hook: [Personalization angle]

## Proposed Outreach
- Channel: [Email/Phone/LinkedIn]
- Subject: [Draft subject line]
- Hook: [Personalized first line]
- Value prop: [1-2 sentences tailored to their context]
- CTA: [Specific next step]
```

## Prospect Scoring Framework

```yaml
scoring_criteria:
  firmographic_fit:
    industry_match: 20 points
    size_match: 15 points
    geography_match: 10 points
  technographic_fit:
    complementary_tools: 15 points
    replaces_competitor_tool: 20 points
  behavioral_signals:
    recent_funding: 15 points
    leadership_change: 10 points
    active_hiring: 10 points
    content_engagement: 5 points
  scoring_tiers:
    tier_1: 70-100 points (immediate outreach)
    tier_2: 40-69 points (nurture sequence)
    tier_3: 20-39 points (monitor and revisit)
    disqualified: below 20 points
```

## Outreach Sequence Recommendations

### Cold Email Sequence (10 days)
- Day 1: Personalized cold email with value hook
- Day 3: Follow-up with relevant case study
- Day 5: LinkedIn connection request with note
- Day 7: Phone call attempt
- Day 10: Break-up email with resource offer

### LinkedIn-First Sequence (14 days)
- Day 1: Follow and engage with recent content
- Day 3: Connection request with personalized note
- Day 7: DM with specific value observation
- Day 10: Share relevant resource
- Day 14: Soft ask for conversation

## Perplexity-Specific Tips

- Search "[Company] challenges problems 2024" for pain point intelligence
- Use **Focus: News** to find recent trigger events
- Use **Pro Search** for deeper organizational research
- Search "[Company] hiring [department] jobs" as growth signal
- Use **Spaces** to organize research by account or territory
- Save prospect profiles for team sharing and CRM import

## Integration Points
- Export prospect lists to CRM (Salesforce, HubSpot, Pipedrive)
- Sync contact data to sales engagement tools (Outreach, Salesloft)
- Share account profiles with AE before discovery calls
- Feed trigger event alerts into Slack channels

## Compliance and Ethics
- Only use publicly available information for research
- Respect do-not-contact lists and opt-outs
- Follow CAN-SPAM and GDPR requirements for outreach
- Honor unsubscribe requests immediately

## Success Metrics
- Prospect list quality score (ICP fit percentage)
- Outreach open and reply rates
- Meeting conversion rate (contacts to demos)
- Pipeline generated from prospecting activities
- Time to build qualified prospect list (target: 70% reduction vs. manual)
- Win rate from prospected vs. inbound accounts
