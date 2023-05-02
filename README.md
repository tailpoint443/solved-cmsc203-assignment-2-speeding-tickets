Download Link: https://assignmentchef.com/product/solved-cmsc203-assignment-2-speeding-tickets
<br>
There are two types of speeding tickets in Maryland – “Payable” and “Must Appear”. “Payable” tickets can be paid by mail, in person or online. “Must Appear” tickets require the violator to appear at the County Court House in addition to paying a fine.

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Assignment Description</strong></td>

  </tr>

 </tbody>

</table>



















The DMV has asked you to build an application that will calculate the fees for a speeding tickets and then print a notice that will be mailed to the violator.

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Concepts tested by this assignment</strong></td>

  </tr>

 </tbody>

</table>
















<ul>

 <li>A driver and a utility class</li>

 <li>UML diagram, class diagrams</li>

 <li>Java fundamentals, including decision structures, loops</li>

 <li>Constructors, Overloaded constructors</li>

 <li>toString method</li>

 <li>Formatting output with DecimalFormat</li>

 <li>Random Class</li>

 <li>Java objects &amp; classes</li>

 <li>Following a Javadoc</li>

</ul>













<table width="100%">

 <tbody>

  <tr>

   <td><strong>Classes</strong></td>

  </tr>

 </tbody>

</table>




<strong> </strong>




<strong>Data Element Class </strong><strong>– Ticket </strong>

<ul>

 <li>Student Created</li>

 <li>Include private instance variables to store information needed for a ticket. Select the correct data types for each one. The speed and speed limit will be integers and that the school zone and work zone will be Boolean.</li>

 <li>A <strong>constructor</strong> that takes the name, speed, speed limit, school zone and work zone.</li>

 <li>Another <strong>constructor</strong> that takes the name, speed and speed limit. The school zone and work zone will be set to false.</li>

 <li>Getters and setters for the private instance variables.</li>

 <li>A public method <strong>calculateFine</strong> which calculates and returns the fine (as a double) based on the table in Assignment Details.</li>

 <li>A public method <strong>printNotice</strong> which returns a String with the contents of the Notice. Make sure that your fine is formatted in decimal format. Please see the Assignment Details for exact wording/format. Use your name instead of Professor Kartchner.</li>

 <li>A private method <strong>generateTicketNum</strong> which randomly generates a ticket number between 100000 and 999999 inclusively.</li>

 <li>A private method <strong>generateCourtDate</strong> which randomly generates a day between 1 and 31 inclusively. All court dates will take place in October 2018.</li>

 <li>A private method <strong>ticketType</strong> which returns a string of either “Payable” or “Must Appear” based on the table in Assignment Details.</li>

 <li>A <strong>toString</strong> method that returns a string representation of a Ticket, including the ticket number and ticket type. No specific format required.</li>

 <li>The method headers must match the Javadoc provided for you for the Ticket class.</li>

</ul>




<strong>Driver Class </strong><strong>– TicketDriver</strong>

<ul>

 <li>Student created</li>

 <li>This is the driver class for Ticket that contains a main method.</li>

 <li>The driver is responsible to:

  <ul>

   <li>print a header</li>

   <li>ask the user for information about a ticket.</li>

   <li>Print out the notice for that ticket using the methods from the Ticket class.</li>

   <li>Allow user to add another ticket.</li>

   <li>When user is finished entering tickets, prints “Exiting the Ticket Manager”</li>

   <li>Refer to the program sample run for more clarification.</li>

  </ul></li>

 <li>Data Validation. The following data must be validated:

  <ul>

   <li>Speed &gt; 0</li>

   <li>Speed Limit &gt;0 and &lt;= 80</li>

  </ul></li>

 <li>Add any necessary methods to modularize your code.</li>

</ul>

<strong> </strong>

<strong>GUI Driver Class </strong><strong>– TicketGUIDriver</strong>

<ul>

 <li>Provided</li>

 <li>Uses methods of the ticket class</li>

 <li>Use as a way to test your cacluateFine and printNotice methods</li>

 <li>Introduction to a Graphical User Interface (GUI) driver</li>

 <li>Include the dmv.jpg in the same package as your .java files for the image to display.</li>

</ul>

<strong> </strong>

<strong>Test Class </strong><strong>– TicketTestDriver</strong>

<ul>

 <li>Provided</li>

 <li>This is the driver class for testing the methods of the Ticket class. This has been given to you to help you test the methods of your Ticket class.</li>

</ul>













<table width="100%">

 <tbody>

  <tr>

   <td><strong>Assignment Details</strong></td>

  </tr>

 </tbody>

</table>










The fines will be based on the following:




Take screenshots of two runs of your program with different data.




Here is an example of the notice based on the following data:

Name: John Smith

Speed: 41

Speed Limit: 35

School Zone: Yes

Work Zone: No







Department of Motor Vehicles

Automated Traffic Enforcement







Dear John Smith,




Please pay the following speeding fine of $200.00 to the DMV within 10 days of

receiving this notice to avoid a driver’s license suspension. You are being fined

for going <strong>41</strong> MPH in a <strong>35</strong> MPH <strong>school</strong> zone.




Ticket Type: PAYABLE

Ticket Number: 482957




Returned checks are subject to a returned check fee of $35.00.




Sincerely,

Professor Kartchner (put your name here)










Here is an example of the notice based on the following data:

Name: Betty Boop

Speed: 58

Speed Limit: 25

School Zone: No

Work Zone: Yes







Department of Motor Vehicles

Automated Traffic Enforcement







Dear Betty Boop,




Please pay the following speeding fine of $450.00 to the DMV within 10 days of

receiving this notice to avoid a driver’s license suspension. You are being fined

for going <strong>58</strong> MPH in a <strong>25</strong> MPH <strong>work</strong> zone.




Ticket Type: MUST APPEAR

You must appear at the County Court House on October 5, 2018

Ticket Number: 936826




Returned checks are subject to a returned check fee of $35.00.




Sincerely,

Professor Kartchner (put your name here)




**Do not use color, this is for demo purposes only

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Examples/Sample Runs</strong></td>

  </tr>

 </tbody>

</table>













<strong>Sample 1 – shows multiple tickets being processed in one run</strong>

Ticket Manager




Enter the name of the violator: Poe Dameron

Enter the speed of the violator (&gt;0): 54

Enter the speed limit (&gt;0,&lt;=80): 30

Was this in a school zone (Y/N): N

Was this in a work zone (Y/N): N







Department of Motor Vehicles

Automated Traffic Enforcement







Dear Poe Dameron,




Please pay the following speeding fine of $495.00 to the DMV within 10 days of

receiving this notice to avoid a driver’s license suspension. You are being fined for going 54 MPH in a 30 MPH zone




Ticket Type: PAYABLE

Ticket Number: 161624




Returned checks are subject to a returned check fee of $35.00




Sincerely

Professor Kartchner







Do you want to enter another ticket? (Y/N)Y




Enter the name of the violator: Kylo Ren

Enter the speed of the violator (&gt;0): 86

Enter the speed limit (&gt;0,&lt;=80): 45

Was this in a school zone (Y/N): Y

Was this in a work zone (Y/N): N







Department of Motor Vehicles

Automated Traffic Enforcement







Dear Kylo Ren,




Please pay the following speeding fine of $675.00 to the DMV within 10 days of

receiving this notice to avoid a driver’s license suspension. You are being fined for going 86 MPH in a 45 MPH school zone




Ticket Type: MUST APPEAR

You must appear at the County Court House on October 16, 2018.

Ticket Number: 737022




Returned checks are subject to a returned check fee of $35.00




Sincerely

Professor Kartchner







Do you want to enter another ticket? (Y/N)N




Exiting the Ticket Manager




<strong>Sample 2 – shows validation loops</strong>




Ticket Manager




Enter the name of the violator: Han Solo

Enter the speed of the violator (&gt;0): -25

Enter the speed of the violator (&gt;0): 59

Enter the speed limit (&gt;0,&lt;=80): -20

Enter the speed limit (&gt;0,&lt;=80): 85

Enter the speed limit (&gt;0,&lt;=80): 45

Was this in a school zone (Y/N): yes

Was this in a school zone (Y/N): Y

Was this in a work zone (Y/N): no

Was this in a work zone (Y/N): N







Department of Motor Vehicles

Automated Traffic Enforcement







Dear Han Solo,




Please pay the following speeding fine of $310.00 to the DMV within 10 days of

receiving this notice to avoid a driver’s license suspension. You are being fined for going 59 MPH in a 45 MPH school zone




Ticket Type: PAYABLE

Ticket Number: 890645




Returned checks are subject to a returned check fee of $35.00




Sincerely

Professor Kartchner




Do you want to enter another ticket? (Y/N)N




Exiting the Ticket Manager







Example of Ticket GUI Driver:

<table width="100%">

 <tbody>

  <tr>

   <td></td>

  </tr>

 </tbody>

</table>




<table width="100%">

 <tbody>

  <tr>

   <td><strong>Deliverables</strong></td>

  </tr>

 </tbody>

</table>




<strong><u> </u></strong>

<strong><u> </u></strong>

<strong><u> </u></strong>

<strong><u> </u></strong>




<strong><u>Deliverables / Submissions</u></strong><strong>: </strong>

Design: UML class diagram with algorithm (pseudo-code) for methods

Implementation: Submit a compressed file containing the follow (see below):  The Java application (it must compile and run correctly); Javadoc files in a directory; a write-up as specified below.  Be sure to review the provided project rubric to understand project expectations.  The write-up will include:

<ul>

 <li>Test Cases

  <ul>

   <li>Prepare a test table with a list of test cases (expected versus actual results) that you are testing the application with. There must be at least 4 sets of valid data and at least one set of invalid data.</li>

   <li>Screenshots of at least two of the test cases in your test table.</li>

  </ul></li>

</ul>

<ul>

 <li>UML diagram</li>

 <li>In three or more paragraphs, highlights of your learning experience</li>

</ul>




<strong><u>Deliverable format</u></strong><strong>:</strong> The above deliverables will be packaged as follows. Two compressed files in the following formats:

<ul>

 <li>zip, a compressed file in the zip format, with the following:

  <ul>

   <li>Write up (Word document) – reflection paragraphs, test cases, screenshots</li>

   <li>UML Diagram – latest version (Word or jpg document)</li>

   <li>doc (directory) – Javadoc</li>

  </ul></li>

</ul>

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     <li style="list-style-type: none;">

      <ul>

       <li>File1.html (example)</li>

       <li>File2.html (example)</li>

      </ul></li>

    </ul></li>

  </ul></li>

</ul>

<ul>

 <li>src (directory)</li>

</ul>

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     <li style="list-style-type: none;">

      <ul>

       <li>File1.java (example)</li>

       <li>File2.java (example)</li>

      </ul></li>

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li>zip, a compressed file containing one or more Java files:

  <ul>

   <li>java (example)</li>

   <li>java (example)</li>

  </ul></li>

</ul>

This folder should contain Java source files only


