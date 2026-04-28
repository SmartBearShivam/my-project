# Migrate to Zephyr

> **Note**  
> This option requires manual enablement by SmartBear support. Create a support ticket to enable this feature.

---

## Overview

The migration user interface allows selected customers to migrate data from Zephyr Squad to Zephyr. The interface provides visibility into entities available for migration and identifies unsupported data before the process begins.

Install the Zephyr app before starting the migration.

---

## Start the migration

To start the migration, perform the following steps:

1. Go to **Apps** > **Zephyr Squad** on the left sidebar in your Jira instance.  
2. Click the three dots to open the app settings.  

   ![App settings](ZephyrSquad_Screenshot_ZephyrSquadAppSettings.png)

3. Install the Zephyr app.  
4. Click **Start Migration** and select the required checkboxes.  

   ![Start migration](ZephyrSquad_Screenshot_StartMigartion.png)

If another migration is in progress, wait for it to complete. The next migration starts automatically.

   ![Migration queue](ZephyrSquad_Screenshot_MigartionQueue.png)

---

## Select projects

After starting the migration, choose one of the following options:

- Select **Migrate All Projects** and click **Continue Migration**.  

  ![Migrate all projects](Zephyr_Migrate_1.png)

- Use the search bar to select specific projects and click **Continue Migration**.  

You can select up to 50 projects at a time. The project list displays migrated projects. You can skip or re-migrate them as needed.

> **Warning**  
> You cannot cancel the migration after it starts.  

> **Warning**  
> Running the migration again overwrites existing data in Zephyr.

---

## Track migration progress

Track migration progress in the user interface using the progress bar. The progress bar shows the overall status across all projects.

If the migration fails or encounters issues, the process stops and displays an error message.

   ![Migration progress](ZephyrSquad_Screenshot_MigartionProgress.png)

### Migration outcomes

- **Migration complete**  
  All selected projects are successfully migrated.  

 
- **Migration partially complete**  
  Some projects fail. Review error logs for details.  

- **Migration fails**  
  Restart the migration using the **Re-run migration** option.  

> **Warning**  
> Re-running the migration restarts the process and overwrites existing data.

---

## Data limitations

The following data is not supported for migration:

- BDD data  
- Test execution history  

The migration process does not support delta migration. Data created after the migration starts is not included.

---

## Using Zephyr Squad during migration

You can continue to use Zephyr Squad during migration. However, data created during the migration is not transferred to Zephyr.

For example, if testers add test cases or executions during migration, recreate or re-import this data in Zephyr after migration completes.

---

## Migration completion

After migration completes, review the migrated data in Zephyr.

To access Zephyr:

- Click **Navigate to Home page** after migration completes, or  
- Go to **Apps** and select **Zephyr** from the Jira homepage.  

If the data meets expectations, subscribe to Zephyr and unsubscribe from Zephyr Squad.

If issues occur, rerun the migration or contact SmartBear support.

---

## Data not migrated

The following data is not migrated:

- BDD data  
- Test execution audit logs  
- Test execution saved filters  
- JQL saved filters  
- Test step custom field change history  
- Custom fields of type Select list (cascading)  
- Custom fields of type Label  
- Advanced custom fields for test cases  

---

## Support

If you encounter issues during migration, contact SmartBear support for assistance.

## Watch the demo

Learn how migration works in Zephyr:

[![Zephyr migration demo](https://support.smartbear.com/zephyr/docs/en/image/uuid-cee830bf-08a2-5c84-5377-de49e75eea57.png)](https://www.youtube.com/watch?v=QbtmHlUvaeI)