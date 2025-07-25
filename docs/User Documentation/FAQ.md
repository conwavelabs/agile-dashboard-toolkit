# Frequently Asked Questions (FAQ)

Find quick answers to common questions about Agile Chart Toolbelt features, configuration, and usage.

## General Questions

### What is Agile Chart Toolbelt?
Agile Chart Toolbelt is an Atlassian Forge application that provides advanced sprint analytics through Sankey diagrams and Sprint Reliability tracking. It helps agile teams visualize sprint scope changes, completion flows, and reliability trends.

### Which Jira versions are supported?
- **Jira Software Cloud**: All current versions

### Is my data safe?
Yes! The app:
- Runs on Atlassian's secure Forge platform
- Never stores sensitive issue data
- Respects all Jira permissions
- Processes data in real-time without external transmission
- Is GDPR compliant

## Installation and Setup

### How do I install the app?
1. Go to **Jira Settings** → **Apps** → **Find new apps**
2. Search for "Agile Chart Toolbelt"
3. Click **Install** and accept permissions
4. Add gadgets to your dashboard

### Why can't I see the app in the marketplace?
Common causes:
- **Permissions**: You need Site Administrator access
- **Jira Version**: Requires Jira Software 8.0+
- **Browser**: Clear cache and try again
- **Region**: Try accessing from different marketplace region

### What permissions does the app need?
The app requires:
- **Project Browse**: To access project and issue data
- **Board Access**: To view sprint information
- **Dashboard Edit**: To add and configure gadgets
- **Sprint View**: To access agile board data

## Feature Questions

### What's the difference between Sankey diagrams and Sprint Reliability?

**Sankey Diagrams**:
- Show flow of work through individual sprints
- Visualize scope changes (original, added, completed, incomplete, removed)
- Best for sprint retrospectives and scope analysis

**Sprint Reliability**:
- Track commitment accuracy over multiple sprints
- Show trends in delivery predictability
- Best for planning and forecasting improvement

### Can I analyze multiple teams at once?
Not directly. The app is designed for single-team analysis. For multi-team insights:
- Create separate dashboards for each team
- Use project-based analysis for cross-team projects
- Compare team dashboards side-by-side

### How far back can I analyze sprint data?
- **Sankey Diagrams**: Any completed sprint (no time limit)
- **Sprint Reliability**: Up to 20 sprints recommended
- **Project Analysis**: Fixed 90-day window
- **Performance**: Best with recent sprints (<6 months)

## Configuration Questions

### Why do I see "No Data Available"?
Common causes and solutions:

**Empty Sprints**:
- Select sprints that contain completed issues
- Ensure issues have story points assigned

**Permission Issues**:
- Verify project browse permissions
- Check board access rights
- Test with a different user account

**Configuration Errors**:
- Reconfigure with valid board/project
- Try a different data source option

### How do I switch between sprints?
Use the **dynamic sprint dropdown** at the top of Sankey gadgets:
- No reconfiguration needed
- Instant switching between available sprints
- Works for both board and project data sources

### What if my team doesn't use story points?
The app requires story points for calculations. Options:
- **Add Story Points**: Assign story points to issues
- **Use Estimates**: Configure alternative estimation field
- **Historical Assignment**: Add story points to past issues for analysis

### Can I customize the colors or appearance?
Currently, the app uses a fixed color scheme optimized for accessibility:
- **Green**: Completed work
- **Orange**: Incomplete work  
- **Red**: Removed work
- **Blue**: Source categories

Custom themes are planned for future releases.

## Data and Calculations

### How does the app determine "Original Scope" vs "Added Scope"?
**Original Scope**: Issues assigned to sprint at sprint start date
**Added Scope**: Issues assigned to sprint after sprint start date

The app analyzes issue change history to determine when issues were added to sprints.

### How is Sprint Reliability calculated?
```
Sprint Reliability = (Completed Story Points / Committed Story Points) × 100%

Where:
- Committed Points = Points assigned at sprint start
- Completed Points = Points finished by sprint end
```

### Why don't my reliability numbers match manual calculations?
Common discrepancies:
- **Story Point Changes**: Mid-sprint story point updates
- **Issue Movements**: Issues moved between sprints
- **Status Timing**: Status changes outside sprint boundaries
- **Field Mapping**: Different story point field used

### What happens if issues are moved between sprints?
- **Sankey Diagrams**: Shows flow based on final sprint assignment
- **Reliability**: Uses sprint assignment at calculation time
- **History**: Tracks when issues were added/removed from sprints

## Performance and Limits

### How much data can the app handle?
**Recommended Limits**:
- Issues per sprint: <500
- Sprint count for reliability: <20
- Concurrent users: <100 per instance
- Project analysis: 90-day window only

**Performance Impact**:
- Large sprints may load slowly
- Consider filtering to specific components
- Use board-based vs project-based for better performance

### Why is the app loading slowly?
Performance optimization steps:
1. **Reduce Scope**: Limit sprint count or date range
2. **Check Jira**: Verify overall Jira performance
3. **Browser**: Clear cache, close tabs, try different browser
4. **Data Volume**: Use smaller sprints or recent data only

### Can I export the data?
Export functionality is coming in a future release. Currently:
- Take screenshots for presentations
- Use browser print to PDF
- Manually record key metrics

## Integration Questions

### Can I use it with Confluence?
Not directly. The app is designed for Jira dashboards. You can:
- Screenshot charts for Confluence pages
- Create dashboard links in Confluence
- Use Jira gadgets in Confluence pages (if supported)

### Does it support Jira Service Management?
No. The app requires Jira Software's agile features:
- Sprint functionality
- Story point estimation
- Agile boards
- Sprint reports

## Troubleshooting

### The gadget appears blank or shows errors
Quick fixes:
1. **Refresh**: Reload the page
2. **Reconfigure**: Edit gadget settings
3. **Permissions**: Check project access
4. **Browser**: Try incognito mode
5. **Data**: Verify sprint has story points

### Issues aren't showing in the correct categories
Verification steps:
1. Check issue change history in Jira
2. Verify sprint assignment dates
3. Review status transition timing
4. Confirm story point assignments

### Multiple users can't see the gadgets
Dashboard sharing checklist:
- Dashboard permissions configured
- Project access granted to all users
- Board visibility set appropriately
- App permissions accepted

## Best Practices

### How often should I review sprint analytics?
**Recommended Frequency**:
- **Sprint Retrospectives**: Every sprint (Sankey analysis)
- **Sprint Planning**: Every sprint (reliability trends)
- **Monthly Reviews**: Team performance trends
- **Quarterly**: Strategic process improvements

### How do I improve sprint reliability?
**Common Strategies**:
1. **Better Estimation**: Use planning poker, historical data
2. **Scope Protection**: Implement change control process
3. **Capacity Planning**: Account for meetings, support work
4. **Definition of Ready**: Ensure stories are ready for sprint

## Pricing and Licensing

### How much does the app cost?
Pricing information is available on the Atlassian Marketplace listing. The app typically follows Atlassian's tiered pricing model based on user count.

### Is there a free trial?
Yes! Most Atlassian Marketplace apps offer a free trial period. Check the marketplace listing for current trial terms.

### What happens if I uninstall the app?
- All configuration data is removed
- No residual data remains in your Jira instance
- You can reinstall anytime without data loss concerns
- Screenshots and exports remain available

---

**Still have questions?** 📧

- **Email**: support@conwavelabs.com
- **GitHub**: [Issues & Discussions](https://github.com/conwavelabs/agile-dashboard-toolkit)
- **Documentation**: [Full User Guide](Home.md)

[← Back to Troubleshooting](Troubleshooting.md) | [Next: Best Practices →](Best-Practices.md)

---
*Last Updated: July 2025*
