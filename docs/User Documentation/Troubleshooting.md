# Troubleshooting Guide

This guide helps you resolve common issues with Agile Chart Toolbelt and optimize its performance.

## Common Issues and Solutions

### Installation Problems

#### App Not Visible in Marketplace
**Symptoms**: Cannot find "Agile Chart Toolbelt" in Atlassian Marketplace

**Causes & Solutions**:
```yaml
Cause: Insufficient permissions
Solution: 
  - Verify Site Administrator access
  - Contact your Jira administrator
  - Check marketplace access permissions

Cause: Unsupported Jira version
Solution:
  - Verify Jira Software 8.0+ requirement
  - Update Jira instance if needed
  - Check version compatibility matrix

Cause: Regional marketplace restrictions
Solution:
  - Try different marketplace region
  - Contact Atlassian support
  - Use direct installation link
```

#### Gadgets Not Appearing After Installation
**Symptoms**: App installed but gadgets missing from dashboard

**Solutions**:
1. **Clear Browser Cache**
   ```
   Chrome: Ctrl+Shift+Delete
   Firefox: Ctrl+Shift+Delete
   Safari: Cmd+Option+E
   ```

2. **Verify App Status**
   - Go to **Jira Settings** → **Apps** → **Manage apps**
   - Ensure "Agile Chart Toolbelt" shows **Enabled**
   - Click **Refresh** if status unclear

3. **Check Browser JavaScript**
   - Ensure JavaScript is enabled
   - Disable ad blockers temporarily
   - Try incognito/private browsing mode

### Configuration Issues

#### "No Data Available" Error
**Symptoms**: Gadget displays but shows no data

**Diagnostic Steps**:
```yaml
Step 1: Verify Data Source
  - Check board/project selection
  - Ensure sprints exist and are completed
  - Verify issues have story points assigned

Step 2: Check Permissions
  - Confirm project browse permissions
  - Verify board access rights
  - Test with different user account

Step 3: Validate Configuration
  - Reconfigure gadget with known good data
  - Test with recently completed sprint
  - Try different board/project selection
```

**Common Solutions**:
```yaml
Issue: Empty sprint selected
Solution: Choose sprint with completed issues

Issue: No story points on issues
Solution: Assign story points to sprint issues

Issue: Permission denied
Solution: Grant project browse permissions

Issue: Invalid board selection
Solution: Select active Scrum board
```

#### Sankey Diagram Not Loading
**Symptoms**: Spinner continues indefinitely, no visualization appears

**Solutions**:
1. **Check Data Volume**
   ```yaml
   Recommended Limits:
     - Issues per sprint: <500
     - Story points per sprint: <1000
     - Sprint age: <6 months old
   ```

2. **Verify Sprint Status**
   ```yaml
   Required Conditions:
     - Sprint is in "Closed" state
     - Sprint has start and end dates
     - Sprint contains completed issues
   ```

3. **Browser Compatibility**
   ```yaml
   Supported Browsers:
     - Chrome 90+
     - Firefox 88+
     - Safari 14+
     - Edge 90+
   ```

#### Sprint Reliability Shows Incorrect Data
**Symptoms**: Reliability percentages don't match manual calculations

**Validation Steps**:
```yaml
Step 1: Story Point Verification
  - Check story point field mapping
  - Verify sprint commitment timing
  - Confirm completion criteria

Step 2: Sprint Boundary Check
  - Validate sprint start/end dates
  - Review issue sprint assignments
  - Check for mid-sprint changes

Step 3: Calculation Review
  - Compare with manual calculation
  - Check for excluded issue types
  - Verify reliability formula application
```

### Performance Issues

#### Slow Loading Times
**Symptoms**: Gadgets take >10 seconds to load

**Optimization Steps**:
1. **Reduce Data Scope**
   ```yaml
   Adjustments:
     - Limit sprint count to 10 or fewer
     - Use board-based vs project-based analysis
     - Focus on recent sprints only
   ```

2. **Check Jira Performance**
   ```yaml
   Diagnostics:
     - Test other Jira pages load time
     - Check Jira system status
     - Review instance resource usage
   ```

3. **Browser Optimization**
   ```yaml
   Actions:
     - Close unnecessary browser tabs
     - Clear browser cache and cookies
     - Disable browser extensions temporarily
     - Try different browser
   ```

#### Memory or Browser Crashes
**Symptoms**: Browser becomes unresponsive, crashes, or shows memory errors

**Solutions**:
```yaml
Immediate Actions:
  - Refresh the browser tab
  - Restart the browser
  - Clear browser cache
  - Increase browser memory allocation

Configuration Changes:
  - Reduce sprint count in reliability tracker
  - Use smaller dashboard gadget sizes
  - Limit concurrent analytics gadgets
  - Switch to board-based analysis
```

### Data Accuracy Issues

#### Missing Issues in Analysis
**Symptoms**: Expected issues not appearing in Sankey flows

**Debugging Process**:
```yaml
Issue Investigation:
  1. Check issue sprint assignment
  2. Verify story point assignment
  3. Confirm issue status transitions
  4. Review sprint date boundaries
  5. Check issue permissions

Common Causes:
  - Issues without story points (excluded)
  - Issues added after sprint end
  - Status transitions outside sprint
  - Permission restrictions
```

#### Incorrect Flow Classifications
**Symptoms**: Issues categorized in wrong Sankey flow categories

**Resolution Steps**:
```yaml
Status Mapping Review:
  1. Document expected vs actual classifications
  2. Check Jira workflow status mappings
  3. Review issue change history
  4. Verify sprint timeline accuracy

Typical Issues:
  - Custom status workflows
  - Bulk issue updates
  - Status transitions during sprint
  - Multiple status changes
```


## Getting Help

### Self-Service Resources

#### Documentation
```yaml
Quick References:
  - [Configuration Guide](Configuration-Guide.md)
  - [FAQ](FAQ.md)
  - [Best Practices](Best-Practices.md)
  - [Support](Support.md)
```


### Contacting Support

#### When to Contact Support
```yaml
Contact for:
  - Confirmed app bugs
  - Installation failures
  - Data accuracy issues
  - Performance problems
  - Security concerns

Try Self-Service First:
  - Configuration questions
  - Usage guidance
  - Best practices
  - Feature requests
```

#### Support Information
```yaml
Contact Details:
  Email: support@conwavelabs.com
  Response Time: See SLA document
  Include: Error messages, browser info, Jira version
```

### Information to Include

#### Bug Reports
```yaml
Required Information:
  - Jira version and instance type (Cloud/Data Center)
  - Browser version and operating system
  - Steps to reproduce the issue
  - Expected vs actual behavior
  - Error messages and screenshots
  - Affected board/project details
  - Number of users affected
```

#### Performance Issues
```yaml
Performance Details:
  - Specific slow operations
  - Data volume (sprint size, issue count)
  - Time measurements
  - Browser developer tools screenshots
  - Jira instance performance status
  - Network connectivity information
```

---

**Quick Resolution Tips** 🔧

Most issues can be resolved by:
1. Checking permissions and configuration
2. Clearing browser cache
3. Verifying data requirements
4. Testing with simplified scenarios

[← Back to Configuration](Configuration-Guide.md) | [Next: FAQ →](FAQ.md)

---
*Last Updated: July 2025*
