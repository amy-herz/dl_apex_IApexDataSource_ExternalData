# dl_apex_IApexDataSource_ExternalData
Each sample in this collection is a single, standalone file, meant to be implmented from a Developer Console in Salesforce. 

These samples demonstrate how to implement the `IApexDataSource` and `ExternalData` class to provide data for use in Document Packages with the Nintex Drawloop app.

## ExternalData sample

The sample is a single file, named ExternalData.java. 

Demonstrates how to implement the `IApexDataSource` interface and use the other inner classes included with the `ExternalData` class to gather data from an external service for use within Drawloop.

### Implementing ExternalData sample

To implement the sample

1. Log into your Salesforce instance, using a Developer Edition account.
2. In a text editor, open the sample file named ExternalData.java.
3. From your Salesforce instance, open the Developer Console. 
4. From the Developer Console, create a new Apex class named `ExternalDataService`.
5. Select the code for the `ExternalDataService` class from the sample file, copy the selected code, and then paste the code into the Developer Console, overwriting the existing contents.
6. Save the new Apex class.
7. From the Developer Console, create a new Apex class named `ExternalData`.
8. Select the code for the `ExternalData` class from the sample file, copy the selected code, and then paste the code into the Developer Console, overwriting the existing contents.
9. Save the new Apex class, and then close the Developer Console.

## OppLineItemGrouping sample

The sample is a single file, named OppLineItemGrouping.java.

Demonstrates how to implement the `IApexDataSource` interface to provide an external data source that can present Salesforce objects by using a custom grouping.

### Implmenting OppLineItemGrouping sample

To implement the sample

1. Log into your Salesforce instance, using a Developer Edition account.
2. In a text editor, open the sample file named OppLineItemGrouping.java.
3. From your Salesforce instance, open the Developer Console.
4. From the Developer Console, create a new Apex class named `OppLineItemGrouping`.
5. Paste the contents of the sample file into the Developer Console, overwriting the existing contents
6. Save the new Apex class, and then close the Developer Console.

## SampleDrawloopApexData1SFObject sample

The sample is a single file, named SampleDrawloopApexData - 1 Sf Object.java.

Demonstrates how to implement the `IApexDataSource` interface to provide data for an Apex Data relationship. In this sample, the data comes from a single Salesforce object.

### Implmenting SampleDrawloopApexData1SFObject sample

To create the Apex class

1. Log into your Salesforce instance.
2. From your Salesforce instance, open the Developer Console.
3. From the Developer Console, create a new Apex class named `SampleDrawloopApexData1SFObject`.
4. Paste the contents of the sample file (SampleDrawloopApexData - 1 Sf Object.java) into the Developer Console, overwriting the existing contents.
5. Save the new Apex class, and then close the Developer Console.

To create the Apex Data relationship

1. In Nintex Drawloop, from **Drawloop Document Packages**, create a new Document Package based on the Opportunity object.
2. From the new Document Package, in the Relationships related list, add an Apex Data relationship.
3. In the Apex Data relationship, from Apex Class, select **--No Namespace--** and **SampleDrawloopApexData1SFObject**.
4. In **Relationship (What you want)**, select **ApexOpportunity**.
5. Save the Apex Data relationship.

## SampleDrawloopApexData1SFObjectTest  sample

The sample is a single file, named SampleDrawloopApexDataTest - 1 Sf Object.java.

Demonstrates how to create a test class for `SampleDrawloopApexData1SFObject`. 

**Note**: Implement this code only after you implement the SampleDrawloopApexData1SFObject sample.  

### Implmenting SampleDrawloopApexData1SFObjectTest sample

To create the Apex test class

1. Log into your Salesforce instance.
2. From your Salesforce instance, open the Developer Console.
3. From the Developer Console, create a new Apex class named `SampleDrawloopApexData1SFObjectTest`.
4. Paste the contents of the sample file (SampleDrawloopApexDataTest - 1 Sf Object.java) into the Developer Console, overwriting the existing contents.
5. Save the new Apex class, and then close the Developer Console.
## SampleDrawloopApexDataQuery sample

The sample is a single file, named SampleDrawloopApexData - 1 Sf Query.java.

Demonstrates how to implement the `IApexDataSource` interface to provide data for a Document Package using an Apex Data relationship. In this sample, the data comes from a SOQL query. 

### Implmenting SampleDrawloopApexDataQuery sample

To create the Apex class

1. Log into your Salesforce instance.
2. From your Salesforce instance, open the Developer Console.
3. From the Developer Console, create a new Apex class named `SampleDrawloopApexDataQuery`.
4. Paste the contents of the sample file (SampleDrawloopApexData - 1 Sf Query.java) into the Developer Console, overwriting the existing contents.
5. Save the new Apex class, and then close the Developer Console.

To create the Apex Data relationship

1. In Nintex Drawloop, from **Drawloop Document Packages**, create a new Document Package based on the Opportunity object.
2. From the new Document Package, in the Relationships related list, add an Apex Data relationship.
3. In the Apex Data relationship, from Apex Class, select **--No Namespace--** and **SampleDrawloopApexDataQuery**.
4. In **Relationship (What you want)**, select **ApexSoql**.
5. Save the Apex Data relationship.

## SampleDrawloopApexData sample

The sample is a single file, named SampleDrawloopApexData.java.

Demonstrates how to implement the `IApexDataSource` interface to provide data for a Document Package using an Apex Data relationship. In this sample, the data comes from three field sets that you create before you implement the class and a SQQL query. 

### Implmenting SampleDrawloopApexData sample

To create the field sets

1. From **Setup**, enter *Field Sets* in the **Quick Find** box, then under Accounts, click **Field Sets** to display a list of the field sets on the Account object in your organization.
2. Click **New**.
3. In **Field Set Label**, type *SampleApexDataFieldSet*
4. In **Field Set Name**, use *SampleApexDataFieldSet* (the same name).
5. In **Where is this used?**, type *This field set is for the SampleDrawloopApexData class.*
6. Click **Save**.
7. In the field set editor, add the fields from this object for the data that you want to make available in your Document Package.
8. Repeat steps 1 through 7 to create field sets on **Opportunity** and **Opportunity Products** objects. Use the same values in **Field Set Label**, **Field Set Name**, and **Where is this used?**. Specify whatever fields seem useful to your organization in the field sets themselves.

To create the Apex class

1. Log into your Salesforce instance.
2. From your Salesforce instance, open the Developer Console.
3. From the Developer Console, create a new Apex class named `SampleDrawloopApexData`.
4. Paste the contents of the sample file (SampleDrawloopApexData.java) into the Developer Console, overwriting the existing contents.
5. Save the new Apex class, and then close the Developer Console.

To create the Apex Data relationship

1. In Nintex Drawloop, from **Drawloop Document Packages**, create a new Document Package based on the Opportunity object.
2. From the new Document Package, in the Relationships related list, add an Apex Data relationship.
3. In the Apex Data relationship, from Apex Class, select **--No Namespace--** and **SampleDrawloopApexData**.
4. In **Relationship (What you want)**, select one of the following:
   * **ApexAccount**: Fields in the *SampleApexDataFieldSet* field set on the Account object.
   * **ApexOppLineItem**: Fields in the *SampleApexDataFieldSet* field set  on the Opportunity Products object.
   * **ApexOpportunity**: Fields in the *SampleApexDataFieldSet* field set on the Opportunity object.  
   * **ApexSoql**: Contacts associated with the account with the letter "C" in their title. 
5. Save the Apex Data relationship.
