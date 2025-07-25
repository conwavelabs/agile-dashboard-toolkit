# Getting Started Tutorial

Welcome! This tutorial will walk you through creating your first sprint analysis using Agile Chart Toolbelt.

## Tutorial Overview

In this 10-minute tutorial, you'll:
1. ✅ Add your first Sankey diagram
2. ✅ Configure it for your board/project
3. ✅ Understand the visualization
4. ✅ Add a Sprint Reliability tracker

## Step 1: Add a Sankey Diagram

### Create the Gadget

1. **Navigate to Dashboard**
   - Go to any Jira dashboard
   - Click **Add gadget** (+ icon)

2. **Select Sankey Diagram**
   - Search for "Sprint Sankey"
   - Click **Sprint Sankey Diagram**
   - Click **Add gadget**

### Configure Your First Diagram

1. **Choose Data Source**
   ```
   Data Source: Board & Sprint
   ```

2. **Select Your Board**
   - Choose an active Scrum board from the dropdown
   - Pick one with recently completed sprints

3. **Save Configuration**
   - Click **Save Configuration**
   - The gadget will load your sprint data

## Step 2: Understanding Your Sankey Diagram

### Reading the Flow

Your Sankey diagram shows how work flows through your sprint:

```
Original Scope ──┐
                 ├─→ Completed ✅
Added Scope ──────┤
                 ├─→ Incomplete ⏳
                 └─→ Removed ❌
```

### Key Insights

**Flow Width = Story Points**
- Thicker flows = more story points
- Hover over flows to see exact numbers

### Dynamic Sprint Selection

**Switch Between Sprints**
- Use the dropdown at the top of the gadget
- Compare different sprints instantly
- No reconfiguration needed!

## Step 3: Add Sprint Reliability Tracking

### Create Reliability Gadget

1. **Add Second Gadget**
   - Click **Add gadget** again
   - Select **Sprint Reliability Tracker**

2. **Configure Reliability Tracking**
   ```
   Board: [Same board as Sankey diagram]
   Sprint Count: 10 (last 10 sprints)
   ```

3. **Save and View**
   - Your reliability trends will appear
   - Shows committed vs. delivered story points

### Understanding Reliability Metrics

**Reliability Score**
```
Reliability = (Delivered Points / Committed Points) × 100%
```

**Trend Analysis**
- 📈 **Upward Trend**: Improving reliability
- 📉 **Downward Trend**: Declining reliability
- ➡️ **Flat Trend**: Consistency

## Step 4: Explore Advanced Features

### Project-Based Analysis

Try the project data source:

1. **Edit Sankey Gadget**
   - Click the gadget's edit button
   - Change **Data Source** to "Project (Last 90 Days)"

2. **Select Project**
   - Choose your project from dropdown
   - Save configuration

3. **Multi-Sprint View**
   - See all sprints containing project issues
   - Analyze project scope across multiple sprints


## Common Use Cases

### For Scrum Masters

**Sprint Retrospectives**
- Show scope change patterns
- Discuss commitment accuracy
- Identify improvement areas

**Sprint Planning**
- Review historical reliability
- Set realistic commitments
- Plan capacity allocation

### For Product Owners

**Scope Management**
- Track scope creep trends
- Understand feature completion rates
- Make data-driven priority decisions

### for Development Teams

**Performance Insights**
- Visualize sprint outcomes
- Understand workflow bottlenecks
- Celebrate completion successes

## Next Steps

Now that you've created your first analytics:

1. **📊 Deep Dive**: [Sankey Diagram Overview](Sankey-Diagram-Overview.md)
2. **📈 Advanced Config**: [Configuration Guide](Configuration-Guide.md)
3. **� Best Practices**: [Best Practices](Best-Practices.md)

## Quick Reference

### Keyboard Shortcuts
- **Refresh Data**: Click gadget refresh icon
- **Edit Config**: Click gadget settings (⚙️)
- **Full Screen**: Click expand icon (⛶)

### Common Actions
| Action | Location | Purpose |
|--------|----------|---------|
| Change Sprint | Top dropdown | Switch sprint analysis |
| Edit Config | Gadget settings | Modify data source |
| Export Data | Coming soon | Download insights |

---

**Congratulations!** 🎉

You've successfully set up your first sprint analytics dashboard. Your team now has powerful insights into sprint performance and scope management.

[← Back to Installation](Installation.md) | [Next: Configuration Guide →](Configuration-Guide.md)

---
*Last Updated: July 2025*
