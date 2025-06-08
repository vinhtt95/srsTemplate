# **Business Requirements**

## **Background**

Employees at the company Process Impact presently spend an average of 65 minutes per day going to the cafeteria to select, purchase, and eat lunch. About 20 minutes of this time is spent walking to and from the cafeteria, selecting their meals, and paying by cash or credit card. When employees go out for lunch, they spend an average of 90 minutes off-site. Some employees phone the cafeteria in advance to order a meal to be ready for them to pick up. Employees don’t always get the selections they want because the cafeteria runs out of certain items. The cafeteria wastes a significant quantity of food that is not purchased and must be thrown away. These same issues apply to breakfast and supper, although far fewer employees use the cafeteria for those meals than for lunch.

## **Business Opportunity**

Many employees have requested a system that would permit a cafeteria user to order meals (defined as a set of one or more food items selected from the cafeteria menu) on line, to be picked up at the cafeteria or delivered to a company location at a specified time and date. Such a system would save employees time, and it would increase the chance of their getting the items they prefer. Knowing what food items customers want in advance would reduce wastage in the cafeteria and would improve the efficiency of cafeteria staff. The future ability for employees to order meals for delivery from local restaurants would make a wide range of choices available to employees and provide the possibility of cost savings through volume discount agreements with the restaurants.

## **Business Objectives**

BO-1: Reduce the cost of cafeteria food wastage by 40% within 6 months following initial release.

Scale: Cost of food thrown away each week by cafeteria staff

Meter: Examination of Cafeteria Inventory System logs

Past: 33% (2013, initial study)

Goal: Less than 20%

Stretch: Less than 15%

BO-2: Reduce cafeteria operating costs by 15% within 12 months following initial release.

BO-3: Increase average effective work time by 15 minutes per cafeteria-using employee per day within 6 months following initial release.

## **Success Metrics**

SM-1: 75% of employees who used the cafeteria at least 3 times per week during Q3 2013 use the COS at least once a week within 6 months following initial release.

SM-2: The average rating on the quarterly cafeteria satisfaction survey increases by 0.5 on a scale of 1 to 6 from the Q3 2013 rating within 3 months following initial release and by 1.0 within 12 months.

## **Vision Statement**

For employees who want to order meals from the company cafeteria or from local restaurants on-line, the Cafeteria Ordering System is an Internet-based and smartphone-enabled application that will accept individual or group meal orders, process payments, and trigger delivery of the prepared meals to a designated location on the Process Impact campus. Unlike the current telephone and manual ordering processes, employees who use the Cafeteria Ordering System will not have to go to the cafeteria to get their meals, which will save them time and will increase the food choices available to them.

## **Business Risks**

RI-1: The Cafeteria Employees Union might require that their contract be renegotiated to reflect the new employee roles and cafeteria hours of operation. (Probability = 0.6; Impact = 3)

RI-2: Too few employees might use the system, reducing the return on investment from the system development and the changes in cafeteria operating procedures. (Probability = 0.3; Impact = 9)

RI-3: Local restaurants might not agree to offer delivery, which would reduce employee satisfaction with the system and possibly their usage of it. (Probability = 0.3; Impact = 3)

RI-4: Sufficient delivery capacity might not be available, which means that employees would not always receive their meals on time and could not always request delivery for the desired times. (Probability = 0.5; Impact = 6).

##  **Business Assumptions and Dependencies**

AS-1: Systems with appropriate user interfaces will be available for cafeteria employees to process the expected volume of meals ordered.

AS-2: Cafeteria staff and vehicles will be available to deliver all meals for specified delivery time slots within 15 minutes of the requested delivery time.

DE-1: If a restaurant has its own on-line ordering system, the Cafeteria Ordering System must be able to communicate with it bi-directionally.

# **Scope and Limitations**

## **Major Features**

FE-1: Order and pay for meals from the cafeteria menu to be picked up or delivered.

FE-2: Order and pay for meals from local restaurants to be delivered.

FE-3: Create, view, modify, and cancel meal subscriptions for standing or recurring meal orders, or for daily special meals.

FE-4: Create, view, modify, delete, and archive cafeteria menus.

FE-5: View ingredient lists and nutritional information for cafeteria menu items.

FE-6: Provide system access through corporate intranet, smartphone, tablet, and outside Internet access by authorized employees

**![FA-1.JPG](https://lh7-rt.googleusercontent.com/docsz/AD_4nXejZLBdCrNJg77Ql-rsGOZUR0SrR3lQGtTW4C3f_5qKVwClTmavSCis6o9FH70X9DKvoOsHZI9KuizNcOjj6IoIbwuq-WyPynTxyMi3Yp9-SRanq1Yk69JmoV1AWakKAZMfVnpqjP49N0e4yW3nng?key=v1EYETYO4E7oLFoGomjtfFLk)**

**Figure 1.** Partial feature tree for the Cafeteria Ordering System.

## **Scope of Initial and Subsequent Releases**

<table><tbody><tr><td><p style="text-align:center;"><strong>Feature</strong></p></td><td><p style="text-align:center;"><strong>Release 1</strong></p></td><td><p style="text-align:center;"><strong>Release 2</strong></p></td><td><p style="text-align:center;"><strong>Release 3</strong></p></td></tr><tr><td>FE-1, Order from cafeteria</td><td>Standard meals from lunch menu only; meal orders for delivery can be paid for only by payroll deduction</td><td>Accept credit and debit card payments</td><td>Accept meal orders for breakfasts and suppers</td></tr><tr><td>FE-2, Order from restaurants</td><td>Not implemented</td><td>Delivery to campus locations only</td><td>Fully implemented</td></tr><tr><td>FE-3, Meal subscriptions</td><td>Not implemented&nbsp;</td><td>Implemented if time permits</td><td>Fully implemented</td></tr><tr><td>FE-4, Menus</td><td>Create and view menus</td><td>Modify, delete, and archive menus</td><td>&nbsp;</td></tr><tr><td>FE-5, Ingredient lists</td><td>Not implemented</td><td>Fully implemented</td><td>&nbsp;</td></tr><tr><td>FE-6, System access</td><td>Intranet and outside Internet access</td><td>iOS and Android phone and tablet apps</td><td>Windows Phone and tablet apps</td></tr></tbody></table>

## **Limitations and Exclusions**

LI-1: Some food items that are available from the cafeteria will not be suitable for delivery, so the menus available to patrons of the COS must be a subset of the full cafeteria menus.

LI-2: The COS shall be used only for the cafeteria at the Process Impact campus in Clackamas, Oregon.

# **Business Context**

## **Stakeholder Profiles**

<table><tbody><tr><td><p style="text-align:center;"><strong>Stakeholder</strong></p></td><td><p style="text-align:center;"><strong>Major Value</strong></p></td><td><p style="text-align:center;"><strong>Attitudes</strong></p></td><td><p style="text-align:center;"><strong>Major Interests</strong></p></td><td><p style="text-align:center;"><strong>Constraints</strong></p></td></tr><tr><td>Corporate Management</td><td>Improved employee productivity; cost savings for cafeteria</td><td>Strong commitment through release 2; support for release 3 contingent on earlier results</td><td>Cost and employee time savings must exceed development and usage costs</td><td>None identified</td></tr><tr><td>Cafeteria Staff</td><td>More efficient use of staff time throughout the day; higher customer satisfaction</td><td>Concern about union relationships and possible downsizing; otherwise receptive</td><td>Job preservation</td><td>Training for staff in Internet usage needed; delivery staff and vehicles needed</td></tr><tr><td>Patrons</td><td>Better food selection; time savings; convenience</td><td>Strong enthusiasm, but might not use it as much as expected because of social value of eating lunches in cafeteria and restaurants</td><td>Simplicity of use; reliability of delivery; availability of food choices</td><td>Corporate intranet access, Internet access, or a mobile device is needed</td></tr><tr><td><p>Payroll</p><p>Department</p></td><td>No benefit; needs to set up payroll deduction registration scheme</td><td>Not happy about the software work needed, but recognizes the value to the company and employees</td><td>Minimal changes in current payroll applications</td><td>No resources yet committed to make software changes</td></tr><tr><td>Restaurant Managers</td><td>Increased sales; marketing exposure to generate new customers</td><td>Receptive but cautious</td><td>Minimal new technology needed; concern about resources and costs of delivering meals</td><td>Might not have staff and capacity to handle order levels; might not have all menus online</td></tr></tbody></table>

## **Project Priorities**

<table><tbody><tr><td><p style="text-align:center;"><strong>Dimension</strong></p></td><td><p style="text-align:center;"><strong>Constraint</strong></p></td><td><p style="text-align:center;"><strong>Driver</strong></p></td><td><p style="text-align:center;"><strong>Degree of Freedom</strong></p></td></tr><tr><td><strong>Features</strong></td><td>All features scheduled for release 1.0 must be fully operational</td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td><strong>Quality</strong></td><td>95% of user acceptance tests must pass; all security tests must pass</td><td>&nbsp;</td><td>&nbsp;</td></tr><tr><td><strong>Schedule</strong></td><td>&nbsp;</td><td>&nbsp;</td><td>release 1 planned to be available by end of Q1 of next year, release 2 by end of Q2; overrun of up to 2 weeks acceptable without sponsor review</td></tr><tr><td><strong>Cost</strong></td><td>&nbsp;</td><td>&nbsp;</td><td>budget overrun up to 15% accept able without sponsor review</td></tr><tr><td><strong>Staff</strong></td><td>&nbsp;</td><td>team size is half-time project manager, half-time BA, 3 developers, and 1 tester; additional developer and half-time tester available if necessary</td><td>&nbsp;</td></tr></tbody></table>

## **Deployment Considerations**

The web server software will need to be upgraded to the latest version. Apps will have to be developed for iOS and Android smartphones and tablets as part of the second release, with corresponding apps for Windows Phone and tablets to follow for the third release. Any corresponding infrastructure changes must be in place at the time of the second release. Videos no more than five minutes in length shall be developed to train users in both the Internet-based and app-based versions of COS.