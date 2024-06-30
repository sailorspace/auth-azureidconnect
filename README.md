# auth-azureidconnect

Azure AD B2C and Azure AD authentication have different purposes and use cases. Here are some key differences:

Azure AD B2C:
- Customer-facing applications
- Used for authenticating customers or users who are external to an organization
- Supports millions of users and billions of authentications per day
- Provides a customizable, white-label authentication solution
- Offers features like single sign-on (SSO), authorization, and token caching
- Integrates with social identity providers like Facebook, Google, and LinkedIn
- Supports custom policies for any identity provider that supports OpenID Connect or SAML

Azure AD:
- Employee-facing applications
- Used for authenticating employees or users within an organization
- Provides features like SSO, Conditional Access, and Identity Protection
- Used for managing access to SaaS apps, licensing, and employee identity management
- Integrates with Microsoft Entra ID for employee authentication
- Does not support social identity providers or custom policies like Azure AD B2C

Azure B2B is primarily made to enable resource sharing and secure collaboration between businesses and their external partners, suppliers, 
or clients. 
Azure B2C, on the other hand, is designed specifically for consumer-facing programs and services that communicate with specific users.

If a company has multiple applications and each with separate user membership or authentication , then Azure B2c provides a platform for centralizing all this ,
in order to provide uniform authentication process.
B2C allows organization to federate with external facing applications by allowing features like OAuth,SAML, or openID .
All the Azure AD feature and capability are applied on the Azure B2C as well

Microsoft AD is On-Premise and Azure AD is cloud based.
Azure AD Connect syncronises between AD and Azure AD , so a seemles features for a companies to access resources such as office 360 etc 

-----------------------B2B-----------------------
To allow some users of a different AD of a company (dure to some business needs and partnership) , we use AZURE B2B ,
an invite is given to those users in order to have collaboration on some resources, enabling various capability for those users.
- also for users with just the microsoft account this works.
- works for any email / gmail etc accounts as well , for gmail accounts the invite will take the user to create the microsoft account ,.
  and this will generate a stub and allow access as in for the B2B as required.
https://www.c-sharpcorner.com/article/azure-active-directory-authentication/
-----------------------B2C----------------------
For customers to sign in with their own existing social identities
Its not tied to regular regular AD , unlike B2B where one uses existing Azure AD 
Allow consumers to allow their existing identiteies e.g, Local (mailids),facebook,google,git etc evently ending them in creating Azure AD Local Account account 
while configuring B2C the azure Admin can choose which ones to allow for the customers ,
B2C cannot collaborate or access to company resources though.
https://learn.microsoft.com/en-us/azure/active-directory-b2c/enable-authentication-web-api?tabs=csharpclient





