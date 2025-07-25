# Sankey Diagram Overview

Sprint Sankey diagrams provide powerful visual insights into how work flows through your sprints, revealing patterns in scope changes and completion rates.

## What is a Sprint Sankey Diagram?

### Visual Representation
A Sankey diagram shows the flow of work from **sources** (where work comes from) to **destinations** (where work ends up) with flow thickness representing story points.

```
Sprint Flow Visualization:

Original Scope ──────┐
    (30 pts)         │
                     ├─→ Completed (25 pts) ✅
Added Scope ──────┐  │
    (10 pts)      │  ├─→ Incomplete (10 pts) ⏳
                  │  │
                  └──┴─→ Removed (5 pts) ❌
```

### Flow Categories

#### Sources (Left Side)
**Original Scope**
- Issues committed at sprint start
- Planned work from sprint planning
- Baseline scope for comparison

**Added Scope**
- Issues added during sprint
- Scope creep or urgent requests
- Mid-sprint priority changes

#### Destinations (Right Side)
**Completed**
- Issues finished by sprint end
- Moved to "Done" status
- Successfully delivered value

**Incomplete**
- Issues not finished by sprint end
- Carried over to next sprint
- Work in progress at sprint close

**Removed**
- Issues removed from sprint
- Descoped or deprioritized work
- Scope reduction decisions

## Interactive Features

### Dynamic Sprint Selection

**Sprint Dropdown**
- Switch between any available sprints
- No reconfiguration required
- Instant visual updates
- Compare sprint patterns easily

**Sprint Information Display**
```
Sprint Navigation:
┌─────────────────────────────────────┐
│ 🎯 Sprint 23 (Closed) ▼            │
│    22 issues • 89 story points     │
└─────────────────────────────────────┘
```

### Hover Interactions

**Flow Details**
Hover over any flow to see:
- Exact story point values
- Issue count breakdown
- Percentage of total scope
- Trend comparison data

**Node Information**
Hover over source/destination nodes:
- Total story points in category
- Issue distribution
- Status breakdown
- Time-based metrics

### Visual Customization

#### Color Scheme
```yaml
Flow Colors:
  Completed Flows: Green spectrum (#4CAF50)
  Incomplete Flows: Orange spectrum (#FF9800)
  Removed Flows: Red spectrum (#F44336)
  
Node Colors:
  Source Nodes: Blue (#2196F3)
  Destination Nodes: Grey (#757575)
```

#### Responsive Design
- **Desktop**: Full-width visualization
- **Tablet**: Condensed layout
- **Mobile**: Simplified view

## Analysis Techniques

### Sprint Retrospective Analysis

#### Questions to Explore
1. **Scope Management**
   - "How much scope was added during the sprint?"
   - "What percentage of original scope was completed?"
   - "Were scope removals strategic or reactive?"

2. **Team Performance**
   - "Did we complete work efficiently?"
   - "What caused incomplete items?"
   - "How predictable was our delivery?"

3. **Process Improvement**
   - "What patterns do we see across sprints?"
   - "Are we improving commitment accuracy?"
   - "How can we reduce scope volatility?"

### Trend Analysis

#### Multi-Sprint Comparison
Use dynamic sprint selection to compare:
- **Consecutive Sprints**: Identify improvement trends
- **Similar Sprints**: Compare sprints with similar scope
- **Seasonal Patterns**: Analyze quarterly or release cycles

## Best Practices

### Configuration Recommendations

#### Board-Based Analysis
```yaml
Best For:
  - Single team analysis
  - Sprint-focused retrospectives
  - Operational team metrics
  
Configuration:
  - Select primary team board
  - Use with Sprint Reliability tracker
  - Focus on recent sprints
```

### Action Items from Analysis

#### High Scope Additions
**Root Cause Analysis**:
- Changing requirements
- External pressures
- Inadequate refinement

**Improvement Actions**:
- Enhance sprint planning
- Implement change control
- Improve stakeholder communication
- Strengthen definition of ready
---

**Master Your Sprint Analysis** 📊

Sankey diagrams provide unparalleled insights into sprint dynamics. Use them regularly to drive continuous improvement and data-driven decision making.

[← Back to Configuration](Configuration-Guide.md) | [Next: Best Practices →](Best-Practices.md)

---
*Last Updated: July 2025*
