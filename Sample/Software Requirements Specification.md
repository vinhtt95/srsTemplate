# **Introduction**

## **Purpose**

This SRS describes the functional and nonfunctional requirements for software release 1.0 of the Cafeteria Ordering System (COS). This document is intended to be used by the members of the project team who will implement and verify the correct functioning of the system. Unless otherwise noted, all requirements specified here are committed for release 1.0.

## **Document Conventions**

No special typographical conventions are used in this SRS.

## **Project Scope and Product Features**

The COS will permit Process Impact employees to order meals from the company cafeteria on-line to be delivered to specified campus locations. A detailed description is available in the _Cafeteria Ordering System Vision and Scope Document_ \[1\], along with the features that are scheduled for full or partial implementation in this release.

## **References**

1.  Wiegers, Karl. _Cafeteria Ordering System Vision and Scope Document_, www.processimpact.com/projects/COS/COS Vision and Scope.docx
2.  Beatty, Joy. _Process Impact Intranet Development Standard, Version 1.3_, www.processimpact.com/corporate/standards/PI Intranet Development Standard.pdf
3.  Rath, Andrew. _Process Impact Internet Application User Interface Standard, Version 2.0_, www.processimpact.com/corporate/standards/PI Internet UI Standard.pdf

# **Overall Description**

## **Product Perspective**

The Cafeteria Ordering System is a new software system that replaces the current manual and telephone processes for ordering and picking up meals in the Process Impact cafeteria. The context diagram in Figure 1 illustrates the external entities and system interfaces for release 1.0. The system is expected to evolve over several releases, ultimately connecting to the Internet ordering services for several local restaurants and to credit and debit card authorization services.

**User Classes and Characteristics**

<table><tbody><tr><td>Patron (favored)</td><td>A Patron is a Process Impact employee who wants to order meals to be delivered from the company cafeteria. There are about 600 potential Patrons, of which 300 are expected to use the COS an average of 5 times per week each. Patrons will sometimes order multiple meals for group events or guests. An estimated 60 percent of orders will be placed using the corporate Intranet, with 40 percent of orders being placed from home or by smartphone or tablet apps.</td></tr><tr><td>Cafeteria Staff</td><td>The Process Impact cafeteria employs about 20 Cafeteria Staff, who will receive orders from the COS, prepare meals, package them for delivery, and request delivery. Most of the Cafeteria Staff will need training in the use of the hardware and software for the COS.</td></tr><tr><td>Menu Manager</td><td>The Menu Manager is a cafeteria employee who establishes and maintains daily menus of the food items available from the cafeteria. Some menu items may not be available for delivery. The Menu Manager will also define the cafeteria’s daily specials. The Menu Manager will need to edit existing menus periodically.</td></tr><tr><td>Meal Deliverer</td><td>As the Cafeteria Staff prepare orders for delivery, they will issue delivery requests to a Meal Deliverer's smartphone. The Meal Deliverer will pick up the food and deliver it to the Patron. A Meal Deliverer’s other interactions with the COS will be to confirm that a meal was (or was not) delivered.</td></tr></tbody></table>

## **Operating Environment**

OE-1: The COS shall operate correctly with the following web browsers: Windows Internet Explorer versions 7, 8, and 9; Firefox versions 12 through 26; Google Chrome (all versions); and Apple Safari versions 4.0 through 8.0.

OE-2: The COS shall operate on a server running the current corporate-approved versions of Red Hat Linux and Apache HTTP Server.

OE-3: The COS shall permit user access from the corporate Intranet, from a VPN Internet connection, and by Android, iOS, and Windows smartphones and tablets.

## **Design and Implementation Constraints**

CO-1: The system’s design, code, and maintenance documentation shall conform to the _Process Impact Intranet Development Standard, Version 1.3_ \[2\].

CO-2: The system shall use the current corporate standard Oracle database engine.

CO-3: All HTML code shall conform to the HTML 5.0 standard.

## **Assumptions and Dependencies**

AS-1: The cafeteria is open for breakfast, lunch, and supper every company business day in which employees are expected to be on site.

DE-1: The operation of the COS depends on changes being made in the Payroll System to accept payment requests for meals ordered with the COS.

DE-2: The operation of the COS depends on changes being made in the Cafeteria Inventory System to update the availability of food items as COS accepts meal orders.

# **System Features**

## **Order Meals from Cafeteria**

### **Description**

A cafeteria Patron whose identity has been verified may order meals either to be delivered to a specified company location or to be picked up in the cafeteria. A Patron may cancel or change a meal order if it has not yet been prepared. Priority = High.

### **Functional Requirements**

<table><tbody><tr><td colspan="2"><strong>Order.Place: Placing a meal order</strong></td></tr><tr><td>.Register:</td><td><p>The COS shall confirm that the Patron is registered for payroll deduction.</p><p>If the Patron is not registered for payroll deduction, the COS shall give the Patron options to register now and continue placing an order, to place an order for pickup in the cafeteria (but not for delivery), or to exit.</p></td></tr><tr><td>.Date:</td><td><p>The COS shall prompt the Patron for the meal date (see BR-8).</p><p>If the meal date is the current date and the current time is after the order cutoff time, the COS shall inform the patron that it’s too late to place an order for today. The Patron can either change the meal date or cancel the order.</p></td></tr><tr><td colspan="2"><strong>Order.Deliver: Delivery or pickup</strong></td></tr><tr><td>.Select:</td><td>The Patron shall specify whether the order is to be picked up or delivered.</td></tr><tr><td>.Location:</td><td>If the order is to be delivered and there are still available delivery times for the meal date, the Patron shall provide a valid delivery location.</td></tr><tr><td>.Notimes:</td><td>The COS shall notify the Patron if there are no available delivery times for the meal date. The Patron shall either cancel the order or indicate that he will pick up the order in the cafeteria.</td></tr><tr><td>.Times:</td><td>The COS shall display the remaining available delivery times for the meal date. The COS shall allow the Patron to request one of the delivery times shown, to change the order to be picked up in the cafeteria, or to cancel the order.</td></tr></tbody></table>

_\[Note: Functional requirements for reordering a meal and for changing and canceling meal orders are not provided in this example.\]_

## **Order Meals from Restaurants**

_\[Details are not provided in this example. Quite a lot of the functionality described under 3.1 Order Meals from Cafeteria could likely be reused, so this section should just specify the additional functionality that addresses the restaurant interface.\]_

## **Create, View, Modify, and Delete Meal Subscriptions**

_\[Details are not provided in this example.\]_

## **Create, View, Modify, and Delete Cafeteria Menus**

_\[Details are not provided in this example.\]_

# **Data Requirements**

## **Logical Data Model**

![Fig A-2.JPG](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdcvcQ2XWZD_IaQ43hSHtf7bXXXSMM5lmu2Q7n_YD5Ltn-8zs28z1n4m5R0-UG8Z4On2O2tTmpP30z7eSGltt_59emWY1V_k37CZffTJk1mSDkJ0RPmSut8g7l6SvjuJwwxUPKyORCs7njhQF67SUk?key=554e9WK70ZKsPIi5wX5NW6Xs)

**Figure . Partial data model for release 1.0 of the Cafeteria Ordering System.**

## **Data Dictionary**

<table><tbody><tr><td><p style="text-align:center;"><strong>Data Element</strong></p></td><td><p style="text-align:center;"><strong>Description</strong></p></td><td><p style="text-align:center;"><strong>Composition or Data Type</strong></p></td><td><p style="text-align:center;"><strong>Length</strong></p></td><td><p style="text-align:center;"><strong>Values</strong></p></td></tr><tr><td>delivery instruction</td><td>where and to whom a meal is to be delivered, if it isn't being picked up in the cafeteria</td><td><p>patron name</p><p>+patron phone number</p><p>+meal date</p><p>+delivery location</p><p>+delivery time window</p></td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td>delivery location</td><td>building and room to which an ordered meal is to be delivered</td><td>alphanumeric</td><td>50</td><td>hyphens and commas permitted</td></tr><tr><td>delivery time window</td><td>beginning time of a 15-minute range on the meal date during which an ordered meal is to be delivered;&nbsp;</td><td>time</td><td>hh:mm</td><td>local time; hh = 0-23 inclusive; mm = 00, 15, 30, or 45</td></tr><tr><td>employee ID</td><td>company ID number of the employee who placed a meal order</td><td>integer</td><td>6</td><td>&nbsp;</td></tr><tr><td>food item description</td><td>ext description of a food item on a menu</td><td>alphabetic</td><td>100</td><td>&nbsp;</td></tr><tr><td>food item price</td><td>pre-tax cost of a single unit of a menu food item</td><td>numeric, dollars and cents</td><td>dd.cc</td><td>&nbsp;</td></tr><tr><td>meal date</td><td>the date the meal is to be delivered or picked up</td><td>date, MM/DD/YYYY</td><td>10</td><td>default = current date if the current time is before the order cutoff time, else the next day; cannot be prior to current date</td></tr><tr><td>meal order</td><td>details about a meal a Patron ordered</td><td><p>meal order number</p><p>+ order date</p><p>+ meal date</p><p>+ 1:m{ordered food item}</p><p>+ delivery instruction</p><p>+ meal order status</p></td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td>meal order number</td><td>unique ID that COS assigns to each accepted meal order</td><td>integer</td><td>7</td><td>initial value is 1</td></tr><tr><td>meal order status</td><td>status of a meal order that a Patron initiated</td><td>alphabetic</td><td>16</td><td>incomplete, accepted, prepared, pending delivery, delivered, canceled</td></tr><tr><td>meal payment</td><td>information about a payment COS accepted for a meal</td><td><p>payment amount</p><p>+ payment method</p><p>+ transaction number</p></td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td>menu</td><td>list of food items available for purchase on a specific date</td><td><p>menu date</p><p>+ 1:m{menu food item}</p></td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td>menu date</td><td>the date for which a specific menu is available</td><td>date, MM/DD/YYYY</td><td>10</td><td>&nbsp;</td></tr><tr><td>menu food item</td><td>description of a menu item</td><td><p>food item description</p><p>+ food item price</p></td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td>order cutoff time</td><td>the time of day before which all meal orders for that date must be placed</td><td>time, HH:MM</td><td>5</td><td>&nbsp;</td></tr><tr><td>order date</td><td>the date on which a patron placed a meal order</td><td>date, MM/DD/YYYY</td><td>10</td><td>&nbsp;</td></tr><tr><td>ordered food item</td><td>one menu food item that a Patron requested as part of a meal order</td><td><p>menu food item</p><p>+ quantity ordered</p></td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td>patron</td><td>a Process Impact employee who is authorized to order a meal</td><td><p>patron name</p><p>+ employee ID</p><p>+ patron phone number</p><p>+ patron location</p><p>+ patron email</p></td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td>patron email</td><td>email address of the employee who placed a meal order</td><td>alphanumeric</td><td>50</td><td>&nbsp;</td></tr><tr><td>patron location</td><td>building and room numbers of the employee who placed a meal order</td><td>alphanumeric</td><td>50</td><td>hyphens and commas permitted</td></tr><tr><td>patron name</td><td>name of the employee who placed a meal order</td><td>alphabetic</td><td>30</td><td>&nbsp;</td></tr><tr><td>patron phone number</td><td>telephone number of the employee who placed a meal order</td><td>AAA-EEE-NNNN xXXXX for area code (A), exchange (E), number (N), and extension (X)</td><td>18</td><td>&nbsp;</td></tr><tr><td>payment amount</td><td>total price of an order in dollars and cents, calculated per BR-12</td><td>numeric, dollars and cents</td><td>dddd.cc</td><td>&nbsp;</td></tr><tr><td>payment method</td><td>how the Patron is paying for a meal he ordered</td><td>alphabetic</td><td>16</td><td>payroll deduction, cash, credit card, debit card</td></tr><tr><td>quantity ordered</td><td>the number of units of each food item that the Patron is ordering in a single meal order</td><td>integer</td><td>4</td><td>default = 1; maximum = quantity presently in inventory</td></tr><tr><td>transaction number</td><td>unique sequence number that COS assigns to each payment transaction</td><td>integer</td><td>12</td><td>&nbsp;</td></tr></tbody></table>

## **Reports**

### **Ordered Meal History Report**

<table><tbody><tr><td><p style="text-align:right;">Report ID:</p></td><td>COS-RPT-1</td></tr><tr><td><p style="text-align:right;">Report Title:</p></td><td>Ordered Meal History</td></tr><tr><td><p style="text-align:right;">Report Purpose:</p></td><td>Patron wants to see a list of all meals that he had previously ordered from the Process Impact cafeteria or local restaurants over a specified time period up to six months prior to the current date, so he can reorder a particular meal he liked.</td></tr><tr><td><p style="text-align:right;">Priority:</p></td><td>Medium</td></tr><tr><td><p style="text-align:right;">Report Users:</p></td><td>Patrons</td></tr><tr><td><p style="text-align:right;">Data Sources:</p></td><td>Database of previously placed meal orders</td></tr><tr><td><p style="text-align:right;">Frequency and Disposition;</p></td><td>Report is generated on demand by a Patron. Data in the report is static. Report is displayed on user's web browser screen on a computer, tablet, or smartphone. It can be printed if the display device permits printing.</td></tr><tr><td><p style="text-align:right;">Latency:</p></td><td>Complete report must be displayed to Patron within 3 seconds after it is requested.&nbsp;</td></tr><tr><td><p style="text-align:right;">Visual Layout:</p></td><td>Landscape mode</td></tr><tr><td><p style="text-align:right;">Header and Footer:</p></td><td>Report header shall contain the report title, Patron's name, and date range specified. If printed, report footer shall show the page number.</td></tr><tr><td><p style="text-align:right;">Report Body:</p></td><td><p>Fields shown and column headings:&nbsp;</p><ul><li>Order Number</li><li>Meal Date</li><li>Ordered From ("Cafeteria" or restaurant name)</li><li>Items ordered (list all items in the meal order, their quantity, and their prices)</li><li>Total Food Price</li><li>Tax</li><li>Delivery Charge</li><li>Total Price (sum of food item prices, tax, and delivery charge)</li></ul><p>Selection Criteria: date range specified by Patron, inclusive of end points</p><p>Sort Criteria: reverse chronological order</p></td></tr><tr><td><p style="text-align:right;">End-of-Report Indicator:</p></td><td>None</td></tr><tr><td><p style="text-align:right;">Interactivity:</p></td><td>Patron can drill down to see ingredients and nutritional information for each item in the order</td></tr><tr><td><p style="text-align:right;">Security Access Restrictions:</p></td><td>A Patron may retrieve only his own meal order history</td></tr></tbody></table>

_\[Note: Other COS reports are not provided in this example.\]_

## **Data Integrity, Retention, and Disposal**

DI-1: The COS shall retain Individual Patron meal orders for 6 months following the meal's delivery date.

DI-2: The COS shall retain menus for one year following the menu date.

# **External Interface Requirements**

## **User Interfaces**

UI-1: The Cafeteria Ordering System screen displays shall conform to the _Process Impact Internet Application User Interface Standard, Version 2.0_ \[3\].

UI-2: The system shall provide a help link from each displayed webpage to explain how to use that page.

UI-3: The webpages shall permit complete navigation and food item selection by using the keyboard alone, in addition to using mouse and keyboard combinations.

## **Software Interfaces**

SI-1: Cafeteria Inventory System

SI-1.1: The COS shall transmit the quantities of food items ordered to the Cafeteria Inventory System through a programmatic interface.

SI-1.2: The COS shall poll the Cafeteria Inventory System to determine whether a requested food item is available.

SI-1.3: When the Cafeteria Inventory System notifies the COS that a specific food item is no longer available, the COS shall remove that food item from the menu for the current date.

SI-2: Payroll System

The COS shall communicate with the Payroll System through a programmatic interface for the following operations:

SI-2.1: To allow a Patron to register and unregister for payroll deduction.

SI-2.2: To inquire whether a Patron is registered for payroll deduction.

SI-2.3: To inquire whether a Patron is eligible to register for payroll deduction.

SI-2.4: To submit a payment request for a purchased meal.

SI-2.5: To reverse all or part of a previous charge because a patron rejected a meal or wasn’t satisfied with it, or because the meal was not delivered per the confirmed delivery instructions.

## **Hardware Interfaces**

No hardware interfaces have been identified.

## **Communications Interfaces**

CI-1: The COS shall send an email or text message (based on user account settings) to the Patron to confirm acceptance of an order, price, and delivery instructions.

CI-2: The COS shall send an email or text message (based on user account settings) to the Patron to report any problems with the meal order or delivery.

# **Quality Attributes**

## **Usability Requirements**

USE-1: The COS shall allow a Patron to retrieve the previous meal ordered with a single interaction.

USE-2: 95% of new users shall be able to successfully order a meal without errors on their first try.

## **Performance Requirements**

PER-1: The system shall accommodate a total of 400 users and a maximum of 100 concurrent users during the peak usage time window of 9:00 A.M. to 10:00 A.M. local time, with an estimated average session duration of 8 minutes.

PER-2: 95% of webpages generated by the COS shall download completely within 4 seconds from the time the user requests the page over a 20Mbps or faster Internet connection.

PER-3: The system shall display confirmation messages to users within an average of 3 seconds and a maximum of 6 seconds after the user submits information to the system.

## **Security Requirements**

SEC-1: All network transactions that involve financial information or personally identifiable information shall be encrypted per BR-33.

SEC-2: Users shall be required to log on to the COS for all operations except viewing a menu.

SEC-3: Only authorized Menu Managers shall be permitted to work with menus, per BR-24.

SEC-4: The system shall permit Patrons to view only orders that they placed.

## **Safety Requirements**

SAF-1: The user shall be able to see a list of all ingredients in any menu items, with ingredients highlighted that are known to cause allergic reactions in more than 0.5 percent of the North American population.

## **Availability Requirements**

AVL-1: The COS shall be available at least 98% of the time between 5:00 A.M. and midnight local time and at least 90% of the time between midnight and 5:00 A.M. local time, excluding scheduled maintenance windows.

## **Robustness Requirements**

ROB-1: If the connection between the user and the COS is broken prior to a new order being either confirmed or terminated, the COS shall enable the user to recover an incomplete order and continue working on it.