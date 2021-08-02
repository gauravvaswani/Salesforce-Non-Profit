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