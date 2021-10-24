/*
Author:- Dhirendra Singh
Date:- 21 October 2021
Description:- This document includes database info, scope and future scope of Assesment 'ShopBridge'.
*/

Database Info-
============================
Table- Category
============================
CategoryId
Name
Description
DeleteInd
CreatedUserId
ModifiedUserId
CreatedDate
ModifiedDate
============================
Table- Product
============================
ProductId
Name
Description
Price
AvailableStock
CategoryId	//Foreign key references Category
Url
DeleteInd
CreatedUserId
ModifiedUserId
CreatedDate
ModifiedDate

======================================
CustomerProduct  //Mapping of User(Customer) and product
======================================
CustomerProductId
UserId		//Foreign key references User
ProductId	//Foreign key references Product
DeleteInd
CreatedUserId
ModifiedUserId
PurchasedDate
ModifiedDate

============================
Table- Individual
============================
IndividualId
FirstName
LastName
DateOFBirth
EmailId
PhoneNumber
DeleteInd
CreatedUserId
ModifiedUserId
CreatedDate
ModifiedDate


===============================================================
Table- Role  //Admin User, Desk User, Customer, Supervisor, etc..
===============================================================
RoleId
Name
Description
DeleteInd
CreatedUserId
ModifiedUserId
CreatedDate
ModifiedDate

==========================================================
Table- RolePermission // Mapping of Role and Permission
==========================================================
RolePermissionId
RoleId			//Foreign key references Role
PermissionId		//Foreign key references Permission
DeleteInd
CreatedUserId
ModifiedUserId
CreatedDate
ModifiedDate

===========================================
Table- Permission  ---Read, Update, Delete
===========================================
PermissionId
Name
Description
DeleteInd
CreatedUserId
ModifiedUserId
CreatedDate
ModifiedDate

=======================
Table- User
=======================
UserId
IndividualId	//Foreign key references Individual
RoleId		//Foreign key references Role
Password
DeleteInd
CreatedUserId
ModifiedUserId
CreatedDate
ModifiedDate

==========================
Table- Audit
==========================
AuditId
UserId		//Foreign key references User
Description
AuditDate
AuditTime
DeleteInd



======================================================================
Scope- 
======================================================================
Default user- 'Product Admin', needs to authenticate and show him 
Inventory Management page on authenticate and autherize.

=====================================================================
Future Scope-
=====================================================================
A full fledged application that enables admin to manage user as per
operational requirement and customers to register/login to application.
Also enables customers to check already product availability
and checkout their product. It also facilitate admin/manager can
generate reports of activities of underlying users.

======================================================================
Software Used-
======================================================================
Visual Studio 2019----.Net 4.7.2 Framework
Microsoft Sql Server

======================================================================
/* Work History */
======================================================================
21-Oct-2021 Analysing and high level application design.
				
22-Oct-2021 initial code and completed Database script work- table structure
			and populate initial records.
23-Oct-2021 Implementation of Code.

24-Oct-2021 Testing, Documentation & Project Upload to Github

=======================================================================
Refer Assessment-ShopBridge.ppt for Screenshots
Feel free to reach out to me.

