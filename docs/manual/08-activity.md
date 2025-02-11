# Activity

Execution history for commands and Jobs is stored by the Rundeck server. Execution history can be filtered and viewed inside the "Activity" page.

![Activity page](~@assets/img/fig0211.png)

## Filtering Activity

By default, the Activity page will list running executions and history
recent executions. The page contains a filter control that can be used to
expand or limit the executions.

The filter form contains a number of fields to limit search:

- Within: Time range. Choices include 1 day, 1 week, 1 month or other
  (given a start after/before to ended after/before).
- Job Name: Job title name.
- User: User initiating action.
- Filter: The node filter used . You can enter just one node name to see if was executed against that node or use the node filter formats. Refer to the [User Guide - Node Filters](/manual/11-node-filters.md) Documentation.
- Ad hoc command: Command typed into the command bar or via `dispatch`.
- Result: Success or failure status.

![History filter form](~@assets/img/fig0212.png)

After filling the form pressing the "Filter" button, the page will
display executions matching the search.

## Activity in PagerDuty Process Automation On Premise's Home

On the home page, users can check activity for a specific project, such as failed executions for each project.

:::warning
Only the **failed** executions will display, excluding "missed" and other status.
:::

![Project Activity on home page (dark mode)](~@assets/img/rundeckHome.png)

## Extended date range

It is also possible to search for activity between dates.
Press the "Other..." menu choice to bring up the form.

![Extended date range search](~@assets/img/fig0217.png)

## Saving the filter

Filters can be saved to a menu that makes repeating searches more
convenient. Click the "save this filter..." link to save the filter
configuration.

## Execution listings

Information for each execution contains the command or Job executed,
options, success status and a link to a file containing all
the output messages.

![Execution view](~@assets/img/fig0213.png)

If any errors occurred, the "Node Failure Count" column will show
the number of nodes in red text. A bar chart indicates the percent
failed.

![Execution view](~@assets/img/fig0216.png)

## RSS link

If configured, an RSS icon provides a link to an RSS view of the events that match
the current filtering criteria.

![RSS link](~@assets/img/fig0214.png)

## Bulk Delete Executions

If you have access, you can click the "Bulk Delete" button to enable bulk-edit mode.

![Activity page bulk delete](~@assets/img/fig08-activity-bulk-delete.png)

Select the Executions you want to delete by clicking on them. You can also click on the "Toggle all", "Select All" or "Select None" links to change the selection.

![Activity page bulk edit mode](~@assets/img/fig08-activity-bulk-edit-mode.png)

Click the "Delete Selected Executions", and confirm to delete the executions.

![Activity page bulk delete confirm](~@assets/img/fig08-activity-bulk-delete-confirm.png)
