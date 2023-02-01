# LAB 1 of training course quizz

## Question 1

`Your users want to sign-in to devices, apps, and services from anywhere. They want to sign-in using an organizational work or school account instead of a personal account. You must ensure corporate assets are protected and that devices meet standards for security and compliance. Specifically, you need to be able to enable or disable a device. What should you do?`

- Enable the device in Azure AD.
- Join the device to Azure AD.
- Connect the device to Azure AD.
- Register the device with Azure AD.

<details>
    <summary>Answer</summary>

    Join the device to Azure AD.

    > Why?

    Join the device to Azure AD. Joining a device is an
    extension to registering a device. This means, it
    provides you with all the benefits of registering a
    device, like being able to enable or disable the
    device. In addition, it also changes the local
    state of a device. Changing the local state enables
    your users to sign-in to a device using an
    organizational work or school account instead of a
    personal account
</details>

## Question 2

`Identify three differences from the following list between Azure Active Directory (AD) and Active Directory Domain Services (AD DS).
Select three:`

- Azure AD uses HTTP and HTTPS communications
- Azure AD uses Kerberos authentication
- There are no Organizational Units (OUs) or Group - Policy Objects (GPOs) in Azure AD
- Azure AD includes Federation Services
- Azure AD can be queried through LDAP

<details>
    <summary>Answer</summary>

    - Azure AD uses HTTP and HTTPS communications
    - There are no Organizational Units (OUs) or Group Policy Objects (GPOs) in Azure AD
    - Azure AD includes Federation Services

    > Why?

    Although the list is by no means conclusive, and
    you may identify others not listed, here are
    several characteristics of Azure AD that make it
    different to AD DS: Azure AD is primarily an
    identity solution, and it is designed for
    Internet-based applications by using HTTP and HTTPS
    communications; because Azure AD is HTTP/HTTPS
    based, it cannot be queried through LDAP. Instead,
    Azure AD uses the REST API over HTTP and HTTPS.
    Because Azure AD is HTTP/HTTPS based, it does not
    use Kerberos authentication. Instead, it uses HTTP
    and HTTPS protocols such as SAML, WS-Federation,
    and OpenID Connect for authentication (and OAuth
    for authorization). Azure AD users and groups are
    created in a flat structure, and there are no
    Organizational Units (OUs) or Group Policy Objects
    (GPOs). While Azure AD includes federation
    services, and many third-party services (such as
    Facebook), AD DS supports federation. 
</details>

## Question 3

`You would like to add a user who has a Microsoft account to your subscription. Which type of user account is this?
Select one:`

- Cloud identity
- Directory-Synchronized
- Provider identity
- Guest User
- Hosted identity

<details>
    <summary>Answer</summary>

    Guest User

    > Why?

    Guest user. Guest users are users added to Azure AD
    from a third party like Microsoft or Google.
</details>


## Question 4

`You are configuring Self-service Password Reset. Which of the following is not a validation method?
Select one:`

- An email notification.
- A text or code sent to a user's mobile or office phone.
- A paging service.
- A set of security questions

<details>
    <summary>Answer</summary>

    A paging service.

    > Why?

    A paging service. At least one authentication
    method is required to reset a password. Choices
    include email notification, a text or code sent to
    user’s mobile or office phone, or a set of security
    questions.
</details>

## Question 5

`You are assigning Azure AD roles. Which role will allow the user to manage all the groups in your Teams tenants and be able to assign other administrator roles?
Select one:`

- Global administrator
- Password administrator
- Security administrator
- User administrator

<details>
    <summary>Answer</summary>

    Global administrator

    > Why?

    Global administrator. Global administrators can
    manage all the groups in your Teams tenants and be
    able to assign other administrator roles.

</details>
