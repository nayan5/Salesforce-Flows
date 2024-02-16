# Salesforce-Flows
Salesforce Flow for sending Birthday Wishes :

Package Link for you : https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000009MmpB&isdtp=p1
 
Worried about forgetting your friend’s birthday, I have a solution for you! With the power 
of Salesforce flows, automating birthday reminders has never been easier. In this blog post, 
we'll explore how to set up a Salesforce flow to send birthday greetings to friends or 
contacts stored in our Salesforce org. 
We will need to store information about our friends, including their email 
addresses and dates of birth in our Salesforce Org. This could be useful for sending 
personalized birthday wishes, be manually remembering and sending these messages can 
be time-consuming. That's where Salesforce flows come in handy. With flows, you can 
automate repetitive tasks like sending birthday reminders, freeing up your time for more 
meaningful work. 


# Setting up the Flow: 
Let's dive into the step-by-step process of setting up a Salesforce flow for birthday 
reminders. 

# Step 1: Define the Object and Fields 
First, ensure you have a custom object in Salesforce to store information about your friends. 
Let's call it "Friend__c". Within this object, create fields for "Email__c" to store email 
addresses and "DOB__c" to store dates of birth. 

# Step 2: Create a Scheduled Triggered Flow 
Navigate to the Flow Builder in Salesforce Setup and create a new flow. Choose the 
"Scheduled Trigger" type for the flow. 

# Step 3: Define the Schedule 
Set the schedule to run daily or at a frequency that suits your needs. For birthday reminders, 
you might want the flow to run once a day. 

# Step 4: Query Records 
Next, add an element to query records from the "Friend__c" object where the date of birth 
matches the current date. This will retrieve records of friends whose birthdays are today. 

# Step 5: Loop through Records 
Add a loop element to iterate through the queried records. 

# Step 6: Send Email 
Within the loop, add an action to send an email to each friend whose birthday is today. Use 
the "Email__c" field to get the recipient's email address and customize the email message 
with a personalized birthday greeting.

# Step 7: Activate the Flow 
Once you've finished configuring the flow, activate it to start sending birthday reminders 
automatically.

Below are images supporting the blog that will give you a clear picture: 

   ![Screenshot 2024-02-16 101922](https://github.com/nayan5/Salesforce-Flows/assets/65781187/cbd08b7b-ead4-4c11-b52a-46fb99bec856)Complete Flow 
---------------------------------------------------------



   ![Screenshot 2024-02-16 101935](https://github.com/nayan5/Salesforce-Flows/assets/65781187/2595621f-db18-4f54-9828-6a6eded63b85)Schedule Flow 
---------------------------------------------------------


   ![Screenshot 2024-02-16 102006](https://github.com/nayan5/Salesforce-Flows/assets/65781187/87e0fc18-41e3-42ae-9b76-225c239d529f)Get Records 
---------------------------------------------------------


   ![Screenshot 2024-02-16 102021](https://github.com/nayan5/Salesforce-Flows/assets/65781187/e962a784-9156-4999-804f-051c862d9875)Loop 
---------------------------------------------------------


   ![Screenshot 2024-02-16 102038](https://github.com/nayan5/Salesforce-Flows/assets/65781187/96c93280-d001-4558-9edc-7b19d0551186)Action 
---------------------------------------------------------


   ![WhatsApp Image 2024-02-16 at 10 22 37 AM](https://github.com/nayan5/Salesforce-Flows/assets/65781187/d09814e4-eca4-4ea2-b6dc-7e01d5fe5fc3)Final Outcome 
---------------------------------------------------------

Conclusion: 
With Salesforce flows, automating birthday reminders for your friends or contacts is a 
breeze. By following the steps outlined in this blog post, you can set up a scheduled 
triggered flow to send personalized birthday greetings on their special day. Not only does 
this save you time, but it also helps you stay connected with your friends in a meaningful 
way. Harness the power of Salesforce flows to streamline your processes and make life a 
little bit easier. 
Start automating your birthday reminders today and never miss another special day again! 
 
