# Salesforce.org Development

## Non-Profit Success Pack

- [Salesforce Non-Profit Success Pack Documentation](https://powerofus.force.com/s/article/NPSP-Documentation)
- [Salesforce.org Installer](https://install.salesforce.org/)
- [Salesforce Foundation NPSP](https://github.com/SalesforceFoundation/NPSP)

### Non-Profit Success Pack Post-Install Configurations

- [Required Configuration](https://powerofus.force.com/s/article/NPSP-Required-Configuration)
- [Recommended Configuration](https://powerofus.force.com/s/article/NPSP-Recommended-Configuration)
- Manual Steps 
    - [Assign Page Layouts](https://powerofus.force.com/s/article/NPSP-Required-Configuration#ariaid-title7)
    - [Assign the Organization Record Type to Profiles](https://powerofus.force.com/s/article/NPSP-Required-Configuration#ariaid-title6)
    - [Override Contact Delete Button](https://powerofus.force.com/s/article/NPSP-Required-Configuration#ariaid-title14)
    - [Override Lead Convert Button](https://powerofus.force.com/s/article/NPSP-Required-Configuration#ariaid-title10)
    - Manage Permission Set Assignment
        - Non-Profit Success Pack Permission
        - Gift Entry Recommended
        - NPSP Data Import
        - View Donations
        - View and Edit Donations
        - View and Edit Donations & Payments
    - CLI command to import Relationships - Relationship Reciprocal Settings:\
    `sfdx force:data:tree:import -p data/npsp-relationship-lookup/npe4__Relationship_Lookup__c-plan.json`

    ## Lightning Email Templates
    - Upgraded NPSP Opportunity Acknowledgment classic email template to lightning using Lightning Email Template Builder
    - [Lightning Email Template Builder](https://help.salesforce.com/s/articleView?id=sf.email_template_builder_parent.htm&type=5)<br/><br>
  >**How to deploy Lightning Email Templates?**
    - To deploy lightning email templates built with Email Template builder, Salesforce creates a FlexiPage of Type - EmailTemplatePage. ([FlexiPage Metadata](https://developer.salesforce.com/docs/atlas.en-us.api_meta.meta/api_meta/meta_flexipage.htm))
    - Retrieve and deploy the metadata for the Email Template Folder, Email Template and FlexiPage
    - Email Templates configured using Lightning Email Template Builder have the **_Made in Email Template Builder (IsBuilderContent)_** checkbox - **True**