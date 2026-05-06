# Data transfer during migration

During the upgrade from Zephyr Squad to Zephyr or Zephyr Essential, Jira settings and permissions remain unchanged. The following sections describe how data is migrated and mapped.

---

## Test case field mapping

| Squad field | Zephyr field | Notes |
|---|---|---|
| Summary | Name | Migrated directly |
| Description | Objective | Migrated directly |
| Status | Status | Jira issue statuses are recreated as custom statuses in Zephyr |
| Assignee | Custom field (Assignee) | Created as a user picker field |
| Labels | Labels | Migrated directly |
| Sprint | Custom field (Sprint) | Select list (multi-choice) |
| Story points | Not migrated | Not supported in Zephyr |
| Fix versions | Custom field (Fix versions) | Select list (multi-choice) |
| Affected versions | Custom field (Affected version) | Select list (multi-choice) |
| Reporter | Owner | Mapped to Owner field |
| Priority | Priority | Migrated as custom priorities |
| Due date | Custom field (Due Date) | Date picker |
| Original estimate | Estimated time | Converted to hh:mm format |
| Time tracking | Not migrated | Represented differently in Zephyr |
| Start dates | Custom field (Start dates) | Date picker |
| Environment | Custom field (Environment) | Multi-line text field |
| Component | Component | Multiple values mapped to custom field |
| Epic link | Traceability section | Linked to Jira issue |
| Issue links | Traceability section | Linked to Jira issue |
| Subtasks | Traceability section | Linked to Jira issue |
| Comments | Comments | Migrated directly |
| Attachments | Attachments | Migrated directly |

---

## Test case custom fields

All custom fields are migrated except advanced Jira field types.

| Squad type | Zephyr type |
|---|---|
| Checkboxes | Select list (multi-choice) |
| Date picker | Date picker |
| Date time picker | Date picker |
| Number field | Number |
| Radio buttons | Select list (single choice) |
| Select list (multiple) | Select list (multi-choice) |
| Select list (single) | Select list (single choice) |
| Paragraph | Text field (multi-line) |
| Short text | Text field (single-line) |
| URL | Text field (multi-line) |
| User picker | User picker |

---

## Test case steps mapping

| Squad | Zephyr |
|---|---|
| Test step | Step |
| Test data | Test data |
| Test result | Expected result |
| Attachments | Attachments |
| Custom fields | Custom fields |

Test step attachments and custom fields are migrated.

---

## Test case history

Test case history is created by combining:

- Jira issue history  
- Test details history  

All changes are sorted by timestamp and imported as a unified history.

---

## Test cycle field mapping

| Squad | Zephyr |
|---|---|
| Version | Release version |
| Name | Name |
| Description | Description |
| Build | Custom field |
| Environment | Custom field |
| From | Planned start date |
| To | Planned end date |

---

## Test execution field mapping

| Squad | Zephyr |
|---|---|
| Execution ID | Execution ID |
| Summary | Summary |
| Description | Objective |
| Execution status | Execution status |
| Assigned to | Assigned to |
| Defects | Issues |
| Comments | Comments |
| Executed by | Executed by |
| Executed on | Executed on |
| Total execution time | Estimated |
| Total logged time | Actual |
| Attachments | Attachments |

### Status mapping

- UNEXECUTED → Not Executed  
- WIP → In Progress  
- PASS → Pass  
- FAIL → Fail  
- BLOCKED → Blocked  
- Custom → Custom  

---

## Test step result mapping

| Squad | Zephyr |
|---|---|
| Step | Step |
| Test data | Test data |
| Result | Result |
| Status | Status |
| Comments | Actual result |
| Attachments | Attachments |
| Defects | Issues |

---

## Test cycle structure mapping

In Zephyr Squad:
- Test cycles are grouped by fix versions  
- Folders exist within cycles  

In Zephyr:
- Folder hierarchy is created first  
- Test cycles are created inside folders  

Migration behavior:
- Squad cycles and folders are converted into Zephyr folders  
- Test cycles are recreated within those folders  
- Fix versions are mapped as fields  

Ad hoc cycles are migrated into a dedicated **Ad hoc** folder.

---

## API tokens

Existing API tokens from Zephyr Squad are not migrated. Create new tokens in Zephyr.

---

## Test automation

Saved automation configurations are not migrated. Zephyr uses REST API-based automation.

---

## Data not migrated

The following data is not migrated:

- BDD data  
- Test execution audit logs  
- Test execution saved filters  
- JQL saved filters  
- Test step custom field change history  
- Custom field of type Select list (cascading)  
- Custom field of type Label  
- Advanced custom fields for test cases  

---

## Summary

Migration preserves core testing data, including test cases, steps, executions, and attachments. Some fields are transformed into custom fields, and unsupported data is excluded. Review mappings carefully before migration to ensure compatibility.