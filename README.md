**SNStandardsFramework**
====================

This is a global app that can be used on ServiceNow to create a best practice/development standards framework

**Description:**
----------------

Ensuring good developments practices are followed is a challenge on ServiceNow space since the application does not provide any native support or adds any constraints in the system, that can stop/alert the developers from following bad practices. This becomes even more challenging if multiple vendors are involved in instance maintenance or development or if the team has members of varying experiences.

Over time, this results in increased maintenance cost of the system and inflated upgrade costs and efforts.

This application/framework is an attempt to reduce such risks and can be used by developers or implementer of the application to introduce constraints, development standards, naming standards, etc without much of an effort.


**Installation:**
-------------

*Install the updatesets found in dist folder* - SNStandardsFramework-V1.0 updateset creates the application and all the needed components in the instance. All the components that are being created are new and do not change any out of the box settings.

You can optionally, install the SNStandardsFramework-Test-Data updateset as well, to get some test constraints added to the system and you can use that for reference. 

**Usage:**
----------

**Note:** ***This is meant to be only used for development environment*** and do not install it on Production as the framework is still in development stage and some of the things built as part of this might show up on ACE report.

Once you have installed the application, you can access from the left navigation as 'ServiceNow Best Practices' application. Use the 'All' module to view all test data if you have also used the test-data update set. 

Since the framework basically uses 2 global scripts to run the entire thing, I have added some constraints that will make sure that those doesn't run for all the tables. The flipside of this would be, you will need to update the property *SN_Standards_Validator_Tables* that gets installed with the updateset and add table names manually if you are adding constraints for a newer table.



**License:**
--------
Standard MIT license.
