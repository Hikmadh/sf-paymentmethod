# _HitPay Payment Method Integration In Salesforce_

### Login into Our Salesforce Account.

![Screenshot 2024-05-10 190645](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/2d5850ca-f700-47f2-99d8-f73ddbc5c8e4)


### Create an Application.

![Screenshot 2024-05-10 190535](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/3a80a164-e8ac-44b1-9639-73dfb1dadd65)


### Then Create an Object.

![Screenshot 2024-05-10 191239](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/e21f65c5-33dc-4f3b-add4-b2b36af1fa6f)


### Inside the Object we need to create a fields.

![Screenshot 2024-05-10 171945](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/6fc01ec4-1006-401a-98a3-58694fa19ec3)


### Create an Apex Class like HitPayIntegration, to Enter the Code.

![Screenshot 2024-05-10 183634](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/880961ea-faf5-489f-bcf9-81b8fbed1e3d)


### After Enter the Code Execute using Anonymous Window.

![Screenshot 2024-05-10 183431](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/632e6251-50a6-4939-a133-30c67f0730c6)


### In this anonymous window we have to enter only the Class name and Method name.

![Screenshot 2024-05-10 183702](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/d745e178-f576-4f2c-bda8-a5df61bb0158)


### Then the User Debug Output shown like this.

![1](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/2eb90b78-c5dd-4530-8a2b-8036c1006a04)


### If we want to display only the URL, then change the code format for that and the User Debug are look like this.

![2](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/9b32b06e-afb5-4abe-9106-2c5313628a47)


### Now Create a Button like Send Payment Request using Visualforce Page.

![Screenshot 2024-05-10 185955](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/f345ada1-ebc4-4acb-a35b-2df1d4cbd68d)


### After creating Visualforce Page click preview to view how the page look like.

![Screenshot 2024-05-10 192057](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/3d60d6a0-94be-487e-a24b-79b981698bd5)


### So here The page will display like that the URL shown as a normal text and we have to changed the code, then it has been changed into URL.

![3](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/c379d1d4-584b-4d70-9f75-9c1c4975b6d6)

![4](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/71a6299e-cd15-41b3-990a-8806d3b44234)


### Then what I'm done here is when we click that send payment request button the URL automatically run and directly go to the Landing page.

![5](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/784c2c1d-f259-4818-8764-426973a5b3e3)

![6](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/d5a94f95-bc4e-4e47-afd2-0e3a8bf4ab46)


### After that create an another Apex for Webhook and Execute the code, then go to Sites in a salesforce and activate the Webhook.

![Screenshot 2024-05-10 193603](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/378d6c2c-4b61-4128-a88e-3821a9f0cd41)


### And check the Output in Debug Log on a Setup.

![Screenshot 2024-05-10 194743](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/fa300946-0efa-425f-b70e-5354ebeab7da)


### Apex Debug Log.

![7](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/86300a01-f828-42b1-bae5-2d0cf141f5b4)


### Here check the User Debug.

![8](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/9de327f8-b4a9-4671-a671-f2705759cee8)


### This is the File that the Separation of this User Debug.

![9](https://github.com/Hikmadh/sf-paymentmethod/assets/154895071/5b9dc911-3645-4a7d-8248-349892a9e30e)






