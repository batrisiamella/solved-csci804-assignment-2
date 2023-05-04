Download Link: https://assignmentchef.com/product/solved-csci804-assignment-2
<br>
This assignment aims to establish a basic familiarity with C++ classes. The assignment introduce increasingly object-based, C++ style of solution to a problem.

<strong>General Requirements</strong>

<ul>

 <li>You should observe the common principles of OO programming when you design your classes.</li>

 <li>You should make proper documentation and implementation comments in your codes where they are necessary.</li>

 <li>Logical structures and statements are properly used for specific purposes.</li>

</ul>




<strong>Objectives</strong>

On completion of these tasks you should be able to:

<ul>

 <li>Code and run C++ programs using the development environment.</li>

 <li>Make effective use of the on-line documentation system that supports the development environment.</li>

 <li>Code programs using C++ in a hybrid style (procedural code using instances of simple classes) and in a more object-based style.</li>

 <li>Familiar with overloading operators.</li>

 <li>Understand class inheritance.</li>

</ul>




<strong>Tasks: </strong>

<strong>Task 1: (4 marks) </strong>

A complex number has the form

<h1>a + b i,</h1>

where <em>a</em>, <em>b</em> are real numbers,<em> i</em> is the imaginary unit, <em>i<sup>2</sup></em> = <em>-1</em>. It is very useful in mathematics, physics, engineering, economics.




In this task, you will define a class <strong>ComplexNumber</strong> in a file <strong>ComplexNumber.h</strong> and implement the C++ program code in a file <strong>ComplexNumber.cpp</strong>.

In the class <strong>ComplexNumber</strong>, declare data members to store a complex number. Define the following functions in the class ComplexNumber.

<ul>

 <li>In the class ComplexNumber, you will define default constructor, copy constructor and other necessary constructors;</li>

 <li>In the class ComplexNumber, define following overloading operators:

  <ul>

   <li>Extraction operator (&gt;&gt;) to get input values from keyboard; o Insertion operator (&lt;&lt;) to print out the a complex number; o Addition operator (+) to compute two complex numbers’ addition. The addition of two complex numbers is defined as: <em>c<sub>1 + </sub> c<sub>2 </sub>i = (a<sub>1</sub> +  a<sub>2</sub> i) + (b<sub>1 +</sub> b<sub>2 </sub>i), </em>where <em>c<sub>1</sub> = a<sub>1</sub>+b<sub>1</sub>, c<sub>2 </sub>= a<sub>2 </sub>+ b<sub>2</sub>.</em></li>

   <li>Addition assignment operator (+=) to compute two complex numbers’ addition. o Subtraction operation (-) to compute two complex numbers’ subtraction.</li>

  </ul></li>

</ul>

The subtraction of two complex numbers  is defined as:

<em>c<sub>1 + </sub> c<sub>2 </sub>i =( a<sub>1</sub> +  a<sub>2</sub> i ) – (b<sub>1 +</sub> b<sub>2 </sub>i), </em>where <em>c<sub>1</sub> = a<sub>1 </sub>– b<sub>1</sub>, c<sub>2 </sub>= a<sub>2 </sub>– b<sub>2</sub>.</em>

<ul>

 <li>Subtraction assignment operator (-=) to compute two complex numbers’ subtraction.</li>

 <li>Multiplication operator (*) to compute two complex numbers’ multiplication. The multiplication of two complex numbers is defined as:</li>

</ul>

<h1>c<sub>1 + </sub> c<sub>2 </sub>i =( a<sub>1</sub> +  a<sub>2</sub> i ) * (b<sub>1 +</sub> b<sub>2 </sub>i),</h1>

where <em>c</em><em>1</em><em> = a</em><em>1 </em><em>* b</em><em>1 – </em><em>a</em><em>2 * </em><em>b</em><em>2</em><em>, c</em><em>2 </em><em>= a</em><em>1 * </em><em>b</em><em>2 </em><em>+ a</em><em>2 * </em><em>b</em><em>1</em><em>.</em>

<ul>

 <li>Multiplication assignment operator (*=) to compute two complex numbers’ multiplication.</li>

 <li>Multiplication operator (*) to compute a complex number times a double value. The multiplication of a complex number is defined as: <em>c<sub>1 + </sub>c<sub>2 </sub>i =( a<sub>1</sub> +  a<sub>2</sub> i ) * b, </em>where <em>c<sub>1</sub> = a<sub>1 </sub>* b, c<sub>2 </sub>= a<sub>2 * </sub></em></li>

 <li>Multiplication operator (*) to compute a double value times a complex number. The multiplication of a double value times a complex number is defined as: <em>c<sub>1 + </sub> c<sub>2 </sub>i =b * ( a<sub>1</sub> +  a<sub>2</sub> i ), </em>where <em>c<sub>1</sub> = b * a<sub>1</sub>, c<sub>2 </sub>= b * a<sub>2 </sub>.</em></li>

 <li>Division operator (/) to compute two complex numbers’ division. The division of two complex numbers is defined as:</li>

</ul>

<h1>c<sub>1 + </sub> c<sub>2 </sub>i = ( a<sub>1</sub> +  a<sub>2</sub> i ) / (b<sub>1</sub> + b<sub>2</sub> i)</h1>

<em> = (( a<sub>1</sub> +  a<sub>2</sub> i ) / (b<sub>1</sub> – b<sub>2</sub> i))/ ((b<sub>1</sub> + b<sub>2</sub> i) * (b<sub>1</sub> – b<sub>2</sub> i)), </em>where <em>c<sub>1</sub> = (a<sub>1</sub>*b<sub>1</sub> + a<sub>2</sub> * b<sub>2</sub>)  / (b<sub>1</sub><sup>2</sup><sub>+</sub>b<sub>2</sub><sup>2</sup>), c<sub>2 </sub>= (a<sub>2</sub> * b<sub>1</sub> – a<sub>1</sub> * b<sub>2 </sub>) / (b<sub>1</sub><sup>2</sup><sub>+</sub>b<sub>2</sub><sup>2</sup>). </em><strong>The function should throw a string exception if the divisor is zero. </strong>

o Division assignment operator (/=) to compute two complex numbers’ division.

<strong>The function should throw a string exception if the divisor is zero. </strong>




Implement <strong>main()</strong> in a file <strong>task1Main.cpp</strong> to test the functions and operators that defined above (See the Testing examples of the task for more details). <strong>In the main() function, exceptions should be caught and message should be displayed.</strong>




<strong>Testing:  </strong>

<strong> </strong>

Use g++ to compile the source files on banshee by

$ g++ –o task1 task1Main.cpp ComplexNumber.cpp




You can test the task by using the data defined in a text file <strong>input1.txt</strong> by

$ ./task1 and input data that required. Your program will print out results like following (Red data means input from keyboard):




Input a complex number for cn1 :  10  4

Complex number cn1 = 10+4i

Input a complex number for cn2 :  5  2

Complex number cn2 = 5+2i

Complex number cn3 = cn1 + cn2 = 15+6i

Complex number cn3 = cn1 = 10+4i

Complex number cn3 += cn2 = 15+6i

Complex number cn3 = cn1 – cn2 = 5+2i

Complex number cn3 = cn1 = 10+4i

Complex number cn3 -= cn2 = 5+2i

Complex number cn3 = cn1 * cn2 = 42+40i

Complex number cn3 = cn1 = 10+4i

Complex number cn3 *= cn2 = 42+40i

Input a real number: 3.4

Complex number cn3 = cn1 * 3.4 = 34+13.6i

Complex number cn3 = 3.4 * cn1 = 34+13.6i

Complex number cn3 = cn1 / cn2 = 2

Complex number cn3 = cn1 = 10+4i

Complex number cn3 /= cn2 = 2




Testing example 2:




Input a complex number for cn1 : 6.3  -2.1

Complex number cn1 = 6.3-2.1i

Input a complex number for cn2 :  -2.1  1.0

Complex number cn2 = -2.1+i

Complex number cn3 = cn1 + cn2 = 4.2-1.1i

Complex number cn3 = cn1 = 6.3-2.1i

Complex number cn3 += cn2 = 4.2-1.1i

Complex number cn3 = cn1 – cn2 = 8.4-3.1i

Complex number cn3 = cn1 = 6.3-2.1i

Complex number cn3 -= cn2 = 8.4-3.1i

Complex number cn3 = cn1 * cn2 = -11.13+10.71i

Complex number cn3 = cn1 = 6.3-2.1i

Complex number cn3 *= cn2 = -11.13+10.71i Input a real number: -2.4

Complex number cn3 = cn1 * -2.4 = -15.12+5.04i

Complex number cn3 = -2.4 * cn1 = -15.12+5.04i

Complex number cn3 = cn1 / cn2 = -2.83364-0.349353i

Complex number cn3 = cn1 = 6.3-2.1i

Complex number cn3 /= cn2 = -2.83364-0.349353i




Testing example 3:




Input a complex number for cn1 : 3.75  0.0

Complex number cn1 = 3.75

Input a complex number for cn2 : 0.0  -2.5

Complex number cn2 = -2.5i

Complex number cn3 = cn1 + cn2 = 3.75-2.5i

Complex number cn3 = cn1 = 3.75

Complex number cn3 += cn2 = 3.75-2.5i

Complex number cn3 = cn1 – cn2 = 3.75+2.5i

Complex number cn3 = cn1 = 3.75

Complex number cn3 -= cn2 = 3.75+2.5i

Complex number cn3 = cn1 * cn2 = -9.375i

Complex number cn3 = cn1 = 3.75

Complex number cn3 *= cn2 = -9.375i

Input a real number: 1.25

Complex number cn3 = cn1 * 1.25 = 4.6875 Complex number cn3 = 1.25 * cn1 = 4.6875

Complex number cn3 = cn1 / cn2 = 1.5i

Complex number cn3 = cn1 = 3.75

Complex number cn3 /= cn2 = 1.5i




Testing example 4:




Input a complex number for cn1 : 0.0 0.0

Complex number cn1 = 0

Input a complex number for cn2 : 1.0 1.0

Complex number cn2 = 1+i

Complex number cn3 = cn1 + cn2 = 1+i

Complex number cn3 = cn1 = 0

Complex number cn3 += cn2 = 1+i

Complex number cn3 = cn1 – cn2 = -1-i

Complex number cn3 = cn1 = 0

Complex number cn3 -= cn2 = -1-i

Complex number cn3 = cn1 * cn2 = 0

Complex number cn3 = cn1 = 0

Complex number cn3 *= cn2 = 0

Input a real number: 3.0

Complex number cn3 = cn1 * 3 = 0 Complex number cn3 = 3 * cn1 = 0

Complex number cn3 = cn1 / cn2 = 0

Complex number cn3 = cn1 = 0

Complex number cn3 /= cn2 = 0




Testing example 5:




Input a complex number for cn1 : 2.5  -1.0

Complex number cn1 = 2.5-i

Input a complex number for cn2 : 0.0  0.0

Complex number cn2 = 0

Complex number cn3 = cn1 + cn2 = 2.5-i

Complex number cn3 = cn1 = 2.5-i

Complex number cn3 += cn2 = 2.5-i

Complex number cn3 = cn1 – cn2 = 2.5-i

Complex number cn3 = cn1 = 2.5-i

Complex number cn3 -= cn2 = 2.5-i

Complex number cn3 = cn1 * cn2 = 0

Complex number cn3 = cn1 = 2.5-i

Complex number cn3 *= cn2 = 0

Input a real number: 5.5

Complex number cn3 = cn1 * 5.5 = 13.75-5.5i

Complex number cn3 = 5.5 * cn1 = 13.75-5.5i Exception : Division by zero.




<strong>Note:</strong> Your program should work on different testing data. <strong> </strong>

<strong> </strong>

<strong>Task2: Class inheritance (6 marks) </strong>




In this task, we will define and implement inheritance classes.




Define the diagrams of the classes for bills below.










Define a base class <strong>Bill</strong> in a file <strong>Bill.h</strong> that contains biller’s name, code, reference number, account number, account name, address, amount due, totalGST, due date, period start date and period end date. Define necessary constructors, destructor, member functions and extraction operator (&gt;&gt;) and insertion operator (&lt;&lt;) for the base class. Implement the member functions and other friend functions in a file <strong>Bill.cpp</strong>.




Define a derived class <strong>ElectricityBill</strong> in a file <strong>ElectricityBill.h</strong> according to the diagrams above. Implement the functions in a file <strong>ElectricityBill.cpp</strong>. Define and implement overloading extraction operator (&gt;&gt;) and insertion operator (&lt;&lt;) for the ElectricityBill class.<strong> Note the rates (rate1 $0.245/kWh, rate2 $0.264/kWh), threshold (1750 kWh) and supply charge ($0.699/day) are the same for all ElectricityBill instances.</strong>




To compute total amount due for an electricity bill, we can use the following expressions: If total usage (<em>currentReading – previousReading</em>) is less than rate1 threshold,




<h1>Total amount electricity = (currentReading – previousReading) * rate1;</h1>




If the total usage is more than the threshold of rate1, we can use the following expression to compute amount of electricity




<em>Total amount  electricity = (currentReading – previousReading) * rate1 + ((currentReading – previousReading) – rate1Threshold) * rate2; </em>

<em> </em>

Then computes total supply charge,

<em> </em>

<em>Total amount supply charge = (periodEndDate – periodStartDate) * supplyCharge; </em>




Then computes total amount due and total GST by

<em> </em>

<em>Total amount due = Total amount electricity + Total amount supply charge ; </em>

<em> </em>

<h1>Total GST = Total amount due * 10%;</h1>




Define a derived class <strong>GasBill</strong> in a file <strong>GasBill.h</strong> according to the diagrams above. Implement the functions in a file <strong>GasBill.cpp</strong>. Define and implement overloading extraction operator (&gt;&gt;) and insertion operator (&lt;&lt;) for the GasBill class.<strong> Note the rates (heatingValue 38.82, pressureFactor 0.9942, rate $0.0297/MJ) and supply charges ($0.443/day) are the same for all GasBill instances.</strong>




To compute total amount due for a gas bill, we can use the following expressions:




Total MJ = <em>(currentReading – previousReading) * heatingValue * pressureFactor;</em>




<em>Total amount gas = total MJ * rate; </em>




Then computes total supply charge,

<em> </em>

<em>Total amount supply charge = (periodEndDate – periodStartDate) * supplyCharge; </em>




Then computes total amount due and total GST by

<em> </em>

<em>Total amount due = Total amount gas + Total amount supply charge ; </em>

<em> </em>

<h1>Total GST = Total amount due * 10%;</h1>




Define a derived class <strong>TelephoneBill</strong> in a file <strong>TelephoneBill.h</strong> according to the diagrams above. Implement the functions in a file <strong>TelephoneBill.cpp</strong>. Define and implement overloading extraction operator (&gt;&gt;) and insertion operator (&lt;&lt;) for the TelephoneBill class.<strong> Note the local call rate ($0.3/call), line rental ($29.9/month) and internet connection charge ($35/month) are the same for all TelephoneBill instances.</strong>




To compute total amount due for a telephone bill, we can use the following expressions:




Total local call = number of local calls<em> * local call rate;</em>




Then computes total amount due and total GST by

<em> </em>

<em>Total amount due = Total local call + international call amount + line Rental + internet connection; </em>

<em> </em>

<h1>Total GST = Total amount due * 10%;</h1>




Implement C++ main() and other functions in a file <strong>task2Main.cpp</strong> to display menu and get input from keyboard for bills and store bills’ information in the memory (such as linkedlist or dynamic arrays) until 0 (zero) for the choice has been input. For each bill data, computes total amount, total GST due for the bill. The program will save bill’s data in a text file, load bills’ data from a text file and display information of loaded bills (See the Testing of the task for more details).




<strong>Testing: </strong>

Use g++ to compile the source files by

$ g++ –o task2 task2Main.cpp Bill.cpp ElectricityBill.cpp GasBill.cpp TelephoneBill.cpp and run the program by $ ./task2

When the program starts, it will display menu and get input data.

<ol>

 <li>Input electricity bill data;</li>

 <li>Input gas bill data;</li>

 <li>Input telephone bill data;</li>

 <li>Set electricity rates;</li>

 <li>Set gas rate;</li>

 <li>Save bill data in a text file; 7. Load bill data from a text file;</li>

 <li>Quit.</li>

</ol>

Your choice: 1

Input electricity bill data.

Biller name: AGL

Biller code: 21345

Reference: 123456789012345678

Account number: 12345678

Account name: Mr. Tim Smith

Address: 1 Moore Street, Wollongong, NSW 2500

Start date: 15 12 2015

End date 14 3 2016

Due date: 5 4 2016

Previous reading (kWh): 12304

Current reading (kWh): 13186




Total amount due: $279

Total GST: $27.9




<ol>

 <li>Input electricity bill data;</li>

 <li>Input gas bill data;</li>

 <li>Input telephone bill data;</li>

 <li>Set electricity rates;</li>

 <li>Set gas rate;</li>

 <li>Save bill data in a text file; 7. Load bill data from a text file;</li>

 <li>Quit.</li>

</ol>

Your choice: 2




Input gas bill data.

Biller name: AGL

Biller code: 13245

Reference: 123456789012344321

Account number: 123443211

Account name: Mr. Tim Smith

Address: 1 Moore Street, Wollongong, NSW 2500

Start date: 10 12 2015 End date 16 3 2016

Due date: 30 3 2016

Previous reading (Cubic meters): 7724.5

Current reading (Cubic meters): 7796.3




Total amount due: $125.27

Total GST: $12.53




<ol>

 <li>Input electricity bill data;</li>

 <li>Input gas bill data;</li>

 <li>Input telephone bill data;</li>

 <li>Set electricity rates;</li>

 <li>Set gas rate;</li>

 <li>Save bill data in a text file; 7. Load bill data from a text file;</li>

 <li>Quit.</li>

</ol>

Your choice: 3




Input telephone bill data.

Biller name: Telstra Biller code: 33215

Reference: 123456789011112222

Account number: 11112222

Account name: Mr. Tim Smith

Address: 1 Moore Street, Wollongong, NSW 2500

Start date: 12 2 2016 End date 11 3 2016

Due date: 31 3 2016 Number of local calls: 23

International calls: 43.2




Total amount due: $115

Total GST: $11.5




<ol>

 <li>Input electricity bill data;</li>

 <li>Input gas bill data;</li>

 <li>Input telephone bill data;</li>

 <li>Set electricity rates;</li>

 <li>Set gas rate;</li>

 <li>Save bill data in a text file; 7. Load bill data from a text file;</li>

 <li></li>

</ol>

Your choice: 4




Set electricity rates.

Rate 1 ($ per kWh): 0.256

Threshold (kWh): 1800

Rate 2 ($ per kWh): 0.274

Supply charge rate ($ per day): 0.712




New rates for electricity bills have been set.




<ol>

 <li>Input electricity bill data;</li>

 <li>Input gas bill data;</li>

 <li>Input telephone bill data;</li>

 <li>Set electricity rates;</li>

 <li>Set gas rate;</li>

 <li>Save bill data in a text file; 7. Load bill data from a text file;</li>

 <li></li>

</ol>

Your choice: 5







Set gas rates.

Rate ($ per MJ): 0.0302 Heating value: 38.45

Pressure factor: 1.03

Supply charge rate ($ per day): 0.472




New rates for gas bills have been set.




<strong>The program will not stop until an input choice is 0 (zero).  </strong>

<strong> </strong>

Assume 6 bills’ data have been added in. When the choice is 6, the program will save all bills into a text file.

<ol>

 <li>Input electricity bill data;</li>

 <li>Input gas bill data;</li>

 <li>Input telephone bill data;</li>

 <li>Set electricity rates;</li>

 <li>Set gas rate;</li>

 <li>Save bill data in a text file; 7. Load bill data from a text file;</li>

 <li>Quit.</li>

</ol>

Your choice: 6




Text file name: bills.txt




6 bills have been saved.




The data in the text file should look like following (each bill stored in one line, start by the type: E-Electricity, G-Gas, T-Telephone):




E; AGL;21345;123456789012345678;12345678;Mr. Tim Smith; 1 Moore Street,

Wollongong, NSW 2500;15/12/2015;14/03/2016;05/04/2016;12304;13186;279;27.9

G;AGL;13245;123456789012344321;12344321;Mr. Tim Smith; 1 Moore Street,

Wollongong, NSW 2500;10/12/2015;16/03/2016;30/03/2016;7724.5;7796.3;125.27;12.53 T;Telstra;33215;123456789011112222;11112222;Mr. Tim Smith; 1 Moore Street,

Wollongong, NSW 2500;12/02/2016;11/03/2016;21/03/2016;23;43.2;115;11.5

…

<strong> </strong>

<ol>

 <li>Input electricity bill data;</li>

 <li>Input gas bill data;</li>

 <li>Input telephone bill data;</li>

 <li>Set electricity rates;</li>

 <li>Set gas rate;</li>

 <li>Save bill data in a text file;</li>

 <li>Load bill data from a text file;</li>

 <li>Quit.</li>

</ol>

Your choice: 7




Text file name: bills.txt




6 bills have been loaded.




Then display all bills information.

<strong> </strong>

Electricity bill:

Biller name: AGL

Biller code: 21345

Reference number: 123456789012345678

Account number: 12345678

Account name: Mr. Tim Smith

Address: 1 Moore Street, Wollongong, NSW 2500

Start date: 15/12/2012

End date: 14/03/2013

Due date: 05/04/2013

Previous reading: 12304

Current reading: 13186

Total amount due: $279

Total GST: $27.9




Gas bill:

Biller name: AGL

Biller code: 13245

Reference number: 123456789012344321

Account number: 12344321

Account name:  Mr. Tim Smith

Address: 1 Moore Street, Wollongong, NSW 2500

Start date: 10/12/2012

End date: 16/03/2013

Due date: 30/03/2013

Previous reading: 7724.5

Current reading: 7796.3

Total amount due: $125.27

Total GST: $12.53




Telephone bill:

Biller name: Telstra

Biller code: 33215

Reference number: 123456789011112222

Account number: 11112222

Account name: Mr. Tim Smith

Address: 1 Moore Street, Wollongong, NSW 2500

Start date: 12/02/2012

End date: 11/03/2013

Due date: 21/03/2013

Number of local calls: 23

International calls: $43.2

Total amount due: $115

Total GST: $11.5

<strong> </strong>

…

<strong> </strong>

You may run the program like:

$ ./task2 &lt; input4.txt




To check memory leak, you may run the program by

$ bcheck ./task2 &lt; input4.txt




You can download input data files <strong>input4.txt</strong> and <strong>input5.txt</strong> for your testing.