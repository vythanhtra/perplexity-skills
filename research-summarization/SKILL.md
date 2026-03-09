# Skill: Research Summarization

## Overview
This skill enables Perplexity AI to rapidly synthesize large volumes of information from multiple sources into concise, structured, and actionable summaries tailored to specific audiences and purposes.

## Skill Metadata
- **Skill ID:** research-summarization
- **Category:** Knowledge Management & Research
- **Complexity:** Intermediate
- **Estimated Time:** 5-30 minutes depending on scope
- **Output Format:** Structured Summary Document (Markdown)

## Capabilities

### 1. Multi-Source Synthesis
- Aggregate information from web articles, papers, reports, and databases
- Cross-reference facts across multiple sources
- Identify consensus views vs. contested claims
- Highlight primary vs. secondary sources
- Flag information gaps and limitations

### 2. Audience-Adapted Summarization
- Executive summaries for leadership (300-500 words)
- Technical summaries for practitioners (detailed, jargon-inclusive)
- Layperson summaries for general audiences (simple language)
- Bullet-point briefings for quick consumption
- Narrative summaries for storytelling contexts

### 3. Structured Output Generation
- Key findings and takeaways
- Supporting evidence and data points
- Conflicting perspectives and nuances
- Implications and recommendations
- Source bibliography and credibility assessment

### 4. Domain-Specific Research
- Academic and scientific literature
- Market research and industry reports
- Legal and regulatory documents
- News and current events
- Technical documentation

### 5. Quality Assurance
- Source credibility scoring
- Recency assessment
- Bias identification
- Confidence level tagging
- Fact-check flagging

## Input Requirements

```yaml
required_inputs:
  - research_topic: "The subject to research and summarize"
  - audience: "Who will read this summary"
  - purpose: "Why this summary is needed"

optional_inputs:
  - scope: "Breadth and depth of coverage"
  - time_range: "How recent the sources should be"
  - length: "brief|standard|comprehensive"
  - format: "bullets|narrative|structured|executive"
  - focus_areas: "Specific aspects to emphasize"
  - output_language: "Language for the summary"
```

## Step-by-Step Workflow

### Phase 1: Scope Definition

**Step 1: Research Brief Creation**
- Define primary research question and sub-questions
- Set geographic or temporal scope
- Identify source type preferences
- Determine depth required and audience expertise level

**Step 2: Source Planning**
- Primary sources: Original research, official reports, data
- Secondary sources: Analysis, commentary, journalism
- Expert opinions: Interviews, podcasts, talks
- Quantitative data: Statistics, surveys, studies

### Phase 2: Information Gathering

**Step 3: Systematic Search**

Search query templates:
- "[Topic] overview 2024"
- "[Topic] research findings"
- "[Topic] expert opinion"
- "[Topic] statistics data"
- "[Topic] challenges implications"

**Step 4: Source Evaluation**

| Criteria | High Quality | Medium Quality | Low Quality |
|----------|-------------|----------------|-------------|
| Authority | Peer-reviewed, official | Industry reports | Anonymous blogs |
| Recency | Last 6 months | Last 2 years | Older than 3 years |
| Accuracy | Verified, cited | Generally accurate | Unverified claims |
| Bias | Neutral/disclosed | Minor bias | Strong agenda |

### Phase 3: Synthesis & Writing

**Step 5: Theme Identification**
- Cluster related information into themes
- Identify recurring points across sources
- Note divergent perspectives
- Prioritize by relevance to purpose

**Step 6: Hierarchical Organization**
1. Executive Summary (top-line findings)
2. Key Themes organized by importance
3. Supporting Data and Evidence
4. Conflicting Views if applicable
5. Implications and Recommendations
6. Sources and Credibility Notes

**Step 7: Writing for Audience**
- C-Suite: Lead with business impact, skip technical details
- Technical teams: Include methodology, data, and specifics
- General public: Define jargon, use analogies, tell stories
- Policy makers: Emphasize implications and action options
- Investors: Focus on opportunity, risk, and financial metrics

## Output Templates

### Executive Summary Template
```
# [Topic] Executive Summary
Prepared: [Date] | For: [Audience] | By: [Author]

## Bottom Line Up Front
[2-3 sentences on what you need to know and why it matters]

## Key Findings
1. [Finding 1]: [One sentence with supporting data]
2. [Finding 2]: [One sentence with supporting data]
3. [Finding 3]: [One sentence with supporting data]

## Implications
- Short-term: [Immediate actions or impacts]
- Long-term: [Strategic considerations]

## Recommended Actions
1. [Action 1]
2. [Action 2]

## Sources
[List of key sources used]
```

### Comprehensive Research Summary Template
```
# Research Summary: [Topic]
Scope: [Geographic/Temporal scope]
Date Range: [Coverage period]
Sources Reviewed: [Number and types]

## Executive Overview
[150-200 word summary]

## Background and Context
[Why this topic matters, historical context]

## Key Themes and Findings

### Theme 1: [Title]
Summary: [2-3 sentence overview]
Evidence:
- [Data point or finding]
- [Supporting example]
- [Expert quote or opinion]
Confidence Level: High/Medium/Low

## Data and Statistics
| Metric | Value | Source | Date |
|--------|-------|--------|------|

## Contrasting Perspectives
Mainstream View: [Summary]
Alternative View: [Summary]
Why it matters: [Implication of the disagreement]

## Gaps and Limitations
- [Information not found or unavailable]
- [Areas needing further research]

## Implications and Recommendations
- [Recommendation 1]
- [Recommendation 2]

## Source Bibliography
| Source | Type | Credibility | Date |
|--------|------|------------|------|
```

## Quality Checklist
- All key claims are supported by at least one source
- Sources are recent within required time range
- Multiple perspectives are represented
- Bias has been identified and noted
- Technical terms are defined for target audience
- Summary length matches requested format
- Confidence levels are assigned to uncertain claims
- Recommendations follow logically from findings

## Domain-Specific Adaptations

### Scientific/Academic Research
- Prioritize peer-reviewed sources
- Include study methodology and sample sizes
- Note statistical significance
- Distinguish correlation from causation

### Market and Industry Research
- Include market size and growth data
- Identify key players and market share
- Note analyst ratings and forecasts
- Highlight investment signals

### Legal and Regulatory Research
- Cite specific laws, regulations, and rulings
- Note jurisdiction and applicability
- Highlight compliance requirements
- Flag areas of legal uncertainty

### News and Current Events
- Prioritize recency (last 24-72 hours)
- Cross-reference across multiple outlets
- Track story evolution over time

## Perplexity-Specific Tips

- Use **Focus: Academic** for scholarly sources and research papers
- Use **Focus: News** for current events and breaking developments
- Enable **Pro Search** for comprehensive multi-source synthesis
- Use **Follow-up questions** to explore specific themes deeper
- Leverage **Spaces** to organize ongoing research projects
- Use date filters to control recency of sources
- Request citations explicitly for verifiable output

## Automation Use Cases

```yaml
recurring_summaries:
  daily:
    - Industry news digest
    - Competitor monitoring brief
  weekly:
    - Market intelligence summary
    - Regulatory update briefing
    - Research paper highlights
  monthly:
    - Industry landscape report
    - Technology trend analysis
  on_demand:
    - Due diligence research
    - Topic deep-dives
    - Crisis information gathering
```

## Success Metrics
- Accuracy rate (fact-checked against sources)
- Reader satisfaction score (audience feedback)
- Time saved vs. manual research (target: 75% reduction)
- Source diversity index (variety of source types)
- Summary utility rate (percentage acted upon)
- Completeness score (key topics covered)
