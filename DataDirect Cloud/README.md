##Introduction
<p align="justify">DataDirect Cloud is a powerful data connectivity service that provides a single point of universal data connectivity for all your data sources—wherever they are, in real time. You can connect to any of the Relational, Big Data or Cloud data sources even though they are behind the firewall and then you can use DataDirect Cloud's ODBC or JDBC or OData API to access the data anywhere, anytime.</p>

##Sign Up

 <a href="https://pacific.progress.com/console/register?productName=d2c">Sign up</a> for a 30 day trial account for Progress Data Direct Cloud, if you don't have an existing account.
 
##Getting Started Tutorial for DataDirect Cloud

###Configuring a DataSource

1. Login to DataDirect Cloud using your credentials that you just used to sign up.
2. On the Landing Page, you should see two options. One of them will be Progress DataDirect Cloud and it will have a button "Connect". Click on the "Connect" button to open the DataDirect Cloud dashboard.
3. On the dashboard, click on the Datasources tab that is present on left side as shown below.

    ![alt tag](https://s3.amazonaws.com/progressintegrate2016/1.png)
    
4. You should now see a view where it will have a button "New Data Source". Click on that button and it should show you group of supported data stores as shown below.

    ![alt tag](https://s3.amazonaws.com/progressintegrate2016/2.PNG)
    
5. Click on the data store that you want to use, and it should now open a new view where you can configure connection to your data source like Datasource name(Unique name for the connection), hostname, port, username, password etc,. Below is an example screenshot of how configuration page of Salesforce looks like. The configuration attributes may vary depending on the data source that you have selected.

    ![alt tag](https://s3.amazonaws.com/progressintegrate2016/3.PNG)
    
6. After you have entered all the required details for connections, you can test the connection by clicking on "Test Connection"  that you can see on top-right side of the view.

### Configuring OData for Datasource

7. Once you have successfully connected, click on the "OData" tab beside the "General" tab to configure the OData feed. Below is the screenshot, in case you weren't able to find it.

    ![alt tag](https://s3.amazonaws.com/progressintegrate2016/4.png)
    
8. Click on "Configure Schema" and you should see a new view that asks you to select schema. Select the schema that you want to enable the OData. On Select, you will see a new view where it shows all the tables that you have in your data source as shown below in the screenshot.

    ![alt tag](https://s3.amazonaws.com/progressintegrate2016/5.PNG)
    
9. You can select all the tables or select the tables that you want to access through OData. If a table doesn't have a Primary key defined on it, you have to select a column/group of columns that can be Primary key for that table. Without Primary key for a table OData will not be enabled for that table. 

10. After you have selected, just click on "Save&Close" button on top-right corner of the view which will validate your selection and saves it if everything is good.

11. You should now be back on the OData Tab, where you can find OData Access URI end point. Copy that and keep it aside.

12. Click on the "Save" button on top-right corner which saves all of your configuration for the datasource.

###Testing your OData URI endpoint

13. If you don't have Postman, you can <a href="https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en">download</a> it from Chrome store.

14. Open Postman and paste the OData Access URI for your datasource in address bar. 

15. Under Authorization tab select "Basic Authentication" and provide your DataDirect Cloud username and password. Now click on "Update Request" button to update the request. 

16. Click on send and you should see the entity names that you have selected when you configured OData in DataDirect Cloud dashboard. Following is a screenshot of Postman that illustrates how you should configure and how the response looks like for a Salesforce datasource that I have configured.
    ![alt tag](https://s3.amazonaws.com/progressintegrate2016/6.png)
    
###Video Tutorials
1. <a href="https://www.youtube.com/watch?v=HKbakiRHNuI">Getting started with DataDirect Cloud</a>
2. <a href="https://www.youtube.com/watch?v=3J6Jaex-PoQ">Configuring a Progress DataDirect Cloud data source for use with the OData API</a>

##Documentation for DataDirect Cloud OData API

1. <a href="http://documentation.progress.com/output/DataDirect/DataDirectCloud/index.html#page/odata%2Fservice-uri-and-resource-path.html%23">Service URI and resource paths</a>
2. <a href="http://documentation.progress.com/output/DataDirect/DataDirectCloud/index.html#page/odata%2Fformulating-queries.html%23">Querying with OData</a>

##Documentation for OData V2.0
1. <a href="http://www.odata.org/documentation/odata-version-2-0/uri-conventions/">URI Conventions (OData Version 2.0)</a>

##Contact Us
If you have any trouble with this setup, contact your nearest Progress DataDirect Cloud expert for help.
