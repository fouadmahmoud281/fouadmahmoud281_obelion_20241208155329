Internet Banking System  Software Requirement Specification  Team name : VIVACIOUS  Version : 1.0  Guided By   : Mr. PARAMJEET SINGH  Team Members  SUNIL KHANCHANDANI  HARSHVARDHAN  MOHIT GARG  HIMANSHU CHANDNA
Table of Contents  1) Introduction: ..........................................................................................................3  1.1) Purpose: ..........................................................................................................................3 1.2) Scope: ...........................................................................................................................3 1.3) Abbreviations: ..............................................................................................................4 1.4) References: ...................................................................................................................5 1.5) Technologies: ...............................................................................................................6 1.6) Overview ……………………………………………………………………………..6  2) Overall Description: ................................................................................................6  2.01) Product Perspective: ....................................................................................................7 2.02) Software Interface: ......................................................................................................8 2.03) Hardware Interface: .....................................................................................................8 2.04) Communication Interface: ...........................................................................................8 2.05) Product Features: ........................................................................................................8 2.06) User Characteristics: ...................................................................................................9 2.07) Design and Implementation Constraints: ....................................................................9 2.08) Use-Case Model Survey: .............................................................................................9 2.09) Architecture diagram: ................................................................................................14 2.10) ER-Diagram:…. ........................................................................................................15 2.11) Assumptions and Dependencies: ................................................................................15  3) Specific Requirements: .........................................................................................16  3.1) Use-Case Reports: .........................................................................................................16 3.2) Supplementary Requirements: .......................................................................................29  4) Supporting Information: ………………………….…………………………….30  4.1) System in context: …………………………………………………………………………….31 4.2) Class Diagram: ………………………………………………………………………………..32  5) Appendices: ……….……………………………….………...……………………33  5.1) Appendix B: References ………………………………………………………………………37 5.2)Screen Shots…………………………………………………………………………………..38  Revision History  Date   Version   Description   Author  1/11/2010   1.0   Internet Banking System   VIVACIOUS
1)   Introduction  Internet banking system provides is specifically developed for online banking for Balance Enquiry, Funds Transfer to another account in the same bank, Request for cheque book/change of address/stop payment of cheques, Mini statements (Viewing Monthly and annual statements).  1.1   Purpose  The Traditional way of maintaining details of a user in a bank was to enter the details and record them. Every time the user need to perform some transactions he has to go to bank and perform the necessary actions, which may not be so feasible all the time. It may be a hard-hitting task for the users and the bankers too. The project gives real life understanding of Internet banking and activities performed by various roles in the supply chain. Here, we provide an automation for banking system through Internet. Internet banking system project captures activities performed by different roles in real life banking which provides enhanced techniques for maintaining the required information up-to- date, which results in efficiency. The project gives real life understanding of Internet banking and activities performed by various roles in the supply chain.  1.2   Scope  This Project investigates the entry threshold for providing a new transaction service channel via the real options approach, where the entry threshold is established by using an Internet banking system designed for the use of normal users(individuals), Industrialists, Entrepreneurs, Educational Institutions(Financial sections), Organizations and Academicians under transaction rate uncertainty.  Customer must have a valid User Id and password to login to the system  If a wrong password is given thrice in succession, that account will be locked and the customer will not be able to use it. When an invalid password is entered a warning is given to the user that his account is going to get locked.  After the valid user logs in he is shown the list of accounts he has with the bank.  On selecting the desired account he is taken to a page which shows the present balance in that particular account number.
User can request for the details of the last ‘n’ number of transactions that he has performed. A report can also be taken of this.  User can make a funds transfer to another account in the same bank. User is provided with a transaction password which is different from the login password.  User can transfer funds from his account to any other account with this bank. If the transaction is successful a notification should appear to the customer, in case it is unsuccessful, a proper message should be given to the customer as to why it failed.  User can request for cheque book/change of address/stop payment of cheque’s  User can view his monthly as well as annual statements. He can also take print out of the same.  Generate reports at every section  Administrator can take a back up of the database for every instance that is happening, periodically.  All users are authenticated to avail the services  FAQ section is also included for end users benefit.  1.3   Definitions, Acronyms and Abbreviations  Administrator :   He is the super user who can add new customers into banking system, and assigns corresponding username, password, account type and other details. When any customer withdraws his account from the bank, he can delete their account and stop the transactions immediately. He can generate different reports. He also takes the system backup.  Team Members (Customers):   After logging in he can request for balance enquiry in his account, Funds Transfer to another account in the same bank, Request for cheque book/change of address/stop payment of cheques, Mini statements (Viewing Monthly and annual statements).  Industrialists, Entrepreneur, Organizations and academicians:   These are another type of customers. They will have extra information to be entered while logging in such as organization Id and so on. They can also perform all the actions what the normal customers are going to perform.
HTML:   Hypertext Markup Language is a markup language used to design static web pages.  EJB:   Enterprise Java Beans .  J2EE:   Java 2 Enterprise Edition is a programming platform part of the Java Platform for developing and running distributed multitier architecture Java applications, based largely on modular software components running on an application server.  DB2:   DB2 Database is the database management system that delivers a flexible and cost effective database platform to build robust on demand business applications.  WAS:   Web   sphere application   server is   an   application   server that   runs   business applications and supports the J2EE and web services standards .  WSAD:   Web sphere studio application developer is a toolkit which is designed for the creation of more complex projects, providing fully dynamic web application utilizing EJB’s. This consist of EJB tools , CMP ,data mapping tools & a universal test client that is designed to aid testing of EJB’ s.  HTTP:   Hypertext Transfer Protocol is a transaction oriented client/server protocol between web browser & a Web Server.  HTTPS : Secure Hypertext Transfer Protocol is a HTTP over SSL (secure socket layer)  TCP/IP:   Transmission Control Protocol/Internet Protocol, the suite of communication protocols used to connect hosts on the Internet. TCP/IP uses several protocols, the two main ones being TCP and IP.  1.4   References  SRS (IEEE SRS Format and Format provided by TGMC)  Project specification requirement (provided by TGMC)  Problem Definition (provided by TGMC)
1.5   Technologies to be used  J2EE   – Application architecture  JAVA   – Application architecture  WSAD   – Development tool  WAS   - Application Server  DB2   – Database  Dreamviewer   – Design tool  1.6   Overview  SRS includes two sections overall description and specific requirements  ü   Overall description will describe major role of the system components and interconnections.  ü   Specific requirements will describe roles & functions of the actors.  2) Overall Description  The following sections describe the general factors that affect the product and its requirements. Customer must have a valid User Id and password to login to the system. After the valid user logs in he is shown the list of accounts he has with the bank. On selecting the desired account he is taken to a page which shows the present balance in that particular account number, user can request details of the last ‘n’ number of transactions he has performed. User can make a funds transfer to another account in the same bank. User is provided with a transaction password which is different from the login password. User can transfer funds from his account to any other account with this bank. If the transaction is successful a notification should appear to the customer, in case it is unsuccessful, a proper message should be given to the customer as to why it failed. User can request for cheque book/change of address/stop payment of cheque’s. User can view his monthly as well as annual statements. He can also take print out of the same. Appropriate help to be provided as and when requested by the user.
2.0.1   Product Perspective  The client will have client interface in which he can interact with the banking system. It is a web based interface which will be the web page of the banking application. Starting a page is displayed asking the type of customer he is whether ordinary or a corporate customer. Then the page is redirected to login page where the user can enter the login details. If the login particulars are valid then the user is taken to a home page where he has the entire transaction list that he can perform with the bank. All the above activities come under the client interface. The administrator will have an administrative interface which is a GUI so that he can view the entire system. He will also have a login page where he can enter the login particulars so that he can perform all his actions. This administrative interface provides different environment such that he can maintain database & provide backups for the information in the database. He can register the users by providing them with username, password & by creating account in the database. He can view the cheque book request & perform action to issue the cheque books to the clients.
2.02   Software Interface  User on Internet   : Web Browser, Operating System (any)  Application Server   : WAS  Data Base Server   : DB2  Network   : Internet  Development Tools   : WSAD (J2EE, Java, Servlets, HTML), DB2, OS (Windows), Application Server.  2.03   Hardware Interface Client Side ( IE Along with Printer )  Processor   Ram   Disc Space  Internet Explorer 6.0  Pentium II at 500 MHz   64 MB   1 GB  Server Side  Web sphere application server  V5.0  Pentium III at 1 GHz   512 MB   2 GB  DB2 V8.1  Pentium III at 1 GHz   512 MB 1GB (Excluding data size)  2.04   Communication Interface  Client on Internet will be using HTTP/HTTPS protocol.  Client on Intranet will be using TCP/IP protocol .  A Web Browser such as IE 6.0 or equivalent.  2.05   Product Features :  The Internet banking system consists of following modules   : 1) Login Process :   This module allows valid customers to access the functionalities provided by the bank. 2) Balance Enquiry :   This module maintains the balance details of a particular account.
3) Update Profile :   This module allows the customer to update profile of their account. 4) Funds Transfer :   This module allows the customers to transfer funds from one account to another within the same bank. 5) Change of Password :   This module allows customers to change their password. 6) Mini Statements :   This module allows customers to view their transaction details.  2.06   User Characteristics :  Customers : The normal users will have an account of fixed or savings and should have a minimum balance of 500 Rs. He can transfer funds to another account of the same bank & may view his monthly or annual statements. Industrialists, Entrepreneur, Organizations academicians: These users will have all the three accounts & should have a minimum balance of 20,000 Rs. He can view the statements of his organization or industry  2.07   Design and Implementation Constraints  Login and password is used for identification of customer’s account and there is no facility for non users to login.  This system works only on a single server.  GUI is only in English  Limited to HTTP/HTTPS protocols  2.08   Use-Case Model Survey:  Description and the priority of this system  When we consider the online internet banking in this we provide the details of how to access the bank account without going to the bank through internet. When we consider the priority of this project it is mainly of medium cost, efficient to user access data, provides the required data, safe and secure one .we can know the details of our account whether it may be a transaction or deposit or balance enquiry etc.  Overall view of the banking system:  The Online Internet Banking provides us the banking facility through internet. The overall view of the banking System is as shown below:
Use-Case Model Survey:  customer  corporate  account list  balance enquiry  funds transfer  update profile  ministatements  initialises  shutdowns  request cheque book  End sessions  start sessions  Login  Data Backup  Crash recovery  help  performs  administrator  log out
Activity Diagram for overall system:  Enter userid & passwd  valid user  balance enquiry   Funds transfer   update profile   request cheque book  Ministatements  yes no  your account balance is ::....  to: ammount:   .  Log out  start stop  Users of the system:  In this online internet banking system, the users are  Ø   Administrators  Ø   Customers  Ø   Corporate.
1.   Administrator : He is the super user responsible for managing system users, taking system backup, generating reports, maintaining organization details, Starting Sessions and ending Sessions and also manages various requests from different Types of users.  Providing UserName, Password and other information required for the users to start an account.  Starting Sessions :   The Administrator creates the system users and will be assigned with the different roles. He is also responsible to start the session when a particular user wants to use the system every time(It is automatically managed setup).  Managing Data Backup :   The Administrator is responsible for managing entire details by taking the backup periodically. He also takes the Backup of the database in order to prevent loss of data on system crashes or inorder to prevent malfunctioning. He can take a backup of entire database or a particular section.  Crash Recovery :   The Administrator manages the crash recovery at the time of system crash or failure occurs.  Ending session :   The administrator is responsible for ending the session when the particular user logged out of the system(It is automatically managed setup).  2.   Customer(Normal/others) :   Ordinary customers have a user name & password with which they can login into their account. They can perform all the transactions such as funds transfer, balance enquiry, cheque book request, etc by sitting at their home on internet.  Login:   User can login to the system by providing appropriate username and password provided by the administrator.  Selecting the Account:   After logging in the user is provided with a screen showing the details of accounts and he selects one of the account inorder to perform the transaction.  Balance Enquiry:   He can view the balance left in his account, if once he has entered into his account.  Funds Transfer:   Upon the request the user can transfer funds from his account to other accounts.  Request for cheque book :   He can request for cheque book.  Mini statements:   He also can take a mini statement print out upon his requirement.
3.   Corporate:   The corporate users include Industrialists, Entrepreneur, Organizations and Academicians etc. They have a corporate id along with username & password. The organization will have an administrator to maintain all the details of their employees. He deposits salaries of the employees into the accounts of the corresponding employees. These employees can perform all the transactions that ordinary customer does.  Login:   corporate can login to the system by providing appropriate username, password and along with Corporate-ID provided by the administrator.  Selecting the Account:   After logging in the user is provided with a screen showing the details of accounts and he selects one of the account inorder to perform the transaction.  Balance Enquiry:   He can view the balance left in his account, if once he has entered into his account.  Funds Transfer:   Upon the request the user can transfer funds from his account to other accounts.  Request for cheque book :   He can request for cheque book.  Mini statements:   He also can take a mini statement print out upon his requirement.  Internal administrator:   Every corporation will be having its own internal administrator who is responsible for maintaining details of their employees, deposits salaries of the employees into their accounts.
2.09 Architecture Diagram :
2.10 ER- Diagram :  2.11 Assumptions and Dependencies  The details of customers such as username, password, account type and their corresponding authority details should be manually entered by the administrator before using this system.  administrator  Customer  organization  manages  password  Customer id   address  Phone no  manages   Works in  Org_name   ISA  Funds_transfer  Balance_enq  Accounts_types  updations Cheque_req   Mini stmts  Admin id   password  Generate the  accounts  Checks the  available  Update profile  Perform transacti  ons  Grant request  displays  Generate trans_list  Internal_admin  manage  Admin id  password
Every user should be comfortable of working with computer and net browsing.  He should be aware of the banking system.  He must have basic knowledge of English too.  3)   Specific Requirements  3.1   Use-Case Reports i)   Administrator : He is the super user responsible for managing clients of the system, taking system   backup, generating reports, maintaining organization details .  Manage Clients:   The Administrator assigns new users when a new client joins the online bank. Also he can delete an account when any of the clients leave the bank organization.  Maintain Organization Details:   The Administrator maintains entire details of the organization that includes details of the clients, entrepreneur details etc.  Take System Backup:   The Administrator Backup the database in order to prevent loss of data on system crashes. He can backup entire database or a particular section..  Generate Reports: :   Responsible for checking the logs of different system users for auditing and maintaining the integrity of the system  Manage Clients  Ø   Name Of Use-Case:   Manage clients.  Description:  The Administrator assigns new users when a new client joins the online bank. Also he can delete an account when any of the clients leave the bank organization.  Preconditions:  Administrator is already logged in.
delete_account  create_account  manage clients  Ø   Name Of Use-Case:   Maintain organizational details  Description:   The Administrator should maintain all the organizational details.  Preconditions:  Administrator is already logged in.  enterprenuar_details  client _details  details  Activity diagram for maintain organizational details:
Store details in database  Enter organizatin details  Ø   Name Of Use-Case:   Take System backup.  Description:   The Administrator Backup the database in order to prevent loss of data on system crashes. He can backup entire database or a particular section.  Preconditions:  Administrator is already logged in.  Ø   Name Of Use-Case:   Generate Reports.  Description:   The Administrator is responsible for checking the logs of different clients for auditing and maintaining the integrity of the system.  Preconditions:  Administrator is already logged in.  ii)   Customer :
.   Ordinary customers have a user name & password with which they can login into their account. They can perform all the transactions such as funds transfer, balance enquiry, cheque book request, etc by sitting at their home on internet.  Login:   User can login to the system by providing appropriate username and password provided by the administrator.  Selecting the Account:   After logging in the user is provided with a screen showing the details of accounts and he selects one of the account inorder to perform the transaction.  Balance Enquiry:   He can view the balance left in his account, if once he has entered into his account.  Funds Transfer:   Upon the request the user can transfer funds from his account to other accounts.  Request for cheque book:   He can request for cheque book.  Mini statements:   He also can take a mini statement print out upon his requirement.  Ø   Name Of Use-Case:   Login.  Description:   Customer must provide a valid User Id and password to login to the system  Preconditions:  Customer must have a valid User Id and password to login to the system.  access account  warning message  Login  +access  <<success>>  +warning  +relogin   <<failure>>
Activity Diagram for Login:  When the user opens the web page, he is shown with a page which asks him whether he is normal or a corporate customer. Then he is redirected to login page. Here the customer is asked to enter user name & password (corporate id if he selects corporate). When the user enters the details & submits it goes to a validation engine where it checks valid/not. If valid he is shown with list of accounts he has with the bank.  customer   System  prompt for user id & passwd  Enter user id & password  validate user & passwd  shows accounts list  valid invalid  Ø   Name Of Use-Case:   Accounts accessing.  Description:   Here the page will display all the accounts that the user has with the bank.  . Preconditions:  Client has already logged in.
Current  Savings  fixed  accounts list  Accessing view:  User after logging into his/her account a page is displayed with the basic requirements:  1) Balance Enquiry. 2) Funds Transfer (same bank). 3) Request Cheque Book. 4) Mini statements. 5) Update profile. User can perform various actions on his/her account.  Name Of Use-Case:   Balance enquiry.  Description:   Client can view the balance left in his account, if once he has entered into his account.  . Preconditions:  The client has already been logged in.  selects account   requests balance enquiry  displays balance  Activity Diagram for balance enquiry:  When the customer needs to check the balance, he selects balance enquiry option from the home page. Then the system checks the balance in his/her account & displays it on the balance enquiry screen.
Customer   System  display the transactions  select balance enquiry option  display the balance  Ø   Name Of Use-Case:   Funds Transfer.  Description:   The client can transfer the amount from his account in the bank to the other account in the same bank.  . Preconditions:  The client has already been logged in.  notify customer  not valid  transfer  Transaction paswd  +wrong passwd +try again  enter amount  valid  +passwd correct  Payee exists in our list  Enter payee  Payee not in list   enter payee details   wait for trans passwd  submit
Activity Diagram for funds transfer:  When the customer selects the funds transfer option in the home page. Then the system prompts for transaction password. When the user enters the transaction password, system checks whether the password is correct or not. If valid it prompts for payee & amount. User enters the payee details & amount, system checks whether the balance is available. If available it transfers & updates both the accounts. Customer is notified whether transaction is success or not.
Ø   Name Of Use-Case:   Request cheque book.  Description:   The client can request for cheque book by giving the details required.  . Preconditions:  The client has already been logged in.  request chequeBook  cheque book issue  submit Enter address  Activity diagram for cheque book request:  When the customer requests for a cheque book in the home page, the system prompts for address details of the customer. After entering the particulars it goes to validation engine & checks the particulars are valid or not. If valid it accepts the request & proper message is displayed to the customer.  Customer   System  display the transactions  select cheque book request option  prompt for address details  Enter address details  validation  accept request  show success/failure notice  yes no
Ø   Name Of Use-Case:   Stop payments of cheques.  Description:   Client can request to stop the payment of the cheque giving its details.  Preconditions:  The client has already been logged in.  stop payment of cheques  Submit Enter cheque details  Activity Diagram for stop payments of cheques:  When the customer selects stop payments of cheques option in the home page, the system prompts for cheque details which is to be stopped. Customer enters the details such as cheque number, payee, date, etc. The system accepts the request & provides the customer success/failure notice.  Customer   System  display the transactions  select stop payment of cheques option  prompt for cheque details  Enter cheque details  accept request  show success/failure notice
Ø   Name Of Use-Case:   Mini Statements.  Description:   The client can request the mini statements i.e monthly, annual or ‘n’ number of transactions.  . Preconditions:  The client has already been logged in.  Monthly stmts  Ministatements   print outs  Annual stmts  Activity Diagram for Mini Statements:  When the user requests for mini statements in the home page, system asks the type of statement needed by the customer. When the customer selects the type of statement (monthly/annual/’n’ number of transactions). The system displays the list of transactions on the screen. If the customer wants to take print outs he can take the print outs of the same.
Customer   System  display the transactions  select ministatements option  prompt for type of stmt  select type of statement  accept request & provide transaction list  view/take print out of list  Ø   Name Of Use-Case:   Update Profile.  Description:   The client can update his profile, i.e he can change his password, address, mobile number, e-mail id, etc.  Preconditions:  The client has already been logged in.  request for updating  enter new values in the fields   fields updated submit  Activity Diagram for update profile:  When the customer requests for update profile in the home page, the system shows present details to the customer. The customer changes the required fields he wishes to change & submits. The system updates the information & a proper message is displayed to the customer about the updated information.
Customer   System  display the transactions  select update profile  Shows   present details with edit option  select edit option for the field to be changed  prompt for new value  Enter new value for the field  update the change  send the updated information  iii)   Corporate users   :  The corporate users will have the same functionalities as that of a customer. The extra functionality of corporate user is to have an internal administrator.  Ø   Name Of Use-Case:   Internal administrator duties.  Description:   The internal administrator has to maintain company accounts & transfer salaries to the employees accounts.  Preconditions:  The internal administrator should have valid corporate_id, username & password.  The internal administrator has already been logged in.
manage company accounts  internal administrator  transfers money to employee's account  3.2   Supplementary requirements: 1 ) Performance Requirements  System can withstand even though many no. of customers request the desired service. Access is given to only valid users of bank who requires the services such as balance enquiry, update  profile, funds transfer, mini statements, and request for stop payments and for cheque book  2) Safety Requirements  By incorporating a robust and proven DB2 UDB into the system, reliable performance and integrity of data is ensured. There must be a power backup for server system. Since the product is of 24x7 availability there should be power backup for server which provides the information .Every day the data should be backup even when the operation of an user is not successful i.e., while performing the operation power failure occurs then data should be backup.  3) Security Requirements  Sensitive data is protected from unwanted access by user’s appropriate technology and implementing strict user-access criteria.   Facility of unique user number and Password in such a way that unauthorized user cannot log in. Operational rights for each user/terminal can be defined. Thus, a user can have access to specific terminals and specific options only.
Online Banking uses the SSL (Secure Socket Layer) protocol for transferring data. SSL is encryption that creates a secure environment for the information being transferred between customer browser and Bank. Online Banking uses 128-bit digital certificate from VeriSign for encryption of the Secure Sockets Layer (SSL) session. SSL is the industry standard for encrypted communication and ensures that customer's interaction with the Bank over the Internet is secure. Secure Socket Layer (SSL) protects data in three key ways:  Ø   Authentication   ensures that you are communicating with the correct server. This prevents another computer from impersonating Bank.  Ø   Encryption   scrambles transferred data.  Ø   Data integrity   verifies that the information sent by customer to Bank wasn't altered during the transfer. The system detects if data was added or deleted after customer sent the message. If any tampering has occurred, the connection is dropped.
4) Supporting Information:  4.1)   System in context:  The “Internet Banking System” is an independent system. In Version 1.0, the system is a Web based application which performs various activities of banking.  Ø   Takes data from the customer.  Ø   Interact with the database for the data storing.  Ø   Includes business logic that supports inventory and payroll.
4.2) Class diagram:  Balance Enquiry  userId : String  accountType : String  balance : Currency  showBalance()  Cheque Book  userId : String  chequeBookDetails : String  requestChequeBook()  stopPayCheques()  Update Profile  userId : String  password : String  firstName : String  lastName : String  address : String  mobile : String  updateProfile()  Funds Transfer  userId : String  accountType : String  TransId : String  payee : String  amount : Currency  transfer()  Customer  userId : String  password : String  firstName : String  lastName : String  address : String  mobile : String  login()  performTransaction()  logOut()  Mini Statements  userId : String  transList : String  showTransList()
5) Appendices:  5.1) Appendix A: Sequence Diagrams  Login process:  : customer   login page   system   services  enter userid & passwd  verification of valid user  allow access to services  login failed  relogin(+3)/block account  Balance Enquiry:  : customer   main page   DataBase balance enquiry  Requests BalanceEnq.  redirect  check  shows balance  view
Funds Transfer:  : customer   main page   funds transfer  page  database  request fund transfer  redirect  ask for trans passwd  enter passwd  enter payee & amount  notify customer  request for payee & amount success/failure  check balance  display message  check passwd  request ok  notify
Update Profile:  : customer   main page   update page   database  request update  redirect  edit the feilds to be updated  updated  notify  display updated details  update  display all fields  get the details  details  Cheque Book Request:  : customer   main  page  cheque book   database banker  Request for chequeBook  redirect  request details  provides details  accepts details  request processing  notify customer   check available check numbers  available numbers  send to customer
Stop payment of cheques:  : customer   main page   stop  payamen...  database  request stop payments  redirect  asks for cheque details  provide cheque details  stop cheque  display message  notify customer  validate  Mini Statements:  : customer   main page   ministmts page   database  request ministatements  redirect  select type of statement  access data requested  provides stmt details  displays transactions list  request printouts  provides printout format  type of statement?
5.1) Appendix C: References  •   tgmc website(www.tgmc.in)  •   ICICI portal(www.icici.com)  •   Google search engine(www.google.com-->online internet banking system)
5.2) Screen Shots  Login Page
Registeration
Welcome
Deposit
Money Transfer
Check balance
Mini-statement
