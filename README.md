# SPLUNK-notes
in progress
*** Splunk has three main components, namely Forwarder, Indexer, and Search Head. These components are explained below ***

# forwarder
  Splunk Forwarder is a lightweight agent installed on the endpoint intended to be monitored, and its main task is to collect the data and send it to the Splunk instance. It does not affect the endpoint's performance as it takes very few resources to process. Some of the key data sources are
- Web server generating web traffic.
- Windows machine generating Windows Event Logs, PowerShell, and Sysmon data.
- Linux host generating host-centric logs.
- Database generating DB connection requests, responses, and errors.

# Splunk Indexer
Splunk Indexer plays the main role in processing the data it receives from forwarders. It takes the data, normalizes it into field-value pairs, determines the datatype of the data, and stores them as events. Processed data is easy to search and analyze.

# Search Head
plunk Search Head is the place within the Search & Reporting App where users can search the indexed logs. When the user searches for a term or uses a Search language known as Splunk Search Processing Language, the request is sent to the indexer and the relevant events are returned in the form of field-value pairs.
 Search Head also provides the ability to transform the results into presentable tables, visualizations like pie-chart, bar-chart and column-chart, as shown below:
![image](https://github.com/CYBERMEDIC1/SPLUNK-notes/assets/125709529/daef8d2c-227e-4a1a-9722-eafc673b0c46)

Search Head also provides the ability to transform the results into presentable tables, visualizations like pie-chart, bar-chart and column-chart, as shown below:

![image](https://github.com/CYBERMEDIC1/SPLUNK-notes/assets/125709529/0543d022-9ef8-48d5-9975-8582ecf00db3)

# Splunk Bar

When you access Splunk, you will see the default home screen identical to the screenshot below.

![image](https://github.com/CYBERMEDIC1/SPLUNK-notes/assets/125709529/4b5dd69b-2937-4c9a-a1e2-5eedfad545c3)

The ability to switch between installed Splunk apps instead of using the Apps panel can be achieved from the Splunk Bar, like in the image below.

![image](https://github.com/CYBERMEDIC1/SPLUNK-notes/assets/125709529/a38e126a-5875-42d9-8ad5-b084261c1a6b)


# Apps Panel

Next is the Apps Panel.  In this panel, you can see the apps installed for the Splunk instance. 

- The default app for every Splunk installation is Search & Reporting. 

![image](https://github.com/CYBERMEDIC1/SPLUNK-notes/assets/125709529/7e137ace-9a4e-47dd-9ed7-d17995f54271)



# Splunk Dashboard
By default, no dashboards are displayed. You can choose from a range of dashboards readily available within your Splunk instance. You can select a dashboard from the dropdown menu or by visiting the dashboards listing page.
- You can also create dashboards and add them to the Home Dashboard. The dashboards you create can be viewed isolated from the other dashboards by clicking on the Yours tab

Splunk documentation on Navigating Splunk : https://docs.splunk.com/Documentation/Splunk/8.1.2/SearchTutorial/NavigatingSplunk

# Adding Data
Splunk can ingest any data. As per the Splunk documentation, when data is added to Splunk, the data is processed and transformed into a series of individual events. 

- The data sources can be event logs, website logs, firewall logs, etc.

- Data sources are grouped into categories. Below is a chart listing from the Splunk documentation detailing each data source category.
![image](https://github.com/CYBERMEDIC1/SPLUNK-notes/assets/125709529/3cdfab75-3614-4c37-9298-9cc35805330a)

# VPN log file for splunk
[Uploading VPN-logs-1663593355154.json…]()



