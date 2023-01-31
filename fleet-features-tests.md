# Tests to Run For Fleet Features

In order to become comofortable and acquainted with the different fleet features for your Hivemapper fleet, here's a list of tasks that would be good to
make sure you are comfortable doing. All instructions for each task can be found in the main [README document](./hivemapper-fleet-management/readme.md).

1) Create fleet (this account is the fleet owner)
This is done by connecting to the Hivemapper Explorer with your account and clicking on the Fleets tab.
Expected behaviour is that you'll be presented with the ability to add a driver to your fleet.

2) Add a driver to your fleet
This account should be loaded on a mobile phone that can be used to pair to your dashcam.
Reminder that you'll need to sign the Join Fleet link within 5 minutes of it being created.
Expected behaviour is that you'll be presented with a success message, and then when going back to the Fleets tab with the fleet owner account, you'll then see the fleet dashboard.

3) Add another driver to your fleet, promote them to Manager 
This account should be loaded on a mobile phone that can be used to pair to your dashcam. 
This user's manager status will not be used for validation in this round of tests, but for the next Fleet feature tests.
Expected behaviour is that the user's Whitelist and Manager checkmarks in the fleet dashboard will now both become greyed.

4) Edit token split for either of the accounts in your fleet
Can test setting it to any amount between 0 and 100.
Expected behaviour is that when you use that account to log in to the mobile app, you will see this change displayed in the Settings tab.

5) Create an account in your phone's Phantom wallet that has not been added to your fleet
Use this new account to connect to the dashcam.
Expected behaviour is that you should be able to connect to it without issue.

6) Connect to the dashcam using the fleet owner account, lock the dashcam
When connecting as the fleet owner, you should notice that the Hivemapper logo will now look slightly different within the app. You will also see that
you are the fleet manager, and you'll now see a lock dashcam toggle.
Expected behaviour is that you'll be able to lock the dashcam. 
You'll also notice that next to the Dashcam ID line, a small lock icon to signify that this dashcam has been locked.
It is possible that you'll receive an error about the "shared secret". If this happens, then you must close the application and try again as the shared
secret for authentication has become too old to be used.

7) Disconnect from dashcam and reconnect using the driver account added in Task 2
You should be able to connect to the camera, as this driver is part of your fleet.
Expected behaviour is that you'll also see the slightly modified Hivemapper logo, as well as the name of the fleet owner account, and the token split
amount that you as a driver will receive. You'll also notice that next to the Dashcam ID line, a small lock icon to signify that this dashcam has been locked.

8) Attempt to connect to dashcam using the account created in Task 5 (account that was not added to the fleet)
Expected behaviour is that you will be presented with an error, asking you to connect using a different account that has access to this dashcam.

9) Connect to dashcam using Manager account created in Task 3
Expected behaviour is that you will be presented with the same experience as Task 7. Reminder that this account will soon be able to also unlock the dashcam, but this is not yet live.

10) Connect to dashcam using fleet owner account. Remove the lock on the dashcam
Expected behaviour is that the lock icon will go away next to the Dashcam ID, and the dashcam will now be open to connection from any account.

11) Attempt to connect to dashcam using new account created in Task 5
Expected behaviour is that you'll be able to connect to the camera using this account.
