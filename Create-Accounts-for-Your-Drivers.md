## Create Accounts for Your Drivers

Some Fleet Managers would like to create accounts for their drivers. This allows you to:

1. Become a recovery partner for your drivers, should they lose access to their account
2. Skip the need to teach your drivers how to setup an account through Phantom and understand public keys/private keys
3. Handle all of the Join Fleet signup yourself, and then simply give them a camera and input some information on their phone for them, 
making it truly hands off for your driver to get started

### Best Practices

It is recommended to create a fresh Phantom Wallet for your drivers, so that you keep some separation between your Fleet Owner account (which
controls your entire fleet) and the accounts of the drivers. While this is not necessary, it is a good security practice to limit any potential risks
you can encounter. 

Since you also maintain access to this account, it is recommended to have your driver remove any payments they receive in this account into a personal account that they create within Phantom. This removes the need for them to trust you won't take any funds from them, and more importantly that should either your account or the private key itself become compromised, they would have a very limited amount of exposed assets.


#### Create a New Browser Profile
To do this, on your laptop/desktop computer you can create a secondary profile within your browser
Here is the documentation on creating new profilts for the 2 most popular browsers.
[Google Chrome Documentation](https://support.google.com/chrome/answer/2364824?hl=en&co=GENIE.Platform%3DDesktop)
[Firefox Documentation](https://support.mozilla.org/en-US/kb/profile-manager-create-remove-switch-firefox-profiles)
This walkthru will include screenshots from Chrome.

Click on your profile icon (Number 1) and then click on +Add (Number 2)

<img src=Create-Accounts/01.png>

Select "Continue without an account"

<img src=Create-Accounts/02.png>

Name your profile (and set a colour theme if you'd like to help differentiate between your two profiles)

<img src=Create-Accounts/03.png>

Once you have this new profile created, you can add the [Phantom extension](https://phantom.app/download).

<img src=Create-Accounts/04.png>

To more easily access Phantom, you can first click on the extensions icon, and then on the Pin to pin it to your browser's main view

<img src=Create-Accounts/05.png>

<img src=Create-Accounts/06.png>

Open Phantom and select "Create a new wallet", and then safely store your 12-word recovery phrase.

<img src=Create-Accounts/07.png>

Once your wallet has been created, click on the Account icon in the upper-left corner of Phantom

<img src=Create-Accounts/08.png>

Click on the Accounts tab

<img src=Create-Accounts/09.png>

Create a new account, either by click on the + button, or the "Add / Connect Wallet" button.

<img src=Create-Accounts/10.png>

Select "Create New Account"

<img src=Create-Accounts/11.png>

Your new account will now be created and visible. To change the name of an account, click on the 3 dots next to that account and click on "Account Name"

<img src=Create-Accounts/12.png>
<img src=Create-Accounts/13.png>

Congratulations! You have now successfully created and renamed your accounts! Do this for as many accounts as you think you'll need.

### Add Driver to Fleet

While signed in to your Fleet Owner account on your primary browser profile, go to the [Fleet Management dashboard on Hivemapper](https://hivemapper.com/fleet-management).

<img src=Create-Accounts/14.png>
<img src=Create-Accounts/15.png>

Click on the "+ Add Driver" button

<img src=Create-Accounts/16.png>

You'll then be asked to enter the address of the driver you'd like to add. 

<img src=Create-Accounts/17.png>

You return to the other browser profile (where you have the Driver Accounts created), you can then click on the account name

<img src=Create-Accounts/18.png>

Click the "Copy" button of the account you'd like to add

<img src=Create-Accounts/19.png>

Paste the address into the Add Driver window of your Fleet Owner account (your primary browser profile). You'll then be able to copy the link

<img src=Create-Accounts/20.png>

Paste the link into the secondary profile window

<img src=Create-Accounts/21.png>

Click on "Connect Wallet", and Phantom will now open, asking you to Connect. If you have the wrong account selected in Phantom, click on the account name at the top of Phantom, and select the proper account that you're currently trying to add to your fleet.

<img src=Create-Accounts/22.png>

Next, click on the green "Join" button, and Phantom will open once again, asking you to Approve the request to join the fleet.

<img src=Create-Accounts/23.png>

You should then see a success message! You can close this tab if you'd like, but you don't need to.

<img src=Create-Accounts/24.png>

Return to your primary browser profile and refresh the page. You should now see your Driver account added to your fleet.

<img src=Create-Accounts/25.png>

Repeat this process for as many accounts as you'd like. 
You should then whitelist all of the accounts you'd added, by checking the checkbox under Whitelist. As well, you should set the desired token split for each account.

<img src=Create-Accounts/27.png>
<img src=Create-Accounts/26.png>

### Export Private Key of an Account

Now that you've added these Driver accounts into your fleet, you'll need to give your drivers each access to one of those accounts. To do this, we'll export a private key so that the Driver can import that address into their Phantom Wallet. This will allow them to access the camera using their mobile phone. This account is also where their rewards will be deposited.

Within Phantom, select the Account tab

<img src=Create-Accounts/32.png height="400px">

Then, select "Security & Privacy"

<img src=Create-Accounts/33.png height="400px">

Now select "Export Private Key"

<img src=Create-Accounts/34.png height="400px">

Phantom will ask you to re-enter your password and you will then be shown your private key. You can copy it now. 
You'll now have to transmit the private key to your driver. Some options are:

1. (Least secure) Send a text message or e-mail with the private key. After it has been copied by the driver, you can both delete the text or e-mail.
2. (More secure) Use an encrypted messaging service such as Signal or WhatsApp if you each have it installed already.
3. (Most secure) Create a locked PDF file. To do this, paste the private key into any text editor you use, and then save the file as a PDF. You can then upload it to this [Adobe site](https://www.adobe.com/acrobat/online/password-protect-pdf.html). You can upload your file to this site and then give it a password. Once it is password protected, you can delete the original file from your computer and transmit this password-protected file to your driver for them to open. 
