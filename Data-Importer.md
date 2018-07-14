Administrators can easily import large amounts of data such as business accounts, personal accounts, addresses, policies, and commissions. The Surefyre Data Importer accepts files in the common **csv** format. This section explains how to do the following:

* [Import Data from a New Source](https://github.com/surefyresystems/Surefyre-Systems/wiki/Data-Importer#import-data-from-a-new-source) - Import data from a source for the first time by creating a new Import Configuration.
* [Import Data from an Existing Source](https://github.com/surefyresystems/Surefyre-Systems/wiki/Data-Importer#import-data-from-an-existing-source) - Quickly import data from a source that you've imported from before by use an existing Import Configuration.

***

# Import Data from a New Source
When importing data for the first time, you must create an Import Configuration for that data source. An Import Configuration simply maps column name in the import csv file to fields in Surefyre.

> Example: An import csv file with business accounts might have a column name **Business Lead Name**. This would map to the **Business Name** field in Surefyre. When the import is executed, Surefyre will use the data in the **Name** column of the import file to populate/update the **Business Name** field on new/existing business accounts. 

1. Click **Create (+)** > **Import Data** to open the Surefyre Data Importer

![](https://user-images.githubusercontent.com/31252743/36079943-9f83f164-0f3d-11e8-8b97-9e7aae8dc2f9.png)

2. Click **Build New Configuration** to create a new mapping between the data import file columns and Surefyre fields

![](https://user-images.githubusercontent.com/31252743/36079942-9f6fb596-0f3d-11e8-89dc-78cf4f2f7018.png)

3. Select a **Content Type** based on the type of data you're importing. Enter a **Name** and **Description** describing the data source for future reference. Examples could be "Carrier ABC Commissions" or "New Leads from ABC Lead Source"

4. Check **Skip Existing** if you'd like to skip rows representing data that already exists in Surefyre.

![](https://user-images.githubusercontent.com/31252743/36079941-9f460322-0f3d-11e8-89b7-a535f89d2808.png)

> Example: You have a large data file with both new and existing leads in it. You only want to import the new leads without updating / overwriting data on your existing leads. You check **Skip Existing** in the Import Configuration to skip all data in the import file that represents existing leads. 

5. **Select Surefyre fields to import:** The **Fields to Import** section contains a searchable list of available Surefyre fields based on the selected **Content Type**. For each column name in your import file, select all corresponding Surefyre field from this list.

6. **Map Surefyre fields to columns in the import file:** Each selected field in the previous step will show up in the **Mapping** section. In the text field below each field, type or paste the column name from your import file that the field should be mapped to.

![](https://user-images.githubusercontent.com/31252743/36080015-b03d85f0-0f3e-11e8-80b4-08b7241d3739.png)
[zoom](https://user-images.githubusercontent.com/31252743/36080015-b03d85f0-0f3e-11e8-80b4-08b7241d3739.png)

> Example: Your data import file has two columns, "Business Lead Name" and "Business Phone Number". In the **Fields to Import** section you select the Surefyre fields "Business Name" and "phone number". In the **Mapping** section, you map the Surefyre fields to columns in the import file by copying and pasting the "Business Lead Name" and "Business Phone Number" column names into the text boxes below "Business Lead Name" and "Business Phone Number", respectively.

7. Click **Next**

8. **Select Matching Fields:** Matching Fields are only needed to identify records in the import file that already exist in Surefyre. When a match is found, Surefyre will update the existing record instead of creating a new record. This means that data from the import file will overwrite data in the existing Surefyre record. If not Matching Fields are selected, every row in your input file will be treated as a new record.

![](https://user-images.githubusercontent.com/31252743/36080640-a2ff07de-0f47-11e8-8cc2-f2f408c6919c.png)
> Example: You select "License #" as the **matching field** for a business account import. When Surefyre finds a business account in your system with a License Number that matches an account in the import file, it will update that account record with the data from the import file for that account.

8. Click **Next** to navigate to the Import Screen. Continue on **Step 3** of [Import Data from an Existing Source](https://github.com/surefyresystems/Surefyre-Systems/wiki/Data-Importer/_edit#import-data-from-an-existing-source).

***

# Import Data from an Existing Source
Follow these steps to import data using an existing **Import Configuration**:

1. Click **Create (+)** > **Import Data** to open the Surefyre Data Importer

![](https://user-images.githubusercontent.com/31252743/36079943-9f83f164-0f3d-11e8-8b97-9e7aae8dc2f9.png)

2. Select an existing Import Configuration from the list.

3. **Upload csv import file:** On the Import Screen you will see a summary of the selected Surefyre fields to upload, their mapped column names, any selected Matching Fields, and an **Imports** section where you can upload import csv files. Tap to search and select or drag and drop your import CSV file into the **Imports** section. All uploaded import files for this configuration will show in a list in this section. Find the uploaded import file that you want to import and click the **Run** button.

![](https://user-images.githubusercontent.com/31252743/36080639-a2eb2430-0f47-11e8-9811-68231c6a2ce1.png)
[zoom](https://user-images.githubusercontent.com/31252743/36080639-a2eb2430-0f47-11e8-9811-68231c6a2ce1.png)

4. **Execute import:** Surefyre will ask if you want to start a Dry Run or an Import:
* **Start Dry Run** will simulate an import without actually create or updating an data. This helps users identify errors or bad data without having committing changes that might need to be undone.
* **Start Import** will execute the import. You will see a notice that your import has begun and will receive an email when it is complete.

![](https://user-images.githubusercontent.com/31252743/36080638-a2d35e5e-0f47-11e8-9160-20a821403a21.png)

5. Once an import has been executed you will see a record with details appear in the **Imports** section. At a glance you can see counts of **New** records created, **Updated** records, **Skipped** records, and record that returned an **Error**.

![](https://user-images.githubusercontent.com/31252743/36081329-249fae4c-0f52-11e8-8f65-2f07ae2aa682.png)

6. Click the **info** icon to see a more detailed view of the import. Here you can see each individual record and its status. You can also see previous and new values of existing Surefyre records whose data was overwritten by the import. Each field of the import can be searched / filtered by entering a value at the top of the respective column.

![](https://user-images.githubusercontent.com/31252743/36081328-248baf96-0f52-11e8-89cd-6061d81814b3.png)


