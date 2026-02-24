---
title: "Active Directory Scraping"
date: 2022-05-01
draft: true
---

 One of the first tasks I took on after starting at MGM was replacing [this](http://www.cjwdev.com/Software/ADReportingTool/Info.html) AD Info report tool. As it stood, one of the IT employees would wake up around 5 am to boot the app up and run it for the different domains. This would take just over 8 hours, and tie her computer up with the whole process.

 I was given the scraps of a powershell script that would query users, but not in anyways wanted. So I designed a whole powershell module that does anything we could ever need to do with active directory scraping. The finished implementation scrapes all users, their groups, the nested groups, and other various AD properties, organizes and cleans it up, to return a nice set of CSV files containing sixty-thousand+ users.

 **Initial Setup**

TK: Starting parts and prep, up to pulling users

 ``` powershell

 ```

**Pulling Users**

TK: How users are gotten and returned
 ``` powershell

 ```

**Dealing with the data returned**

 TK: Data Manipulation, Multiple examples of the different functions that are used in order to clean itup
  ``` powershell

  ```


**Export**

  TK: Exporting all that data to spreadsheet
   ``` powershell

   ```
