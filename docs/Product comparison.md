# Zephyr Squad and Zephyr feature comparison

This section compares key features in Zephyr Squad and Zephyr or Zephyr Essential.

## Test management

| Feature | Zephyr Squad | Zephyr or Zephyr Essential |
|---|---|---|
| Requirement management | Yes, through Jira | Yes, through Jira |
| Requirement and test case coverage traceability | Yes | Yes |
| Test case folder structure | No | Yes |
| Test case data | No | Yes |
| Test case parameters | No | Yes |
| Test steps | Yes | Yes |
| Test step wiki formatting | Yes | Yes |
| Import test cases | Yes | Yes |
| Test case repository | No | Yes |
| Test case versioning | No | Yes |
| Test case archiving | No | Yes |
| Test case history | Yes | Yes |
| Test case search | Yes | Yes |
| Test case saved filter | Yes | Yes |
| Test case bulk creation | Yes | Yes |
| Test case bulk edit | Yes | Yes |
| Test case clone | Yes | Yes |
| Reuse and execute test cases across spaces | No | Yes |
| Cross-space reporting and dashboard | No | Yes |
| Call to test to reuse test steps | No | Yes |

## Test planning and execution

| Feature | Zephyr Squad | Zephyr or Zephyr Essential |
|---|---|---|
| Test cycles | Yes | Yes |
| Test cycle history | No | Yes |
| Test cycle folder structure | Yes | Yes |
| N-level folder structure | No | Yes |
| Flexible move and copy across cycle folders | Yes | Yes |
| Test plans | No | Yes |
| Test plan history | No | Yes |
| Test execution | Yes | Yes |
| Test step results | Yes | Yes |
| Test execution history | Yes | No |
| Defect link on test execution | Yes | Yes |
| Defect link on test step results | Yes | Yes |
| Time tracking during execution | Yes | Yes |
| Search test executions | Yes | No |
| Export test cycles | CSV, HTML, XML | Excel |

## User management

| Feature | Zephyr Squad | Zephyr or Zephyr Essential |
|---|---|---|
| Roles and groups | Yes, through Jira | Yes, through Jira |
| Permission control | Yes, through Jira | Yes |

## Reports and advanced analytics

| Feature | Zephyr Squad | Zephyr or Zephyr Essential |
|---|---|---|
| Built-in reports, including traceability | Yes, up to five | Yes, up to 31 |
| Jira dashboard gadgets | Yes, up to nine | Yes, up to 19 |
| Test execution details gadget | Yes | No |
| Top Defects Impacting Testing gadget | Yes | No |
| Executions By Date gadget | Yes | No |

## Behavior-driven development

| Feature | Zephyr Squad | Zephyr or Zephyr Essential |
|---|---|---|
| Cucumber and Gherkin integration | Yes | Yes |
| Advanced features, such as Gherkin validations and tag management | Yes | No |

## Automation

| Feature | Zephyr Squad | Zephyr or Zephyr Essential |
|---|---|---|
| Supported automation frameworks | Eggplant, JUnit, Selenium, TestNG, Tricentis Tosca, UFT, Cucumber, Robot, and PyTest | JUnit, Selenium, TestNG, Tricentis Tosca, UFT, Cucumber, Robot, and PyTest |
| CI/CD script integration | Bitbucket Pipelines, TeamCity, CircleCI, GitLab, Azure DevOps, and others | Bitbucket Pipelines, TeamCity, CircleCI, GitLab, Azure DevOps, and others |
| CI/CD native integrations | Jenkins and Bamboo | Jenkins and Bamboo |
| SmartBear tools integration | ReadyAPI, TestComplete, CrossBrowserTesting, and LoadNinja | No |
| APIs for custom integrations | Yes | Yes |
| Import test cases from other tools | Yes | Yes |

## Other features

| Feature | Zephyr Squad | Zephyr or Zephyr Essential |
|---|---|---|
| Team-managed project support | Yes | Yes |
| Internationalization support | Yes | Yes |
| Server to Cloud migration support | Yes | Yes |
| GDPR compliance | Yes | Yes |
| Cloud Security participant | Yes | Yes |
| Cloud Fortified support | No | Yes |

## Key differences

### Test cycle folder structure

In Zephyr Squad, cycles are organized by releases. Users can create folders within a cycle to add another level of organization.

In Zephyr, users can organize test cycles into hierarchical folders. These folders are not tied to releases. Test cases can be added to a cycle in a flat list.

### Test execution history

Zephyr Squad logs test execution history for status changes, attachments, assignees, comments, and custom fields.

Zephyr does not track history at the individual test execution level. Zephyr tracks changes at the test cycle level.

### Search test executions

Zephyr Squad includes a Search Test Executions page with basic search, advanced search, saved filters, and predefined filters.

Zephyr does not include a dedicated search test executions page.

### Export test cycles

Zephyr Squad supports exporting test cycles from Cycle Summary and Search Test Executions in CSV, HTML, and XML formats.

Zephyr supports exporting test cycle information through reports in Excel format.

### Reports and gadgets

Zephyr Squad includes up to five built-in reports and up to nine Jira dashboard gadgets.

Zephyr includes up to 31 reports and up to 19 Jira dashboard gadgets. Some Zephyr Squad reports and gadgets do not have direct equivalents in Zephyr, including:

- Test execution details gadget.
- Top Defects Impacting Testing gadget.
- Executions By Date gadget.

### Cucumber and Gherkin support

Zephyr does not include a feature editor or tag management. Zephyr exports one feature file per test case, while Zephyr Squad supports feature-level organization.

Zephyr provides a more detailed test case result view with additional error details.

### Automation

Zephyr does not include a UI for creating automation tasks. Zephyr uses REST API endpoints and supports Cucumber, JUnit 5, and JUnit 4 file formats.

Some frameworks supported by Zephyr Squad require result conversion to JUnit format before use in Zephyr.

### SmartBear tools integration

Zephyr Squad integrates with the following SmartBear tools:

- TestComplete.
- ReadyAPI.
- LoadNinja.
- CrossBrowserTesting.

Zephyr does not provide direct integrations with these tools. Use Zephyr REST APIs to upload results.

### REST API differences

Zephyr Squad and Zephyr use different REST APIs. Review and update custom integrations before migration.

- Zephyr Squad API: Zephyr Squad Cloud REST API.
- Zephyr API: Zephyr for Jira Cloud API.