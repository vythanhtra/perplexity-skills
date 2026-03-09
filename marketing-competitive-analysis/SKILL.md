# Skill: Marketing Competitive Analysis

## Overview
This skill enables Perplexity AI to conduct comprehensive competitive intelligence research, analyze market positioning, and generate actionable insights to support marketing strategy and sales enablement.

## Skill Metadata
- **Skill ID:** marketing-competitive-analysis
- **Category:** Marketing & Strategy
- **Complexity:** Advanced
- **Estimated Time:** 15-45 minutes per competitor
- **Output Format:** Structured Markdown Report + Battlecard

## Capabilities

### 1. Competitor Profiling
- Company overview, funding, team size, and growth trajectory
- Product/service offerings and feature comparison
- Target customer segments and use cases
- Pricing model and packaging analysis
- Geographic presence and market focus

### 2. Market Positioning Analysis
- Brand messaging and value proposition
- Marketing channels and content strategy
- Share of voice and SEO keyword analysis
- Customer reviews and sentiment (G2, Capterra, Trustpilot)
- Awards, certifications, and analyst recognition

### 3. SWOT Intelligence
- Strengths based on customer feedback and product capabilities
- Weaknesses from complaint patterns and feature gaps
- Opportunities from market trends and unmet needs
- Threats from competitor roadmap signals and partnerships

### 4. Sales Battlecard Generation
- Head-to-head feature comparison table
- Objection handling scripts
- Win/loss themes and patterns
- Recommended talk tracks for sales team

### 5. Trend Monitoring
- Recent news, press releases, and announcements
- Job postings as signals of strategic direction
- Patent filings and technology investments
- Partnership and integration announcements

## Input Requirements

```yaml
required_inputs:
  - competitor_name: "Name of the competitor company"
  - your_company: "Your company name and product"
  - analysis_depth: "quick|standard|deep"

optional_inputs:
  - specific_products: "Specific product lines to focus on"
  - target_segment: "Customer segment for comparison"
  - geographic_focus: "Region or market to analyze"
  - time_range: "Recency of information needed"
  - output_format: "report|battlecard|both"
```

## Step-by-Step Workflow

### Phase 1: Data Collection (Automated Research)

**Step 1: Company Intelligence Gathering**
```
Search queries to run:
- "[Competitor] company overview funding employees"
- "[Competitor] product features pricing 2024"
- "[Competitor] target customers use cases"
- "[Competitor] vs [Your Company] comparison"
- "[Competitor] news announcements partnerships"
```

**Step 2: Customer Voice Research**
```
Platforms to analyze:
- G2 Reviews: ratings, pros/cons, top use cases
- Capterra: user demographics, feature ratings
- Trustpilot: sentiment trends over time
- Reddit/communities: authentic user discussions
- LinkedIn comments: professional perspective
```

**Step 3: Digital Presence Analysis**
```
Channels to assess:
- Website: messaging, CTAs, positioning changes
- Blog/Content: topics, frequency, SEO focus
- Social media: engagement, tone, campaigns
- Paid ads: messaging themes (via ad libraries)
- Job postings: team growth signals
```

### Phase 2: Analysis & Synthesis

**Step 4: Feature Matrix Construction**

| Feature Category | Your Product | Competitor | Advantage |
|-----------------|-------------|------------|----------|
| Core Feature A | Yes | Yes | Tie |
| Core Feature B | Yes | No | Ours |
| Core Feature C | No | Yes | Theirs |
| Integration X | Yes | No | Ours |

**Step 5: Positioning Mapping**
- Plot on axes: Price vs. Value, Ease vs. Power, etc.
- Identify white space opportunities
- Note messaging overlap and differentiation

**Step 6: Win/Loss Pattern Analysis**
- Reasons customers choose competitor over you
- Reasons customers choose you over competitor
- Customer segments where you win/lose most

### Phase 3: Battlecard & Report Generation

**Step 7: Executive Summary**
- One-paragraph competitor snapshot
- Top 3 threats they pose
- Top 3 opportunities to exploit

**Step 8: Sales Battlecard Assembly**

### Battlecard Structure

**Header:** Competitor name, last updated date, competitive win rate

**Quick Overview:** What they do, target customer, pricing model, key recent developments

**Strengths (Be Honest):** Where they genuinely compete well, what customers like (from reviews)

**Weaknesses:** Consistent customer complaints, technical limitations, gaps in offering

**Our Differentiators:** 3-5 specific ways your product or approach is different

**Objection Handling:**

| If the prospect says... | Respond with... |
|---|---|
| "[Competitor] does X too" | "Here is how our approach differs..." |
| "[Competitor] is cheaper" | "Here is what that price difference gets you..." |

**Win/Loss Themes:**
- Common reasons deals are won against this competitor
- Common reasons deals are lost to this competitor

### Best Practices

**Data Quality:**
- Prioritize recent sources (last 6-12 months)
- Cross-reference claims across multiple sources
- Label speculation vs. confirmed information
- Note confidence levels for uncertain data

**Ethical Guidelines:**
- Only use publicly available information
- Do not misrepresent competitor capabilities
- Be honest about your own weaknesses
- Update battlecards quarterly or after major releases

**Bias Prevention:**
- Actively seek out positive competitor reviews
- Include genuine strengths, not just weaknesses
- Have sales team validate win/loss themes
- Test objection responses with real customers

## Output Templates

### Quick Snapshot (15 min)
```markdown
## [Competitor] Quick Snapshot
**Updated:** [Date]
**Tier:** Primary/Secondary/Emerging

### Who They Are
[2-3 sentences]

### Their Best Use Case
[1-2 sentences]

### Our Key Advantage
[1-2 sentences]

### Watch Out For
[1-2 sentences]
```

### Full Competitive Report (45 min)
- Executive Summary (1 page)
- Company Profile & Funding History
- Product Feature Deep-Dive
- Pricing Analysis
- Customer Sentiment Summary
- Marketing & Positioning Analysis
- SWOT Analysis
- Strategic Recommendations
- Appendix: Raw Data Sources

## Perplexity-Specific Tips

- Use **Follow-up questions** to drill deeper into specific areas
- Enable **Pro Search** for more comprehensive web coverage
- Use **Focus: Web** for latest news, **Focus: Academic** for market research
- Save and export reports directly from Perplexity interface
- Set up **Spaces** to organize ongoing competitive monitoring
- Use date filters to ensure information recency

## Automation Opportunities

```yaml
recurring_tasks:
  weekly:
    - Monitor competitor news and announcements
    - Check for new product updates or releases
    - Track review score changes
  
  monthly:
    - Update pricing information
    - Refresh battlecards with new win/loss data
    - Analyze competitor content strategy changes
  
  quarterly:
    - Full competitive landscape refresh
    - Update feature comparison matrix
    - Present findings to sales and marketing teams
```

## Integration Points
- Export to CRM (Salesforce, HubSpot) as battlecard attachments
- Share via Slack to sales channels before key deals
- Embed in sales playbooks and onboarding materials
- Link from proposal templates for relevant competitors

## Success Metrics
- Competitive win rate improvement over baseline
- Sales team battlecard utilization rate
- Time saved vs. manual research (target: 70% reduction)
- Accuracy of competitive intelligence (validated by sales)
- Frequency of battlecard updates (target: quarterly minimum)
