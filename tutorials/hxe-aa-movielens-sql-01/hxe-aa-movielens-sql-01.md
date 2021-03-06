---
title: Check your environment
description: Check your environment before starting the MovieLens tutorial series for SAP HANA, express edition
auto_validation: true
primary_tag: topic>machine-learning
tags: [ tutorial>beginner, products>sap-hana\, express-edition, topic>machine-learning ]
---

## Prerequisites
 - **Proficiency:** Beginner

## Details
### You will learn

- Which flavor and version of SAP HANA, express edition is needed to complete this tutorial series
- Complete a series of required post-installation task
- Enable the builders for the development space
- Add a connection in the Database Explorer
- Enable the Script Server to allow the execution of `AFL`s functions

### Time to Complete
**20 Min**

[ACCORDION-BEGIN [Info: ](Which SAP HANA flavor and version?)]

In order to complete this tutorial series, you need to use as a minimum version:

 - **SAP HANA, express edition 2.0 SPS03**

This version will allow you to complete all the steps described in the series. And thanks to the availability of the SAP HANA Automated Predictive Library (APL), you will be able to compare different predictive libraries.

As you may already know, SAP HANA, express edition comes in two different flavors. In this series, you will be running series of SQL statements. Therefore, you will need:

 - **Server only**

You can check the [SAP HANA, express edition installation flowchart](https://www.sap.com/developer/topics/sap-hana-express.html#flowchart) to find all the installation details.

If you don't have an instance up and running, be aware that you don't need to complete the installation of all optional packages (this will be described when needed).

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 1: ](Prepare your System)]

In order to complete this series, you will first need to prepare your instance to execute Machine Learning algorithms.

Complete the following group:

- [Prepare your SAP HANA, express edition instance for Machine Learning](https://www.sap.com/developer/tutorials/mlb-hxe-setup-basic.html)

As you will mostly execute SQL commands during this series, you will need to setup a SQL query tool for SAP HANA, express edition as describe in the following tutorial group:

 - [Select, install and configure a SQL query tool for SAP HANA, express edition](https://www.sap.com/developer/groups/mlb-hxe-tools-sql.html).

Off course you can use any tool of your choice, like Jupyter (as described in the following [tutorial](Use Jupyter Notebook with SAP HANA, express edition)).

Finally, you don't need to setup all of them, but one is enough.

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 8: ](Check the installation)]

Connect to the **HXE** tenant using the **SYSTEM** user credentials and execute the following SQL statement:

```sql
SELECT SERVICE_NAME, PORT, ACTIVE_STATUS FROM SYS.M_SERVICES ORDER BY 1;
```

The result should return a list of service names, their associated port numbers and their statuses including an entry for the `scriptserver`.

Provide an answer to the question below then click on **Validate**.

[VALIDATE_1]
[ACCORDION-END]
