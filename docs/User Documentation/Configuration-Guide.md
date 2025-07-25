# Configuration Guide

This guide covers all configuration options for Agile Chart Toolbelt gadgets, helping you customize analytics for your team's needs.

## Sankey Diagram Configuration

### Data Source Types

#### Board & Sprint Analysis
**Best for**: Traditional Scrum teams with defined sprints

```yaml
Configuration:
  Data Source: Board & Sprint
  Board: [Select from your accessible boards]
  Sprint Selection: Dynamic (in view)
```

**Use Cases**:
- Sprint retrospectives and planning
- Individual sprint performance analysis
- Sprint-to-sprint comparison
- Scope change tracking within sprints

#### Project-Based Analysis
**Best for**: Product teams tracking features across multiple sprints

```yaml
Configuration:
  Data Source: Project (Last 90 Days)
  Project: [Select from your accessible projects]
  Sprint Selection: Dynamic (filtered to project issues)
```

**Use Cases**:
- Cross-sprint feature analysis
- Product roadmap progress tracking
- Multi-team project coordination
- Long-term scope trend analysis

### Advanced Configuration Options

#### Time Range Settings
```yaml
Project Analysis:
  Time Window: 90 days (fixed)
  Issue Filter: Updated within timeframe
  Sprint Filter: Sprints containing project issues
```

#### Data Filtering
- **Automatic Filtering**: Issues assigned to selected sprints
- **Status Mapping**: Automatic mapping of Jira statuses to flow categories
- **Story Point Requirements**: Issues without story points are excluded from flow calculations

## Sprint Reliability Configuration

### Basic Setup

```yaml
Required Fields:
  Board: [Scrum board with story point tracking]
  Sprint Count: 5-20 sprints (recommended: 10)
  
Optional Fields:
  Date Range: Auto-calculated from sprint count
  Team Filter: All team members (default)
```

### Reliability Calculation Settings

#### Story Point Sources
The app automatically detects story points from:
1. **Story Points field**

#### Commitment Detection
```yaml
Commitment Logic:
  Sprint Start: Issues in sprint at start date
  Sprint End: Issues completed by end date
  Calculation: (Completed Points / Committed Points) × 100
```

### Advanced Reliability Options

## Dashboard Integration


### Multi-Dashboard Strategy

#### Team Dashboard
```yaml
Focus: Operational metrics
Gadgets:
  - Current sprint Sankey diagram
  - 5-sprint reliability tracker
  - Sprint burndown
  - Team velocity
```

#### Leadership Dashboard
```yaml
Focus: Trends and outcomes
Gadgets:
  - Project-based Sankey analysis
  - 10-sprint reliability trends
  - Cross-team comparisons
  - Quarterly summaries
```

### Security Considerations

#### Data Privacy
- **No Data Storage**: App doesn't store sensitive issue data
- **Real-time Queries**: Data fetched fresh from Jira APIs
- **User Context**: Respects individual user permissions

#### Compliance
- **GDPR Compliant**: No personal data retention
- **SOC 2**: Inherits Atlassian security standards
- **Audit Trail**: Configuration changes logged

### Common Issues

#### "No Data Available"
**Causes & Solutions**:
```yaml
Issue: Empty sprint or project
Solution: Verify sprint contains issues with story points

Issue: Permission denied
Solution: Check project/board access permissions

Issue: Invalid configuration
Solution: Reconfigure with valid board/project selection
```

---

**Need Help with Configuration?**

- 📧 Email: support@conwavelabs.com
- 📚 Detailed Guides: [Feature Documentation](Home.md#features)
- 🔧 Troubleshooting: [Common Issues](Troubleshooting.md)

[← Back to Getting Started](Getting-Started.md) | [Next: Sankey Overview →](Sankey-Diagram-Overview.md)

---
*Last Updated: July 2025*
