# Zephyr Squad to Zephyr feature comparison

Use this reference to compare Zephyr Squad and Zephyr capabilities before migration.

## Test management

| Feature | Zephyr Squad | Zephyr | Can be migrated | Additional information |
|---|---|---|---|---|
| Test issue type | Yes | No | No | In Zephyr Squad, test cases are Jira issues. In Zephyr, test cases are internal Zephyr objects managed by SmartBear. |
| Test cases | Yes | Yes | Yes | Test cases migrate to Zephyr, but use a different data architecture. |
| Test case custom fields | Yes | Yes | Yes | Advanced custom field types are not migrated. |
| Test case attachments | Yes | Yes | Yes | Attachments migrate with test cases. |
| Multiple components | Yes | No | Yes | If a test case has multiple components, one component maps to the component field. Other components map to the **Squad components** custom field. |
| Test steps | Yes | Yes | Yes | Test steps migrate to Zephyr. |
| Test step wiki formatting | Yes | Yes | Yes | Wiki formatting migrates to Zephyr. |
| Test step custom fields | Yes, maximum five | Yes | Yes | Test step custom fields migrate to Zephyr. |
| Test step attachments | Yes | Yes | Yes | Test step attachments migrate to Zephyr. |
| Export test cases with test steps | Yes | Yes | Not applicable | Zephyr supports export through supported formats. |
| Import test cases | Yes | Yes | Not applicable | Zephyr supports import using CSV, Excel through CSV, and XML. |
| Test repository | No | Yes | Not applicable | Zephyr includes a test repository. |
| Test case archiving | Yes for Server and Data Center, no for Cloud | Yes | Not applicable | Zephyr supports archived test cases. |
| Test case history | Yes | Yes | Yes | Test case history migrates to Zephyr. |
| Test step history | Yes | Yes | Yes | Test step history migrates to Zephyr. |
| Test case search | Yes | Yes | Not applicable | Search is available in both products. |
| Test case saved filters | Yes | Yes | No | Saved filters are not migrated. |

## Test planning and execution

| Feature | Zephyr Squad | Zephyr | Can be migrated | Additional information |
|---|---|---|---|---|
| Test cycles | Yes | Yes | To be determined | Test cycles are supported in both products. |
| Test cycle custom fields | No | Yes | Not applicable | This feature does not exist in Zephyr Squad. |
| Test cycle attachments | No | Yes | Not applicable | This feature does not exist in Zephyr Squad. |
| Ad hoc test cycles | Yes | Yes | To be determined | Zephyr supports ad hoc test executions. |
| Multi-level folder structure | No | Yes | Not applicable | This feature does not exist in Zephyr Squad. |
| Test cycle organization | Versions and subfolders within cycles | No direct equivalent | Not applicable | Zephyr Squad organizes cycles by releases and folders. |
| Export test cycles | Yes | Yes | Not applicable | Zephyr exports test cycle data through reports. |
| Test cycle search | Yes | Yes | To be determined | Search is available in both products. |
| Test plans | No | Yes | Not applicable | This feature does not exist in Zephyr Squad. |
| Test plan search | No | Yes | Not applicable | This feature does not exist in Zephyr Squad. |
| Test plan custom fields | No | Yes | Not applicable | This feature does not exist in Zephyr Squad. |
| Test plan attachments | Yes | Yes | To be determined | Test plan attachment migration status is not finalized. |
| Test execution | Yes | Yes | To be determined | Test executions are supported in both products. |
| Test execution custom fields | Yes, maximum five | Yes | To be determined | Zephyr supports test execution custom fields. |
| Test execution attachments | Yes | Yes | To be determined | Zephyr supports test execution attachments. |
| Test execution custom status | Yes | Yes | To be determined | Zephyr supports custom execution statuses. |
| Defect link on test execution | Yes | Yes | To be determined | Defects can be linked to test executions. |
| Multiple test executions in test cycle | Only on ad hoc cycles | Yes | To be determined | Zephyr supports multiple test executions in a test cycle. |
| Export test execution | Yes | Yes | To be determined | Zephyr exports test execution data through reports. |
| Test step results | Yes | Yes | To be determined | Zephyr supports test step results. |
| Test step result attachments | Yes | Yes | To be determined | Zephyr supports attachments on test step results. |
| Test step result custom status | Yes | Yes | To be determined | Zephyr supports custom statuses for test step results. |
| Defect link on test step results | Yes | Yes | To be determined | Defects can be linked to test step results. |
| Time tracking during execution | Yes | Yes | To be determined | Zephyr supports time tracking. |
| Reporting on test execution | Yes | Yes | Not applicable | Zephyr provides similar reporting capabilities. |
| Reporting on top defects | Yes | No | No | This feature does not exist in Zephyr. |
| Traceability | Yes | Yes | Not applicable | Zephyr provides similar traceability capabilities. |
| Search test executions | Yes | No | Not applicable | This feature does not exist in Zephyr. |
| Test execution filters | Yes | No | No | This feature does not exist in Zephyr. |
| Test execution bulk operations | Yes | Partial | Not applicable | Zephyr supports bulk assignment of tester, environment, and iteration. |
| Test execution change history | Yes | No | Partial | Zephyr records changes at the test cycle level only. Execution status changes are not recorded. |

## User management

| Feature | Zephyr Squad | Zephyr | Can be migrated | Additional information |
|---|---|---|---|---|
| Roles and groups | Yes, through Jira | Yes, through Jira | Not applicable | Uses Jira roles and groups. |
| Permission control | Jira permissions in Cloud. Jira and Zephyr permissions in Server. | Jira and Zephyr permissions | Not applicable | Zephyr includes Jira and Zephyr permission controls. |
| Issue type support control | Yes for team-managed projects. No for company-managed projects. | Yes | Not applicable | Zephyr supports issue type configuration. |

## Reports and analytics

| Feature | Zephyr Squad | Zephyr | Can be migrated | Additional information |
|---|---|---|---|---|
| Jira dashboard gadgets | Nine gadgets | 21 gadgets | Not applicable | Test execution details and Top Defects Impacting Testing have no direct Zephyr equivalent. |
| Jira reports | Three reports | No | Not applicable | Zephyr uses its own reports section. |
| Zephyr test metrics page | Five reports | 29 reports | Yes | Zephyr provides reporting through the Reports tab. |

## Jira Agile board

| Feature | Zephyr Squad | Zephyr | Can be migrated | Additional information |
|---|---|---|---|---|
| Link test cycles or folders to a sprint | Yes | No | Not applicable | This feature does not exist in Zephyr. |
| Test execution view in issue backlog | Yes | No | Not applicable | This feature does not exist in Zephyr. |

## Behavior-driven development

| Feature | Zephyr Squad | Zephyr | Can be migrated | Additional information |
|---|---|---|---|---|
| Cucumber and Gherkin integration | Yes | Partial | Not applicable | Zephyr does not support BDD feature file creation. |
| Advanced Gherkin features | Yes | Partial | Not applicable | Zephyr supports Gherkin validations, but does not support tag management. |

## Automation

| Feature | Zephyr Squad | Zephyr | Can be migrated | Additional information |
|---|---|---|---|---|
| Supported automation frameworks | Yes | Yes | Not applicable | Zephyr supports common frameworks through JUnit and Cucumber JSON formats. |
| Test automation integration UI | Yes | No | Not applicable | Zephyr uses REST API for test automation. |
| ZBot | Yes | No | Not applicable | ZBot is not available in Zephyr. |
| CI/CD tool support | Yes | Yes | Not applicable | Both products support CI/CD integrations through post-build actions. |
| REST API support | Yes | Yes | Not applicable | Zephyr Squad and Zephyr APIs are different. Update integrations before migration. |
| SmartBear tool integrations | Yes | No | Not applicable | Zephyr Squad integrates with TestComplete, ReadyAPI, LoadNinja, and CrossBrowserTesting. |

## Configuration and administration

| Feature | Zephyr Squad | Zephyr | Can be migrated | Additional information |
|---|---|---|---|---|
| Reindexing | Yes | Not required | Not applicable | Zephyr does not require reindexing. |
| Custom status | Yes | Yes | Yes | Zephyr supports custom statuses for test cases, plans, cycles, and executions. |
| Custom environment | Jira environment field | Yes | Yes | Custom environments migrate to Zephyr. |
| Custom labels | Jira label field | Yes | Yes | Custom labels migrate to Zephyr. |
| Custom priorities | Jira priority field | Yes | Yes | Custom priorities migrate to Zephyr. |
| Custom datasets | No | Yes | Not applicable | This feature does not exist in Zephyr Squad. |

## Other capabilities

| Feature | Zephyr Squad | Zephyr | Can be migrated | Additional information |
|---|---|---|---|---|
| Team-managed project support | Yes | Yes | Not applicable | Both products support team-managed projects. |
| Internationalization | Yes | Yes | Not applicable | Supported languages differ by product. |
| GDPR compliance | Yes | Yes | Not applicable | Both products support GDPR requirements. |
| Cloud Security Participant | Yes | Yes | Not applicable | Both products participate in Atlassian Cloud Security programs. |
| Cloud Fortified support | No | Yes | Not applicable | Zephyr supports Cloud Fortified requirements. |
| Data storage | Jira and SmartBear servers | SmartBear servers | Not applicable | Zephyr stores data on SmartBear servers and does not store test data on Jira servers. |

## Data architecture differences

In Zephyr Squad, test cases are Jira issues. In Zephyr, test cases are internal Zephyr objects managed by SmartBear.

This architecture reduces the impact on Jira performance because Zephyr does not store test management data on Jira servers.

## Migration considerations

Review the following before migration:

- Zephyr Squad and Zephyr use different REST API endpoints.
- Update automation scripts before migration.
- Advanced custom fields are not migrated.
- BDD data is not fully supported in Zephyr.
- Test execution saved filters are not migrated.
- Some Zephyr Squad reports and gadgets have no direct Zephyr equivalent.