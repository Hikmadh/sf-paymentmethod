# _HitPay Payment Method Integration In Salesforce_

### Login into Our Salesforce Account.
#### To log in to Salesforce, go to the Salesforce login page and enter your username and password.

![Screenshot 2024-05-10 190645](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/2d5850ca-f700-47f2-99d8-f73ddbc5c8e4)


### Create an Application.
#### To create an application in Salesforce, navigate to the Setup menu, select "Apps", then click "New App" and follow the prompts to define its name, description, and choose its type (e.g., standard, console). Customize the app's tabs, branding, and access settings before saving and deploying it for users.

![Screenshot 2024-05-10 190535](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/3a80a164-e8ac-44b1-9639-73dfb1dadd65)


### Then Create an Object.
#### To create an object in Salesforce, go to Setup, select "Object Manager," then click "Create" and choose "Custom Object." Define the object's properties like name, fields, and relationships, then save it to make it available for use in your Salesforce environment.

![Screenshot 2024-05-10 191239](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/e21f65c5-33dc-4f3b-add4-b2b36af1fa6f)


### Inside the Object we need to create a fields.
#### To create fields within an object in Salesforce, navigate to the Object Manager, select the desired object, then click "Fields & Relationships." Choose "New Field," specify its type (text, number, picklist, etc.), define properties like label and length, and save the field to add it to the object. Repeat this process for each additional field needed.

![Screenshot 2024-05-10 171945](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/6fc01ec4-1006-401a-98a3-58694fa19ec3)


### Create an Apex Class like HitPayIntegration, to Enter the Code.
#### To create an Apex class in Salesforce, navigate to Setup, select "Developer Console" under "Developer Tools," then click "File" > "New" > "Apex Class." Enter your class name, then write your Apex code within the class body. Save the class when finished.

![Screenshot 2024-05-10 183634](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/880961ea-faf5-489f-bcf9-81b8fbed1e3d)


### After Enter the Code Execute using Anonymous Window.
#### In Salesforce Developer Console, we can run Apex code quickly using the Anonymous Window. Just open the Developer Console, navigate to Debug, choose Open Execute Anonymous Window. It's handy for testing snippets of code or debugging without creating a formal class or trigger.

![Screenshot 2024-05-10 183431](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/632e6251-50a6-4939-a133-30c67f0730c6)


### In this anonymous window we have to enter only the Class name and Method name.
#### In the Anonymous Window of the Salesforce Developer Console, you can execute Apex code by calling methods directly from existing classes. You'll typically enter the class name followed by the method name to invoke the desired functionality.

![Screenshot 2024-05-10 183702](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/d745e178-f576-4f2c-bda8-a5df61bb0158)


### Then the User Debug Output shown like this.
#### In the Salesforce Developer Console, after executing code in the Anonymous Window, the debug output appears in the "Debug Logs" tab. This output includes any messages or data you've specified to be logged using System.debug() statements in your Apex code. These logs provide valuable insights into the execution flow and help in debugging and troubleshooting.

![1](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/2eb90b78-c5dd-4530-8a2b-8036c1006a04)


### If we want to display only the URL, then change the code format for that and the User Debug are look like this.
#### If you want to display only the URL in the debug output, modify your Apex code to include a System.debug() statement specifically for the URL. When you execute this method in the Anonymous Window, the debug output will only show the URL, making it easier to focus on the specific information you need.

![2](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/9b32b06e-afb5-4abe-9106-2c5313628a47)


### Now Create a Button like Send Payment Request using Visualforce Page.
#### To create a "Send Payment Request" button using Visualforce in Salesforce, start by navigating to Setup and creating a new Visualforce page. Name it appropriately and insert a simple markup defining a button using <apex:commandButton>. This button will be linked to an action method in an Apex controller. Next, create an Apex class to handle this action. Implement a method named sendPaymentRequest within this class to define the functionality when the button is clicked. Once saved, users can access the Visualforce page to see and use the button, triggering the specified action upon clicking.

![Screenshot 2024-05-10 185955](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/f345ada1-ebc4-4acb-a35b-2df1d4cbd68d)


### After creating Visualforce Page click preview to view how the page look like.
#### Once you've created a Visualforce page in Salesforce, you can preview it directly from the Visualforce Page setup page. After saving your Visualforce page, click the "Preview" button next to the page's name. This allows you to see a preview of how the page will look and function when accessed by users. It's a convenient way to ensure that your page appears as expected and functions correctly before making it available to users within your Salesforce organization.

![Screenshot 2024-05-10 192057](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/3d60d6a0-94be-487e-a24b-79b981698bd5)


### So here The page will display like that the URL shown as a normal text and we have to changed the code, then it has been changed into URL.
#### If the Visualforce page initially displays the URL as normal text, but we want it to be rendered as an actual clickable URL, we can make adjustments to the Visualforce markup.Consider updating the markup to use an <apex:outputLink> tag instead of directly outputting the URL as text. 

![3](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/c379d1d4-584b-4d70-9f75-9c1c4975b6d6)

![4](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/71a6299e-cd15-41b3-990a-8806d3b44234)


### Then what I'm done here is when we click that send payment request button the URL automatically run and directly go to the Landing page.
#### To configure the "Send Payment Request" button to automatically navigate to a landing page when clicked, we'll need to update the Visualforce page's Apex controller method associated with the button. Inside the sendPaymentRequest method, use the PageReference class to specify the URL of the landing page, and then return this PageReference object. Now, when users click the "Send Payment Request" button on the Visualforce page, it will execute the sendPaymentRequest method in the Apex controller. This method will automatically redirect the user to the specified landing page URL.

![5](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/784c2c1d-f259-4818-8764-426973a5b3e3)

![6](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/d5a94f95-bc4e-4e47-afd2-0e3a8bf4ab46)


### After that create an another Apex for Webhook and Execute the code, then go to Sites in a salesforce and activate the Webhook.
#### To set up a webhook in Salesforce, first, create an Apex class to handle webhook logic. Then, activate it as a REST web service. Test the endpoint to ensure it works correctly. Next, configure a public site in Salesforce and expose the webhook endpoint through the site's guest user profile. Finally, activate the webhook by providing its URL to the external service that will send data to it. This setup allows Salesforce to receive and process webhook notifications from external sources.

![Screenshot 2024-05-10 193603](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/378d6c2c-4b61-4128-a88e-3821a9f0cd41)


### And check the Output in Debug Log on a Setup.
#### After configuring the webhook in Salesforce and activating it through a public site, you can monitor its behavior and debug any issues by checking the output in the Debug Log. Navigate to Setup, then search for and select "Debug Logs." Here, you can set up new debug logs or view existing ones associated with the Apex classes handling the webhook logic. By examining these logs, you can track the execution flow, inspect variables, and troubleshoot any errors encountered during webhook processing. This provides valuable insight into the webhook's behavior and helps ensure its smooth operation within the Salesforce environment.

![Screenshot 2024-05-10 194743](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/fa300946-0efa-425f-b70e-5354ebeab7da)


### Apex Debug Log.
#### The Apex Debug Log in Salesforce provides detailed information about the execution of Apex code, including system methods, triggers, and anonymous blocks. It captures events such as database operations, code execution, and system processes. Developers can use Debug Logs to monitor and troubleshoot Apex code, including any errors or unexpected behavior.

![7](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/86300a01-f828-42b1-bae5-2d0cf141f5b4)


### Here check the User Debug.
#### In the Apex Debug Log within Salesforce, the "User Debug" entries specifically display messages generated by the System.debug() statements embedded within Apex code. These statements are useful for developers to log custom messages, variable values, or any other relevant information during the execution of their code. By reviewing the "User Debug" entries in the Debug Log, developers can gain insights into the flow of their code, verify the values of variables, and diagnose issues more effectively. This feature enables developers to track and analyze specific behaviors or variables within their Apex code, aiding in debugging and optimizing application performance.

![8](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/9de327f8-b4a9-4671-a671-f2705759cee8)


### This is the File that the Separation of this User Debug.

![9](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/5b9dc911-3645-4a7d-8248-349892a9e30e)






