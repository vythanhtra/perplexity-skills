---
name: data-exploration
description: Profile and explore datasets to understand their shape, quality, and patterns before analysis. Use when encountering a new dataset, assessing data quality, discovering column distributions, identifying nulls and outliers, or deciding which dimensions to analyze.
author: Perplexity
version: '1.0'
---

# Data Exploration Skill

Systematic methodology for profiling datasets, assessing data quality, discovering patterns, and understanding schemas.

## Data Profiling Methodology

### Phase 1: Structural Understanding

Before analyzing any data, understand its structure:

**Table-level questions:**
- How many rows and columns?
- What is the grain (one row per what)?
- What is the primary key? Is it unique?
- When was the data last updated?
- How far back does the data go?

**Column classification:**
- **Identifier**: Unique keys, foreign keys, entity IDs
- **Dimension**: Categorical attributes for grouping/filtering
- **Metric**: Quantitative values for measurement
- **Temporal**: Dates and timestamps
- **Text**: Free-form text fields
- **Boolean**: True/false flags
- **Structural**: JSON, arrays, nested structures

### Phase 2: Column-Level Profiling

For each column, compute:

**All columns:**
- Null count and null rate
- Distinct count and cardinality ratio
- Most common values (top 5-10 with frequencies)
- Least common values (bottom 5 to spot anomalies)

**Numeric columns:**
- min, max, mean, median (p50)
- standard deviation
- percentiles: p1, p5, p25, p75, p95, p99
- zero count, negative count

**String columns:**
- min length, max length, avg length
- empty string count
- pattern analysis, case consistency

**Date/timestamp columns:**
- min date, max date, null dates
- future dates (if unexpected)
- distribution by month/week, gaps in time series

### Phase 3: Relationship Discovery

- **Foreign key candidates**: ID columns that might link to other tables
- **Hierarchies**: Columns that form natural drill-down paths
- **Correlations**: Numeric columns that move together
- **Derived columns**: Columns that appear to be computed from others
- **Redundant columns**: Columns with identical or near-identical information

## Quality Assessment Framework

### Completeness Score

- **Complete** (>99% non-null): Green
- **Mostly complete** (95-99%): Yellow - investigate the nulls
- **Incomplete** (80-95%): Orange - understand why
- **Sparse** (<80%): Red - may not be usable without imputation

### Consistency Checks

- Value format inconsistency ("USA", "US", "United States")
- Type inconsistency: Numbers stored as strings, dates in various formats
- Business rule violations: Negative quantities, end dates before start dates
- Cross-column consistency: Status = "completed" but completed_at is null

### Accuracy Indicators

Red flags:
- Placeholder values: 0, -1, 999999, "N/A", "TBD", "test"
- Default values: Suspiciously high frequency of a single value
- Stale data: Updated_at shows no recent changes
- Impossible values: Ages > 150, dates in the far future

## Pattern Discovery

### Distribution Analysis

- **Normal**: Mean and median are close, bell-shaped
- **Skewed right**: Long tail of high values (common for revenue)
- **Power law**: Few very large values, many small ones
- **Bimodal**: Two peaks (suggests two distinct populations)

### Temporal Patterns

- Trend, seasonality, day-of-week effects, holiday effects
- Change points: Sudden shifts in level or trend
- Anomalies: Individual data points that break the pattern

## Schema Documentation Template

```
## Table: [schema.table_name]

**Description**: [What this table represents]
**Grain**: [One row per...]
**Primary Key**: [column(s)]
**Row Count**: [approximate, with date]
**Update Frequency**: [real-time / hourly / daily / weekly]

### Key Columns

| Column | Type | Description | Example Values | Notes |
|--------|------|-------------|----------------|-------|
| user_id | STRING | Unique user identifier | "usr_abc123" | FK to users.id |

### Known Issues
- [List any known data quality issues]
```
