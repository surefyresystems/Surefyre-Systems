---
layout: page
title: Create DocGen Templates
wikiPageName: Create-DocGen-Templates
menu: wiki
---

_Page currently under construction..._

The DocGen is a powerful tool that allows users to automatically fill and send lengthy documents such as ACORD forms with just a few clicks. Before users can generate these documents, document templates must be defined by their administrator. These templates define the mapping between fields in the document and fields in Surefyre. For example, the template will define that the **Carrier** field in an ACORD form should be populated by the carrier associated to the policy.

1. **Start with a fillable PDF form** - To create a template you must first start with a PDF version of the document with [fillable fields](https://acrobat.adobe.com/us/en/acrobat/how-to/create-fillable-pdf-forms-creator.html). Depending on the document that you'd like to create this might be easily found online or created manually with a PDF editing tool like [Adobe Acrobat](https://acrobat.adobe.com/us/en/acrobat.html) [(fillable forms tutorial)](https://helpx.adobe.com/acrobat/how-to/convert-word-excel-paper-pdf-forms.html). 

2. **Ensure all necessary fields exist in Surefyre** - Your Surefyre system is likely already configured to accommodate all the data you normally collect. Common fields like insured name, contact information, policy number, insurer, etc. exist by default. But, if there are additional fields that make sense to have in Surefyre, you can easily add them by following instructions for [creating custom fields](https://github.com/surefyresystems/Surefyre-Systems/wiki/Custom-Fields). For this tutorial, create a **Policy** currency field called **Health Election**. 

3. **Create a Template PDF Doc** - Once you have your fillable form and have created any necessary fields, it's time to create your template. Click **Setup (gear)** > **Admin** > **Template PDF Docs**
