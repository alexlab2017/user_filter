# User filter

How to __filter users__ based on the criteria *enabled* or *disabled*

## Active Directory Users and Computers

1. Menu: "View"

![](./images/image1.jpg)

2. Select: "Filter Options..."

![](./images/image2.jpg)

3. Choose: "Create custom filter" and Click: "Customize..."

![](./images/image3.jpg)

4. Select tab: "Advanced"

![](./images/image4.jpg)

5. Write: "Enter LDAP query:" (text in the subsections below)

![](./images/image5.jpg)

6. Click: "OK"
7. Click: "OK"


### Enabled users

    (!UserAccountControl:1.2.840.113556.1.4.803:=2)

### Disabled users

    UserAccountControl:1.2.840.113556.1.4.803:=2

Inspitarion for this guide took from [here](https://social.technet.microsoft.com/Forums/windowsserver/en-US/44048e98-b191-4d18-9839-d79ffad86f76/ldap-query-for-all-active-users?forum=winserverDS)
