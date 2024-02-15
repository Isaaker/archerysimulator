# Auth0

![Auth0 logo](../images/auth0.png)

## About

Auth0 is our Login and Identy provider and here you can find some important information to Develpo and Integrate the Platform with it.

**Also we have a security [wiki section](https://github.com/Isaaker/Ghost_Simulator_ES/wiki/Security)**

## User info modifications

Here are the processes by which the user can change their information (passwords, email and other data).

### Password

To change the password, the user only needs to access the Password Recovery Auth0 page

**What happens?**

1. The user enters the login page and clicks "¿No puedes acceder a tu cuenta?" or "Can´t login to your account"
2. The user enter her password
3. Auth0 check the email
4. If the email is correct, auth0 send an change password email
5. The user click the button or access the URL attached
6. The user access to the Auth0 recovery page and changes the password
7. The password is changed!!!

### Email

To change the email the user needs to contact to the administrator, there are to ways to make this:

** First option: Send an email with the actual email (Default)**

You should send an email to the platform administrator at the following address: archery.ghost.simulator@gmail.com with the subject: "Change Email" or "Change Email". To send the email, use the email that you use to login in to the simulator account.

**What happens?**

1. The user sees the email with as is detailed below
2. The administrator approves the changes and change manually the email
3. The administrator answer to the new email confirming the change
4. The user confirms the new email with the confirmation email
5. The user re-login with the new email and accepts the Conditions of use*
6. The user can now use the new email!!!

** Second option: Send an email with the new email and the security code (Only if the old email address is not retained)**

This method has been created as a double layer of security to avoid that if the access to the old email is lost, it can be changed in order to regain access to the account.

**For this method it is mandatory to have the recovery code that was sent to you when you created your account, this code is unalterable and will only be changed after you have used it. The password is not valid!!!**

**What happens?**

1. The user send an email with recovery code that assigned to it when it was discharged or when it was reassigned to it because it was previously used.
2. You send an email with the email to the administrator email (archery.ghost.simulator@gmail.com) and the subject: "Change Email" or "Change Email"., including the current recovery code in the body, no previous code or password will be valid.
3. The administrator answer to the new email confirming the change
4. The user confirms the new email with the confirmation email & suggests a new recovery code
5. The user re-login with the new email and accepts the Conditions of use*
6. The user can now use the new email!!!

*[Please refer to this section of the Conditions of use](../CONDITIONS.html)
> Al cambiar su dirección de email (previo aviso al administrador que es el encargado de realizar el cambio), se le volverá a solicitar que acepte las condiciones de uso de la plataforma, esto no implica que al cambiar el email halla dejado de aceptar las condiciones de uso, si no que nos indica que usted también acepta que se traten los datos de ese email.

## Auth0 endpoints


|URL|Use|
|---|---|
|ghostsimulator.eu.auth0.com/oidc/logout|Logout Users|