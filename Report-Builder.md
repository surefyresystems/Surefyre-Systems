This section explains the following:

* [Report Builder Overview](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#report-builder-overview)
* [Report Content Types](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#report-content-types)
* [Running Saved Reports](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#running-saved-reports)
* [Creating / Editing Reports](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#creating--editing-reports)
  * [Report Filters](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#report-filters)
  * [Report Columns](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#report-columns)
  * [Adding Filter/Column Fields](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#adding-filter--column-fields)
  * [Removing Filter/Column Fields](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#removing-filter--column-fields)
* [Pinning Reports](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#pinning-reports)
* [Downloading Reports](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#downloading-reports)
* [Mass Email](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#mass-email)  
* [Video Tutorials](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#video-tutorials)

***


## Report Builder Overview

The Report Builder is a powerful and customizable tool that allows you to create filtered lists of accounts, people, policies, and commission records. You can use reports to execute various actions such as emailing, downloading, or making call lists. Depending on the type of insurance you sell, these are some common use cases of the Surefyre Report Builder:

* Find all policies with renewals coming up next month so you can get in touch with those accounts
* Find all people who have a birthday next month and mass email happy birthday notes
* Find all accounts in a specific zip code for planning on-site visits
* Create and download census reports to send to carriers for quotes or enrollments
* Build a call list of all open leads
* Segment leads and add them to email drip marketing campaigns
* and many more...

Access the Report Builder tab anytime from the [Navigation Bar](https://github.com/surefyresystems/Surefyre-Systems/wiki/Basic-Naviation).

![](https://user-images.githubusercontent.com/31252743/37816982-4c19ac58-2e32-11e8-84a2-68488a050dff.png)
[Zoom](https://user-images.githubusercontent.com/31252743/37816982-4c19ac58-2e32-11e8-84a2-68488a050dff.png)

***

## Report Content Types

The Report Content Type describes what you're reporting on. In other words, it defines what each row of the report represents. Here are the possible content types:

* **Account** - Account reports can return any type of account (Business, Personal, Group, etc.). An example is a lead or client list.
* **Person** - Person reports return information about individual people in the system such as insured and dependents. An example is a list of all people (insured, dependents, etc.) that have a birthday this month and should receive happy birthday emails or letters.
* **Policy** - Policy reports return information about policies. An example is a report showing all policies that have renewals next month. 
* **Commission** - Commission reports give users more granular control of which commission records they are viewing or downloading (compared to the Commissions section).

The content type is always indicated underneath the report name:

![](https://user-images.githubusercontent.com/31252743/37816283-c37b1dac-2e2f-11e8-89d6-db8b7ce71abc.png)
[Zoom](https://user-images.githubusercontent.com/31252743/37816283-c37b1dac-2e2f-11e8-89d6-db8b7ce71abc.png)

When creating new reports, be sure to start with the content type that makes sense for the type of data you want to see.

***

## Running Saved Reports

To run an existing report simply click the **Saved Reports** tab in the left column then select the desired report from the list to run it.

![](https://user-images.githubusercontent.com/31252743/37817353-c33a981e-2e33-11e8-80fd-6efe5d6cef6f.png)
[Zoom](https://user-images.githubusercontent.com/31252743/37817353-c33a981e-2e33-11e8-80fd-6efe5d6cef6f.png)

***

## Creating / Editing Reports

Whether creating a new report or editing an existing one, you must start by [running a saved report](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#running-saved-reports). Basic reports such as All Accounts, All Policies, etc. are available by default and are a good starting point for their respective [content types](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#report-content-types).
> For example, if you'd like to create a report of people who are turning 65 next quarter, start with the default All People report and filter it down to just people whose birthdays fall in that date range.

Once you have selected a saved report as a starting point, [edit the report filters](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#editing-report-filters) to exclude records that you don't want.
> In our above birthday example, this would be the step where you would add Date of Birth field as a filter and set the desired date range. Any people with birthdays outside the filter range will not show up in the report.

Next, [edit the report columns](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#editing-report-columns) to see the desired fields in each row.
> Again in the above birthday example, you could add the Email field as a column to ensure that each person in the report has an email address before sending off a [mass email](https://github.com/surefyresystems/Surefyre-Systems/wiki/Email#mass-add-accounts-to-a-an-email-campaign).

Finally, save your changes to the current report by clicking **Save**. It's important to **save often** to ensure your changes are not lost. You can also save as a new report by clicking **Save As**. When creating a new report you can indicate a name and whether or not it's public. Public reports can be seen all any user in your Surefyre system that has access to the report builder. Note that default reports cannot be overwritten, so the Save button is not available.

![](https://user-images.githubusercontent.com/31252743/37822978-55c0425e-2e45-11e8-8969-5b91fd3ea8e0.png)

### Report Filters

Use filters to ensure only the records you want to see are in your report. When you select the **Filters** tab in the left column you will see a list of all filters selected for the current report. Filters with no value have no affect on the report.

In the example below we are filter an account report to only show leads for a specific user:
![](https://user-images.githubusercontent.com/31252743/37823459-c1fc647e-2e46-11e8-9fac-6c7dcf5ada0f.png)
[Zoom](https://user-images.githubusercontent.com/31252743/37823459-c1fc647e-2e46-11e8-9fac-6c7dcf5ada0f.png)

To add filters click the **+ Add Field** button below the existing filter fields. The field selection popup will appear with a list of all content type fields available for selection. See [Adding Filter / Column Fields](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#adding-filter--column-fields) for a guide to selecting filter fields.

### Report Columns

Edit report columns to see all the desired data about the records in your report and remove unnecessary data.

To add columns click the **+ Add Column** button in the view options of the report results window. The field selection popup will appear with a list of all content type fields available for selection. See [Adding Filter / Column Fields](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#adding-filter--column-fields) for a guide to selecting column fields.

To reposition or rename columns (usually to prepare the data for import into a 3rd party system), click the pencil icon in the view options of report results window. This will enable **edit mode**. While in edit mode you can reposition columns by dragging and drop and rename them by clicking the column header title and entering a new value. When you're finished click **Done Editing**.

### Adding Filter / Column Fields

When adding [filter](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#report-filters) or [column](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#report-columns) fields you will be presented with a popup where you can quickly search and add multiple fields. When you've found the field you want simply click it and a confirmation will appear that it's been added.

![](https://user-images.githubusercontent.com/31252743/37823866-0e6e4c22-2e48-11e8-9f33-11fec91c7679.png)

You can add fields from related content types. In the example of an account report, you can add account fields from addresses and/or people associated to that account.

### Removing Filter / Column Fields

To remove [filter](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#report-filters) or [column](https://github.com/surefyresystems/Surefyre-Systems/wiki/Report-Builder#report-columns) fields, click the pencil icon in the view options of the report results window. This will enable **edit mode**. While in edit mode you can click the delete / trash icon next to any column or filter field to remove it.

***

## Pinning Reports

You can pin reports to your [Home Page Dashboard](https://github.com/surefyresystems/Surefyre-Systems/wiki/Home-Page) for quick reference. For example, if you create a report of all accounts that need a follow up, you can see that report at a glance each time you sign in to Surefyre.

![](https://user-images.githubusercontent.com/31252743/37824981-93bebe04-2e4b-11e8-8f77-0d117ac2bc56.png)

To pin a saved report to your own dashboard, click the **star icon** next to the report name in the left column. Pinned reports will display at the top of the Saved Reports list.

![](https://user-images.githubusercontent.com/31252743/37824713-c4bb7282-2e4a-11e8-9ad2-54667d347f32.png)

To pin a saved report to another user's dashboard or for an entire group (if permissions allow), click the **Group** icon next to the report name in the left column. A popup will appear allowing you to pin the report to multiple groups and/or users.

![](https://user-images.githubusercontent.com/31252743/37825199-38149e42-2e4c-11e8-97e3-ddd3e1469298.png)

***

## Downloading Reports

Click the **Download** button in the left column to download the current report as a csv file. These files can be used for any number of external processes including upload into 3rd party systems.

***

## Mass Email

See [mass add accounts to an email campaign](https://github.com/surefyresystems/Surefyre-Systems/wiki/Email#mass-add-accounts-to-a-an-email-campaign)

***

## Video Tutorials

* [Create a Simple Policy Report](https://youtu.be/08V_yCPKa0c)
* [Mass Email with Report Builder](https://youtu.be/uKcd18RsM1o)
* [Create Benefit Census with Insureds and Dependents](https://youtu.be/V3CpvKrNsAE)

***

Related:

* [Home Page Dashboard](https://github.com/surefyresystems/Surefyre-Systems/wiki/Home-Page)
* [Mass add accounts to an email campaign](https://github.com/surefyresystems/Surefyre-Systems/wiki/Email#mass-add-accounts-to-a-an-email-campaign)