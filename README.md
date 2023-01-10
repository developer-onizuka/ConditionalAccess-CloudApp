# ConditionalAccess-CloudApp

# 0. Get Microsoft 365 E5 license
> https://github.com/developer-onizuka/O365Access_GraphAPI#1-create-developer-account <br>

# 1. Conditional Access (in Azure AD's Enterprise Application)
**Important:**<br>
Please note Organizations that choose to implement Conditional Access policies that replace security defaults must disable security defaults.<br>
> https://learn.microsoft.com/en-us/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults

**(1) Create New Policy** <br>
    "Office 365" and "Microsoft Teams" are selected **in Cloud apps** to control.<br>
    "Use Conditional Access App Control" is set **in Session** as below:<br>
    You should add some users in addition to the above **in Users**.<br>
<img src="https://github.com/developer-onizuka/ConditionalAccess-CloudApp/blob/main/NewPolicy1.png" width="480"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src="https://github.com/developer-onizuka/ConditionalAccess-CloudApp/blob/main/NewPolicy2.png" width="240">

**(2) Click "Configure custom policy" in Session above** <br>
     Connected App is launched soon. Then, hit "Edit app" in bottom right. <br>
<img src="https://github.com/developer-onizuka/ConditionalAccess-CloudApp/blob/main/ConnectedApp.png" width="960">

**(3) Check "Use the app with session controls"** <br>
<img src="https://github.com/developer-onizuka/ConditionalAccess-CloudApp/blob/main/SessionControl.png" width="480">

**(4) Create Session Policy** <br>
<img src="https://github.com/developer-onizuka/ConditionalAccess-CloudApp/blob/main/CreateSessionPolicy.png" width="960">

**(5) Edit Session Policy** <br>
<img src="https://github.com/developer-onizuka/ConditionalAccess-CloudApp/blob/main/EditSessionPolicy.png" width="960">

# 2. Access Cloud App from the user assigned in Conditional Access
> https://www.office.com/ <br>

You can find the notification that you are monitored by organization. <br>
<img src="https://github.com/developer-onizuka/ConditionalAccess-CloudApp/blob/main/Notification.png" width="640">
