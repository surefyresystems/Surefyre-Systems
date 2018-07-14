This tutorial explains how to map PDF form fields to Surefyre fields by creating a DocGen PDF Template. These templates can be used in the DocGen to auto-fill forms that can easily be saved or emailed to carriers and clients.


1. Click **Setup (gear)** > **Admin** > **Template PDF Docs**

2. Click **+ Add Template PDF Doc**

3. Enter a **Name** for reference, in this case "Section 125 Cafeteria Plan Elections Form". Click **Choose File** and select the fillable PDF form from your computer. For this tutorial we will be using a simplified [Section 125 Cafeteria Plan Elections Form](https://github.com/surefyresystems/Surefyre-Systems/files/1694297/SECTION.125.CAFETERIA.PLAN.ELECTION.FORM.FILLABLE.pdf). Ensure that the **Primary Content Type** is set to **Account**.

4. Click **Save and Continue Editing**

5. The template has now been created and all fillable fields are now represented in the **Doc Fields** section. This is where you will define the mapping between the PDF form fields and Surefyre fields.

6. **Ensure all necessary fields exist in Surefyre** - You can easily add them by following instructions for [creating custom fields](https://github.com/surefyresystems/Surefyre-Systems/wiki/Custom-Fields). For this tutorial, create a **Policy** currency field called **Health Election**. 

Accounts in Surefyre can have different types of information associated to them such as people or policies. This kind of information is referred to as **Additional Content Types**. For example:
> An Additional Content Type of **Person** could be a an employee that is part of a group plan, a dependent, a business contact, or any other person that is associated to an account.
> An Additional Content Type of **Policy** could be a group health, general liability, or any other type of policy associated to an account.  

The Surefyre DocGen has the ability to generate forms with all of this type of information but it must be identified in the template. In our Section 125 example, there is employee information on the form so we will need to identify one Additional Content Type of Person. There is also election information that is tied to a specific policy (Health plan pre-tax election).

7. **Create any needed Additional Content Types** - Navigate back to the **Admin** page and click **Additional Content Types**.

8. Click **+ Add Additional Content Type**

9. Name the content type **Insured** in this case since it will be used to identified the insured person on the form. Set **Content Type** to **person** since the insured is a person. Click **Save and Add Another**

10. Name the second content type **Policy** since we want to simply specify a policy to pull data from for the form. Click **Save**.

11. **Map Fields** - Navigate back to the **Admin** page and click **Template PDF Docs** and click **Section 125 Cafeteria Plan Elections Form** to continue editing the template.

12. Under **Additional Data** you will now find our two recently created content types: **Insured** and **Policy**. Select them both from the left hand / available column and click the **right arrow** to move them to the right hand / chosen column. Clikc **Save and Continue Editing**.

13. You can now begin mapping fields. Before you begin, click the **Download Template** button in the top right corner of the page. View the PDF file to see all fillable fields populated with their field names. This is a great way to quickly understand what each PDF field is named so you can map is to the correct field in Surefyre. All of these fields were automatically detected by Surefyre when the template was created. Take note of the **Employee Name** field. Navigate back to the template.

14. In the **Doc Field** section, scroll to the Doc Field titled **Employee Name**. We know this field should display the insured employee's name. In the **Value** column you can use hashtag search to quickly find any available Surefyre field to map to the **Employee Name** PDF field. In this case we want to map it to a field from the Additional Content Type of **Insured** since it's the person's name and that content type identifies a person on the account. Type "#insured:" to see a list of all available person fields. Select **Insured: First Name**, notice that the appropriate reference text was placed into the **Value** field. Next type "#middle name" to show all fields of any content type that match that search criteria. Select **Insured: Middle Name**. Finally, search and select **Insured: Last Name**. When used in the DocGen this field will now dynamically pull the first, middle, and last name of the selected person.The final mapping should look like this:
> {{Insured.first_name}} {{Insured.middle_name}} {{Insured.last_name}} 

15. Repeat the same steps for **Phone**, **Birth Date**, and **SSN**

16. In the **Doc Field* section, scroll to the Doc Field titled **health_amount**. If you reference the downloaded template file again, you'll see that this field represents the pre-tax election that the person has made for this policy. We'll map this to our recently created custom field called **Health Election**. Type "#health election" and select the field, ensuring that the content type is **Policy**. The **Value** field should look like this:
> {{Policy.Health_Election}} 

Your DocGen template is now available to users. When they choose to generate this document, they will be prompted to select a person (for the **Insured**) and a policy (for the **Policy**). 

***

Related:
* Generate Documents with the DocGen