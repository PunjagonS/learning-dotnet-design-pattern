# The Cool Shop project - Phase 1

**CoolShop** is a large retail shopping mall which has chain of mall's in Mumbai and Pune city.  
The company management wants a simple customer management system for their retail shops with the following features.  
Company has decided to launch the project in phases.

So in the first phase they just want to capture the customer information.  
Below is the requirement in more details:

1. Application would be capturing 5 fields for now: **Customer Name**, **Phone Number**, **Bill Amount**, **Bill Date**, and **Customer Address**.

2. In phase 1 two types of customer data are collected. One is the lead and the other is a customer.  
   - A **lead** is a person who comes to the Cool Shop but does not buy anything. He just enquires and goes away.  
   - A **customer** is a person who comes and buys things from the shop. A customer actually does a financial transaction.

3. When it’s a **lead**, only *Customer Name* and *Phone Number* are compulsory.  
   But for a **customer**, *all fields* are compulsory.  
   System should have a provision to add new validation rules seamlessly and these validation rules should be flexible and reusable to apply to the system.
   
4. System should have the ability to display, add, update and delete customer data.

5. For now the system will use SQL Server and ADO.NET as the data layer technology.  
   But in the coming months we would be migrating this data layer to Entity Framework.  
   Migration should be seamless without many changes across the system.
   
6. System should have the ability of cancelling any modification done on the screen.  
   So if the customer is editing a record and he has changed some values,  
   he should have the opportunity to revert back to the old values.
