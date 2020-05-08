Android Technical Documentation


How to Run the App
* Download Android Studio from the following link:
   * https://developer.android.com/studio
* Install Android Studio
* Go to the project repository in Github or follow the link:
   * https://github.com/boolyy/DripNDashMain
* Download the repository from GitHub
* Open Android Studio Follow the sequence:
   * Click on File, New, Import project
      * Go in the zip file, click on the DripNDashProject folder, and click open
* Update any plugins that you are prompted to update
* Allow Gradle to sync
* If a dialog box asks to add files press allow
* At the top middle of the screen, you will see a run configuration. Click on Open AVD Manager and click on Create Virtual Device
* Choose Pixel 2, Choose Q for system image, then click finish.
* Repeat above step one more time, so you have two devices
* Next to the green triangle at the top middle, you will see the device Pixel. Click on the drop-down menu and select run on multiple devices
* Select both devices that you downloaded and run
* On one device, log in as a customer and on the other device, log in as a Dasher. Authentication is given below.


File Names
Java Class Files


Written by: Abdullah Bashir
Tested by: Abdullah Bashir
Debugged by: Abdullah Bashir
Customer.java 
- contains the customer object fields such as name, email, dorm etc.
CustomerFirestore.java 
- contains methods for interacting with customer’s information in the database
CustomerHomeActivity.java 
* Customer home view contains everything that a customer needs (request service, see progress etc.)
CustomerHomeFragment.java
* Extends the CustomerHomeActivity is a separate card that holds information that does not fit in the CustomerHomeActivity 
CustomerInProgressAdapter.java
* Gets the job progress from the Firebase database (Firestore)
CustomerPastJobsFragment.java
* Extends CustomerHomeActivity, shows all the previous jobs that the Customer has completed along with all the details of the job
Written by: Nicolas Rubert
Tested by: Nicolas Rubert
Debugged by: Nicolas Rubert
CustomerProfileFragment.java
* Extends CustomerHomeActivity, shows the Customer’s profile and allows them to edit their profile such as dorm room, campus etc.


Written by: Abdullah Bashir
Tested by: Abdullah Bashir
Debugged by: Abdullah Bashir
CustomerRegisterActivity.java
* User can register as a Customer
CustomerRequestDialog.java
* Extends CustomerHomeActivity, if a Customer wants to request a job they will receive a dialog with information pertaining to it
Dasher.java
* Holds all the Dasher fields such as name, email, dorm, etc.
DasherFirestore.java
* Dasher info that is connected to Firebase database (firestore)
DasherFirestoreInterface.java
* Extends DasherFirestore, allows the Firebase database(firestore) connect and update to the Dasher
DasherHomeActivity.java
* Dasher home view contains everything that a dasher needs (get job, see current job, etc.)
DasherHomeFragment.java
* Extends the DasherHomeActivity is a separate card that holds information that does not fit in the DasherHomeActivity 
DasherInProgressItem.java
* Dasher updates the job progression
DasherInProgressItemAdapter.java
* Takes the DasherInProgressItem and connects it to the Firebase database (Firestore)
DasherJobAcceptDialog.java
* Extends DasherHomeActivity, if there is a job available the Dasher will receive a dialog
DasherJobStatusFragment.java
* Extends DasherHomeActivity and DasherInProgressItem, is a view that allows the Dasher to update the job status 
DasherNoJobsDialog.java
* Extends DasherHomeActivity, if there is no jobs available the Dasher will receive a ‘no jobs available” dialog
DasherPastJobsFragment.java
* Extends DasherHomeActivity and shows all the previous jobs that the Dasher has completed along with all the details of the job
Written by: Nicolas Rubert
Tested by: Nicolas Rubert
Debugged by: Nicolas Rubert
DasherProfileFragment.java
* Extends DasherHomeActivity, shows the Dasher’s profile and allows the Dasher to edit their profile such as dorm room, campus etc. 


Written by: Abdullah Bashir
Tested by: Abdullah Bashir
Debugged by: Abdullah Bashir
DasherRegisterActivity.java
* User can register to become a Dasher
JobRequest.java
* Job request object fields such as number of loads, who requested the service etc.
JobRequestFireStore.java
* Extends JobRequest, writes the job request to Firebase database (Firestore)
JobRequestFirestoreInterface.java
* Extends JobRequestFireStore, allows the job to be updated by the Dasher/Customer 


Written by: Roberto Cruz
Tested by: Roberto Cruz
Debugged by: Roberto Cruz
RegisterActivity.java
* Users can register for the service for either Dasher or customer


Written by: Abdullah Bashir
Tested by: Abdullah Bashir
Debugged by: Abdullah Bashir
SignInActivity.java
* Allows users to sign into their account
TestActivity.java        
* Test activity to test whether or not the Dasher is competent to provide the service


Layout Files
Written by: Abdullah Bashir
Tested by: Abdullah Bashir
Debugged by: Abdullah Bashir
Activity_customer_home.xml
* Layout for the Customer home activity
Activity_customer_register.xml
* Layout for the Customer registration page activity 
Activity_dasher_home.xml
* Layout for the Dasher home activity
Activity_dasher_register.xml
* Layout for the Dasher registration page activity 


Written by: Roberto Cruz
Tested by: Roberto Cruz
Debugged by: Roberto Cruz
Activity_register.xml
* Layout for the registration activity


Written by: Abdullah Bashir
Tested by: Abdullah Bashir
Debugged by: Abdullah Bashir
Activity_sign_in.xml
* Layout for singing in activity
Activity_test.xml
* Layout for the Dasher test activity
Dialog_customerrequest.xml
* Layout for the Customer request activity
Fragment_customer_home.xml
* Fragment for Customer Home activity 
Fragment_customer_pastjobs.xml
* Fragment for Customer’s past job requests activity 
Fragment_customer_profile.xml
* Fragment for Customer’s profile activity 
Fragment_dasherjobstatus.xml
* Fragment for Dasher’s job status activity 
Fragment_home.xml
* Fragment that for Dasher home activity
Fragment_pastjobs.xml
* Fragment for Dasher’s past jobs  activity 
Inprogresscustomer_item.xml
* Layout to show the current Customer
Inprogressdasher_item.xml
* Layout to show the current Dasher 




Drawables- image files
ic_business_center_black_24dp.xml
* Image of a briefcase
Ic_check_black_24dp.xml
* Image of a check markt
Ic_directions_run_black_24dp.xml
* Image of a figure running


AndroidManifest.xml
* Contains information on the different activities of the app, assigns launcher activities and assigns main page for app


Dasher Accounts:
This is a Dasher who lives in the BEST dorm.
Username: bestdash2@gmail.com
Password: password


This is a Dasher who lives in the Livingston Apartments
Username: lividash@gmail.com
Password: password
Customer Accounts: 
This is a customer who lives in the BEST dorm.
Username: newcussy@gmail.com
Password: password


This is a customer who lives in the Livingston Apartments
Username: livicustomer@gmail.com
Password: password