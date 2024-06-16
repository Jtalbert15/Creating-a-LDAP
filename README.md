# Creating-a-LDAP

<h1>Summary</h1>

In this lab we will gain access to Active Directory through a VM other than our server. We will utilize LDAP (Lightweight Directory Access Protocol). LDAP allows us to modify Active Directory through a machine other than our server machines. LDAP utilizes TCP Port 389 to allow us to do this.

<h1>Step 1) Logging in and Setting Users Group</h1>
<img width="636" alt="Screenshot 2024-06-05 at 5 41 32 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/d6e736b1-a32d-49cf-a910-bd1b381acce4">

Take note of what client account you are logging into we will need to give the user permissions

Now on your server VM navigate to active directory users and computers and double click on your user

<img width="355" alt="Screenshot 2024-06-05 at 5 44 43 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/e0851ad7-7fcf-48af-b481-8356b18ad1db">

Click on Member of 

<img width="358" alt="Screenshot 2024-06-05 at 5 45 46 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/8cf456ea-d22a-4d0c-9c9e-cb4362b03d57">

You can see we are a member of 2 groups. Domain users and administrators

When your account is created you are a domain user by default

Typically you would not be a member of Administrators unless you are very high up but for simplicity's sake we added ourselves to the administrators group

Now let's navigate back to our user's client. You may have to restart your VM so changes take effect

<h1>Step 2) Downloading Active Directory</h1>

Now using Microsoft edge search active directory download windows 10

<img width="639" alt="Screenshot 2024-06-05 at 6 01 02 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/a17f5935-b61e-40b8-9153-5e9a5b807901">

The page should like the site up above. Scroll down and click download

<img width="638" alt="Screenshot 2024-06-05 at 6 02 51 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/df8d7035-8ca2-4b7e-961f-29c3466f1c9b">

Once it has downloaded click open file in the top right of the screen

<img width="638" alt="Screenshot 2024-06-05 at 6 03 40 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/b0e137d3-5216-4ee3-b159-52e022d10432">

Now we need to log into an account within our domain that has administrator privledges 

<img width="340" alt="Screenshot 2024-06-05 at 6 06 41 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/57e39be6-f62b-4378-aef3-0d904256b4f5">

Click I Accept (it will take a bit to install)

<img width="341" alt="Screenshot 2024-06-05 at 6 24 09 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/e1cd6f71-7d77-4c62-8e84-c6199f2a3c2a">

Now we can navigate to the windows icon in the bottom left part of the screen and navigate down to windows administrative tools


<img width="639" alt="Screenshot 2024-06-05 at 6 26 20 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/d9bec1ae-9b96-482b-b81c-6b178590efbf">

Click on the downward arrow and you can see we now have access to active directory

<img width="636" alt="Screenshot 2024-06-05 at 6 28 50 PM" src="https://github.com/Jtalbert15/Creating-a-LDAP/assets/66844406/978b8189-8d1d-479f-a566-643b032214b8">

Now we can manage active directory from this VM





