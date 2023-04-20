# SYNOPSIS ABOUT PROJECT

An airport requires a management system to control its various operations such as maintaining account of all the people in its domain of services, attending to various needs of customers and also achieving increased efficiency in the overall working of the airport itself.


## 1.1 PURPOSE OF THE SYSTEM

An airline ticket is a document or electronic record, issued by an airline or a travel agency, which confirms that an individual is entitled to a seat on a flight in an aircraft. The airline ticket may be one of two types: a paper ticket, which compromises coupons or vouchers, and an electronic ticket or e-ticket. The ticket, in either form, is required to obtain a boarding pass during check-in at the airport. Then with the boarding pass and the attached ticket, the passenger is allowed to board the aircraft.

## 1.2 WORKING

Here we start off by asking the user if he wants to create his own new account or login by the default made by the programmer.

![image](https://user-images.githubusercontent.com/67582528/233315153-ab676e5e-5ad3-47c9-a495-eb9021ae1a87.png)


Figure: Create an account or Login

If he/she chooses “CREATE NEW ACCOUNT” then the following details would be required to fill up.

![image](https://user-images.githubusercontent.com/67582528/233315324-efb21a7f-9c33-48cd-ae69-6b9b1cdc4862.png)



After this program we initially check the authenticity of the user by entering the password registered by them.
            ▪ If someone (can be any intruder, hacker) tries to enter with wrong password the program will not start.
            ▪ After 2 trials the program will ask you whether to change your password if in case forgotten.
            ▪ But it will have a security question which is registered by the user itself in “CREATE NEW ACCOUNT” so that an intruder cannot change the password and break in.


![image](https://user-images.githubusercontent.com/67582528/233318360-b1e1b898-eb42-4299-b4d6-dea4fb1411e8.png)


After the username and password is accepted :- A menu is displayed with several options
            ▪ Book A Flight
            ▪ Display Bookings
            ▪ Flight Search
            ▪ Names List
            ▪ Print Bill
            ▪ Search details
            ▪ Delete Details
            ▪ Settings
            ▪ Exit

![image](https://user-images.githubusercontent.com/67582528/233318500-c5da55a9-ed24-4538-bc5d-66deec7d8f8a.png)


If the first option ‘Book A Flight’ is selected, we ask the operator to fill in the details of the customer like name, type of trip etc.
Further the customer registration is to be done i.e. filling of Address, phone number and E-mail.
In second option ‘Display Bookings’, all the details of the customer, who had registered, are displayed, we can scroll between the screens using arrow keys.
In the option ‘Names List’ only the names of the customers are displayed who have registered in the system.
Bill is generated according to type of flight which is entered by the operator as ‘Print Bill’ option is selected. Bill is generated with full customer details and at the bottom of the bill all including fare details are written. Bill is also dependent on the number of passengers travelling in the flight. Class plays an important role in the bill. If the customer is travelling in business class then the fair is higher as compared to economy class.
NOTE: If this option is selected without registering any customer it will generate junk values.
In ‘Search details’, system first ask the operator to enter the name of the customer of whom the operator wants to fetch details. If the name entered is
already registered then details of that customer would come but if the name is not registered then screen will show “Desired name not found..!!”.
In ‘Flight Search’ departure date needs to be entered. Then comes the Departure city and Arrival city. Then randomly flight name, Departure time and arrival time will come. In this program we can have flight search for only 4 busiest routes of India that is between Delhi, Kolkata, Chennai and Mumbai.
Note: The first letter of the Departure city and Arrival city should be uppercase .
Syntax – Delhi, Mumbai etc.
In ‘Delete Details’ the operator can delete details of the passengers who have bookings completely from the file.
In ‘Settings’ the operator can see his account information, can change is username and password and can also see information about the program that how it works.


# HARDWARE & SOFTWARE REQUIREMENT

The programming language which is used to develop this program is C++. Hence we decided to use Turbo C++ (Borland C++ Builder) as our platform.
For optimal usage of such software a windows based operating system preferably Windows 7/8/10/XP must be there.
This program requires a system having enough processing speed, memory, hard disk space and compatible graphic card to run the program smoothly.

# HEADER FILES AND ITS FUNCTIONS

<iostream.h>
    • cout
    • cin
<stdlib.h>
        ◦ itoa
        ◦ exit
<conio.h>
        ◦ gotoxy
        ◦ getch
<stdio.h>
        ◦ gets
        ◦ puts
<dos.h>
        ◦ sound
        ◦ delay
        ◦ nosound
<string.h>
        ◦ strlen
        ◦ strcmp
<graphics.h>
        ◦ cleardevice
        ◦ setcolour
        ◦ outtextxy
        ◦ gotomaxx
        ◦ gotomaxy
        ◦ setfillstyle
        ◦ floodfill
        ◦ setbkcolour
        ◦ initgraph
        ◦ closegraph

## 1.3 DESCRIPTION ABOUT STRUCTURES

### Structure for Flight details and customer details. struct flight
{
  int flight_no; char
  name[30],depart[30],arrive[30],class1[30],address[30],searchn[30],flight_nam e[30],time1[7],time2[7];
  Date Train_date,Train_date1,Train_date2; int hr,min;
  int runway_no, no_of_seats; char boing_type[30];
  float fees; char:type_trip,mail_id[30],phone_no[15],house_no[10], street_name[30], city[18],pin_code[7],locality[20],pass_num[20];
}c[30];


 ### Structure for Date

struct Date
{
  int d,m,y;	//d—Day , m—Month , y—Year
};



### Structure for random ticket number in bill

struct ticket
{
  char ticket_no[10];
}q[10];


### Structure for creating a new account and displaying the information

Struct reg
{
  char name1[30],name2[30],email[50],sex[3];
}r[30];

### Structure for searching details

struct search
{
  char searchn[30];	//declairing structure for search variable
}m[30];

### Structure for generating date

struct date1
{
  int da_year;	/* current year */
  char da_day;	/* day of the month */ char da_mon;		/* month (1 = Jan) */
};

### Structure for displaying time

struct time1
{
  unsigned char ti_min;		/* minutes */ unsigned char ti_hour; /* hours */ unsigned char ti_sec;	/* seconds */
};

----------------------------------------------------------
# OUTPUT SCREENS

![image](https://user-images.githubusercontent.com/67582528/233319647-688907a1-b2f6-4ba2-9423-b6aac4770773.png)
Fig: Compilation of Program

![image](https://user-images.githubusercontent.com/67582528/233319699-faf87a2c-23df-4b02-8684-1f64b6ceed36.png)
Fig: Log-in Screen

Username and Password is basically for the security purpose.

Username: gomyway
Password:abcd1234

![image](https://user-images.githubusercontent.com/67582528/233319831-0aceb58e-8f18-4b1c-977e-327a13435f2e.png)
Fig: Incorrect Password Entered
System won’t start until correct password is entered.
After 2 seconds operator can re-enter Username and Password.

![image](https://user-images.githubusercontent.com/67582528/233319870-772917bc-9116-47ba-8e3b-e173544bae67.png)
Fig: Welcome Screen

![image](https://user-images.githubusercontent.com/67582528/233319902-7d0d8b4d-2f21-4d9b-b3df-cedc0407c4b1.png)
Fig: Home Screen
Arrow keys can be used to move the cursor and select these options.
Selecting ‘Exit’ will shut down the program.

![image](https://user-images.githubusercontent.com/67582528/233319955-cdd0033b-f854-4186-a1bd-b8d33016e10a.png)
Fig: ‘Book a Flight’ Screen
Here the operator will fill in the customer details.

![image](https://user-images.githubusercontent.com/67582528/233320016-0421813e-29b9-454b-ae12-aec93984e68f.png)
Fig: Further Details
If one way trip is selected then only departure date is to be filled.

![image](https://user-images.githubusercontent.com/67582528/233320087-4d63c7a9-3f77-492e-bf27-e94f05ee05db.png)
Fig: Further Details
If round trip is selected then the operator has to enter the departure date as well as the return date.

![image](https://user-images.githubusercontent.com/67582528/233320148-f2508114-f248-44ee-8297-7e0da76b45ca.png)
Fig: Registeration
Here the operator will enter the personal details of the customer like address, phone no. , E-Mail etc.

![image](https://user-images.githubusercontent.com/67582528/233320232-88e03272-abec-42fc-9022-ba301f8ca1d0.png)
Fig: “Customer Details”
Here the details of the customer entered by the operator are shown. On pressing arrow keys we can scroll the screen to right and left and show further details.

![image](https://user-images.githubusercontent.com/67582528/233320314-78a939f7-c419-424e-a852-c52e5051a7a7.png)
Fig: “Customer Details”
Here further details are shown on scrolling the screen.

![image](https://user-images.githubusercontent.com/67582528/233320362-7a8c9643-af40-42fc-95f6-4a6794148fd6.png)
Fig: “Flight Details”
In‘Flight Details’ departure date needs to be entered. Then comes the departure city and Arrival city. Thenvrandomly flight name, Departure time and arrival time will come.
In this program we can have flight search for only 4 busiest routes of India i.e between Delhi, Kolkata, Chennai and Mumbai

![image](https://user-images.githubusercontent.com/67582528/233320680-6f2acaa3-f8f7-4b2b-afee-5d122477c719.png)
Fig: “Flight Details”
Here on scrolling the screen the operator will enter the Flight details according to the customer.
The flight name date and time should be from the previous screen only (full flight name should be written).
Refer the previous screen for full name of flights.

![image](https://user-images.githubusercontent.com/67582528/233320723-7d45a47e-9642-4c95-b540-8cbf5dd19d8c.png)
Fig: “Flight search”
If the operator enters name of departure and arrival place other than Delhi, Mumbai, Kolkata or Chennai
Then this error will come up and the screen will again go back to main menu. Also if the first letter is not uppercase the then also error will occur.

![image](https://user-images.githubusercontent.com/67582528/233320807-690452fc-4d50-4481-9485-d8bb8d1bbdd9.png)
Fig: “Names List”
Here only the names of the customers are displayed who have registered in the system.

![image](https://user-images.githubusercontent.com/67582528/233320858-3337b352-0031-42b0-a124-599988cd685b.png)
Fig: “Print Bill”
Name, Address, Phone Number, departure date will be displayed in the bill along with type of flight chosen in the description. Also here random booking number and day is generated (top right corner).
Pressing ESC will take operator back to the main menu.

![image](https://user-images.githubusercontent.com/67582528/233320914-62301724-d039-4a1d-80cc-943f0364fae6.png)
Fig: “Search Details” Screen.
In ‘Search details’, system first ask the operator to enter the name of the customer of whom the
operator wants to fetch details.

![image](https://user-images.githubusercontent.com/67582528/233320977-4f3b5786-f611-4605-a6c2-805d814d6e0d.png)
Fig: “Search Details” screen.
If the name entered is already registered then details of that customer would come.

![image](https://user-images.githubusercontent.com/67582528/233321048-c76b2fcc-2cf0-45de-8d27-c26c1046e702.png)
Fig: “Search Details” screen.
If the name is not registered then screen will show “Desired name not found!”
On pressing ESC the operator will go back to main menu.

![image](https://user-images.githubusercontent.com/67582528/233321159-b23d649a-8e2a-4edb-9429-e6b046094d59.png)
Fig. “Settings” Menu
Here we can see modify our account settings and view the information of our account.

![image](https://user-images.githubusercontent.com/67582528/233321210-b140891e-9a01-4536-9b13-aca626f9f1b8.png)
Fig. “Username” settings
Here we can change the username of the account.

![image](https://user-images.githubusercontent.com/67582528/233321253-571cbdb6-4678-43db-98ab-cb62c72f2318.png)
Fig. ”Password” settings
Here we can change the password of the account.

![image](https://user-images.githubusercontent.com/67582528/233321305-856d9097-c5b6-4f13-8dcb-9a431378fcd5.png)
Fig. “Account Information”
Here we can view all the details of the account.

![image](https://user-images.githubusercontent.com/67582528/233321340-bc1634f9-2f43-46c4-a4ae-9cbe4546fec8.png)
Fig. “Delete Records”
Here the user can delete all the details of the customer from his program permanently.

![image](https://user-images.githubusercontent.com/67582528/233321394-da607dc3-0c4a-4d3b-9a58-be916695e505.png)
Fig. “Delete Records”
When file is deleted successfully press enter to go back to main menu

![image](https://user-images.githubusercontent.com/67582528/233321462-08e168ed-8711-4378-bf93-ead8e2693aa0.png)
Fig. “Forgot Password”
If the user forgets the password for his/her account then he/she can reset the account password provided the following particulars should be filled correctly.

![image](https://user-images.githubusercontent.com/67582528/233321533-a49a00e2-ebed-4498-9841-65bcb14e38ee.png)
Fig. “Forgot Password”
Here if the answer to the secret question (i.e. “Which is your favorite book”) is not given correctly the
password would not change.
After the password has been changed successfully it will directly come to the Main Menu screen.

![image](https://user-images.githubusercontent.com/67582528/233321580-1800fc4d-fb3d-45c2-94ac-76c283bd3958.png)
Fig: “Main Menu” Screen
On selecting EXIT the program will shut down an all the data in the program will be saved in the file called









