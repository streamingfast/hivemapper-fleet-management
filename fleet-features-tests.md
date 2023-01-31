# Tests to Run For Fleet Features

In order to become comofortable and acquainted with the different fleet features for your Hivemapper fleet, here's a list of tasks that would be good to
make sure you are comfortable doing. All instructions for each task can be found in the main [README document](./hivemapper-fleet-management/readme.md).

1) Create fleet (this account is the fleet owner)
2) Add a driver to your fleet (This account should be loaded on a mobile phone that can be used to pair to your dashcam)
3) Add another driver to your fleet, promote them to Manager (This account should be loaded on a mobile phone that can be used to pair to your dashcam). This user's manager status will not be used for validation in this round of tests, but for the next Fleet feature tests.
4) Edit token split for either of the accounts in your fleet
5) Connect to dashcam using fleet owner account and lock the dashcam
6) Disconnect from dashcam and reconnect using the driver account added in Task 2
7) Create a new account in Phantom that IS NOT part of your whitelist. Attempt to connect to dashcam using this account (should not be able to connect properly)
8) Connect to dashcam using Manager account created in Task 3
9) Connect to dashcam using fleet owner account. Remove the lock on the dashcam
10) Attempt to connect to dashcam using new account created in Task 7 (should be able to connect now)
