# Squad to Zephyr upgrade guide

This guide helps teams upgrade from Zephyr Squad to Zephyr. It outlines the upgrade path, migration process, and key considerations. Zephyr provides improved performance, advanced automation capabilities, and a modern user experience.

---

## Why upgrade to Zephyr

Zephyr provides the following benefits:

- Modern and consistent user experience with AI-powered automation workflows  
- High-performance backend system designed for scalability and advanced automation  
- Support for compliance and enterprise automation requirements  

---

## Key features

Zephyr includes the following capabilities:

- Cross-space test management  
- Test repository  
- Test case versioning  
- Test data and parameters  
- Test plans  
- Multi-level folder structure  
- Enhanced reporting  
- Improved performance  
- AI-powered no-code automation  
- Record and play test generation  
- Test step suggestions  
- Data residency and compliance support  
- Upgrade path to Zephyr Advanced, including cross-browser testing, parallel testing, email and SMS testing, and increased AI test runs  

For more details, see Product Comparison and Feature Comparison.

---

## Upgrade experience

Upgrading from Zephyr Squad to Zephyr includes:

- Dedicated migration UI  
  - Project-level migration  
  - Progress tracking and retry options  
  - Migration logs  

- Ability to migrate individual spaces  
- Validation per space during or after migration  

---

## App availability during migration

Zephyr Squad remains available during migration. You can continue to create or modify data.

To include newly added or updated data in Zephyr, rerun the migration. This process overwrites previously migrated data.

Existing data in Zephyr is also overwritten. Merging or incremental migrations are not supported.

The migration UI includes an option to block Squad during migration. Enable this option to prevent data inconsistencies and maintain data integrity.

---

## Environment options

### Production migration  
Fully supported. Zephyr Squad remains available during migration.  

### Sandbox migration  
Supported with manual setup. You cannot copy Squad data directly from production. Use CSV export and import for test cases and test steps.  

> **Note**  
> CSV import supports only test cases and test steps. It does not support test cycles or test executions.  

For step-by-step instructions, see Upgrade to Zephyr – Step-by-step guide.

---

## Migrated data

The migration includes the following entities:

- Test cases  
- Test cycles  
- Test executions  

The following data is not migrated:

- BDD data  
- Test execution history  

For details, see Data Mapping Reference and Non-migrated Data Details.

---

## Roadmap for non-migrated data

Support for additional data types is planned:

| Data type                | Expected availability |
|-------------------------|----------------------|
| BDD data                | Q3 2026              |
| Test execution history  | Q3 2026              |

These timelines are subject to change.

Track updates or submit requests on the Feature Request Portal.

---

## Time and effort required

Migration occurs space by space, allowing validation at each step.

Zephyr uses different REST API endpoints than Zephyr Squad. Update automation scripts to use the new endpoints.

For more information, see:
- Zephyr API Documentation  
- API Differences Reference  

The total time required depends on data volume and the number of spaces.

---

## Pricing and licensing

Upgrading to Zephyr requires a new license.

If more than six months remain on the Zephyr Squad subscription, request a prorated discount. The discount is provided as a promo code for the new Zephyr subscription.

You can allow the existing Squad license to expire.

Dual licensing is available during upgrade or user acceptance testing (UAT) upon request. A limited free license is provided for customers with an active paid subscription.

For licensing questions, contact richard.humphries@smartbear.com.

---

## Register for the upgrade

To start the upgrade, create a support ticket. The support team provides guidance based on the selected upgrade path.

---

## See also

- Upgrade to Zephyr – Step-by-step guide  
- Data Mapping Reference  
- Non-migrated Data Details  
- CSV export and import help article  
- Product Comparison  
- Feature Comparison  

---

## Known issues and troubleshooting

> **Warning**  
> Zephyr Squad to Zephyr Essential or Zephyr upgrades are not currently supported on the Forge platform. Migrations do not work when using Squad version 8.2.11 or later. A fix is under development.  

For known issues, see the Migration Known Issues Tracker.

If you encounter issues not listed, contact SmartBear support.