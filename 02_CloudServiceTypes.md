# Introduce
## 1. Public Cloud
> The public cloud is defined as computing service offered by third-party provider over the public Internet,
 making them available to anyone who wants to use or purchase them.
## 2. Private Cloud
> The private cloud is defined as computing service offered either over the Internet or private internal network
>  and only to select users instead of the general public. 
## 3. Hybrid Cloud
> The hybrid cloud is a computing environment that combines a private cloud with a public cloud.

Example
```mermaid
---
title: SQL Stretch Database
---
    flowchart LR
        ua(User Application)
        ldb[("`On-Premies Local Database
								Hot data
								Cold data`")]
        azdb[("`Azure SQL Stretch Database
        Cold data`")]
								ua --"T-SQL Queries"--> ldb
								ldb <--"Smart query processing"--> azdb
								ldb <--"Eligible data"--> azdb
```
# Compare and contrast
||Public Cloud|Private Cloud|Hybrid Cloud|
|-------------|-------------|-------------|-------------|
|Accessibility|Everyone purchase service|Authorized users|Authorized users and their customers|
