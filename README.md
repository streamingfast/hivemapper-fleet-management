# Fleet Management for the Hivemapper Network

This README will serve as an explainer on creating a Hivemapper fleet, adding driver accounts to your Hivemapper fleet, setting and changing token splits, locking dashcam access to your fleet of drivers, and exporting historical driving data of your fleet members.

## Creating a Hivemapper Fleet

A Hivemapper fleet is created at the time of [adding a driver](#adding-a-driver) to your fleet. Once a driver has been imported to your fleet, the Solana address is then tagged as a fleet manager by Hivemapper. This Solana address is the owner of the fleet, and will always have complete control over this fleet.

> **Note**
> You must use a brand new Solana address that has never connected to Hivemapper when creating a fleet.

## Adding a Driver

In the [Hivemapper Explorer](https://hivemapper.com/explorer), open the menu and select Fleets. 

#### Adding Your First Driver
If this is your first time adding a driver, you will be presented with a button to import a driver. 
Once selected, you'll be able to enter the Solana address of the driver you'd like to add. The driver will need to provide this to you after they have set up their [Phantom](https://phantom.app) wallet.

> **Note**
> THe driver must use a brand new Solana address that has never connected to Hivemapper when joining a fleet.

#### Adding a Driver to an Established Fleet
If you have already added at least one driver, you'll be presented with your fleet dashboard. In the top right, you'll find a +Import Driver button. This will open a modal window in which you can enter the Solana address of the driver you'd like to add. The driver will need to provide this to you after they have set up their [Phantom](https://phantom.app) wallet.

> **Note**
> THe driver must use a brand new Solana address that has never connected to Hivemapper when joining a fleet.

In both cases above, you'll then be presented a button to copy a link which is then sent to the driver. The driver will then open this link on their device where they have Phantom installed, and sign the requests to join your fleet.

> **Warning**
> The driver will need to accept your request to join your fleet within 5 minutes of generating the Join Fleet link.

Once joined, you will now see their account in your fleet dashboard view in the Hivemapper Explorer.

#### Promoting a Driver to Manager
TODO

## Token Splits

To set the token split for a driver's account, go to the fleet dashboard view of the [Hivemapper Explorer](https://hivemapper.com/explorer). In the right column, you'll find the Edit button for each driver. Select that and the token split will now become editable. The amount that is set is the percentage of earned tokens that will be kept by the fleet operator. 

For example, a token split of 100 will send all earned HONEY to the fleet manager account, while a token split of 25 will send 25% of earned HONEY to the fleet manager and 75% to the driver’s account. You can input an integer between 0 and 100, inclusively.

This value can be edited at any time, and will be applicable immediately to the current, and all future payout periods.

Each driver will be able to see the value set for the token split within the Hivemapper mobile application. 

## Access Control List

The Access Control List (ACL) is a list of Solana addresses that you'd like to give access to connect to any dashcams within your fleet that you'd like to have permissioned access for. 

#### Creating an ACL
Within the fleet dashboard, you can select any and all members that you'd like to have added to your ACL. At the moment, only the fleet owner is able to modify who can be added to the ACL.

#### Adding an ACL to a Dashcam
To add the ACL to a dashcam, you must connect a mobile phone to the dashcam you'd like to lock, while being connected to either the fleet owner account or any account that has been set as a manager within the fleet. 

Within the Hivemapper phone application, once signed in, you should see that your account is designated as a fleet manager and you'll have a toggle with which you can choose to lock the camera. When selecting to lock it, the application will pull the ACL in its current state from Hivemapper and write the ACL to the dashcam. This means that if you were to add a new account to your fleet's ACL after this has been done, that new address **WILL NOT** be added to this dashcam's ACL.

#### Modifying the ACL on a Dashcam
To modify the ACL on a dashcam, you'll first need to set the desired ACL in the fleet dashboard view of the [Hivemapper Explorer](https://hivemapper.com/explorer). Then you'll need to connect a mobile phone to the dashcam while being connected to either the fleet owner account or any account that has been set as a manager within the fleet. Note that the ACL that is already written to the dashcam will contain the list of managers that were set on the fleet *at the time when it was loaded onto the dashcam*. This means that if a driver has been promoted to manager within your fleet during the time since the ACL was loaded to the dashcam, they **will not** be able to modify the ACL (only those listed as managers at that point would have access). 

While paired with the dashcam, if you unlock the camera and then re-lock the camera, the new ACL will be retrieved from Hivemapper and loaded onto the dashcam.

#### Removing the ACL from a Dashcam
To remove the ACL from a dashcam, you'll need to connect a mobile phone to the dashcam while being connected to either the fleet owner account or any account that has been set as a manager within the fleet. Note that the ACL that is already written to the dashcam will contain the list of managers that were set on the fleet *at the time when it was loaded onto the dashcam*. This means that if a driver has been promoted to manager within your fleet during the time since the ACL was loaded to the dashcam, they **will not** be able to remove the ACL (only those listed as managers at that point would have access). 

Once the Hivemapper mobile application shows the camera as being unlocked, it will be freely useable by anyone who connects to it.
