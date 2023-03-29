# Best Practices When Setting Up a Hivemapper Fleet

> **Note**
> Please read through the top level [README](../readme.md) first

1) If you already have dashcams distributed to members and you'd like to begin using the fleet features, you'll need to create new accounts for all fleet
members. The Hivemapper system wants to ensure that every account that is part of a fleet has not been used to sign in to Hivemapper before. 
This is to ensure that any pending rewards will not be split unnecessarily.

2) When adding a new member to your fleet through the [Hivemapper Explorer](https://hivemapper.com/explorer), the system will automatically detect
if the account you are attempting to add has been seen before. 

3) It is recommended to build out your entire fleet of members within the Fleet Dashboard so that when you set the ACL on the dashcams, all members
will be added. This will save you from having to manage multiple ACLs. In the future, you will be able to more easily select which members you want (and don't want) to have access to specific dashcams.

4) It is recommended to create at least one extra account that is controlled by yourself and add it to the fleet. You should then promote this account to Manager status within the Fleet Dashboard. This is a fallback measure should you lose access to your main account. This will allow you to remove the ACL from each dashcam, and you'll be able to start a fresh fleet at that point. Recommended to create this account under a separate 12-word seed phrase so that you don't lose access to both accounts at the same time. The functionality for a Manager to remove the ACL is still pending, but best to setup the Manager account now.

5) Reminder that when adding a member to your fleet, there is a 10 minute window for them to accept the Join Fleet invitation. Be sure to be in contact with them when taking this step to ensure a smooth experience.

6) If you have a fleet that is distributed outside of where you live, you can use the Manager status to promote any trusted drivers in a region to become
a proxy for yourself to help with setting, modifying or removing an ACL should there be a need. (this feature will be available soon, but best to setup any Manager accounts now so that it can be used once the feature is deployed)

7) If you don't have anyone in a region that you can promote as Manager, another recommendation would be to create some extra accounts that you control the private keys to and add them to your fleet. If a driver loses access to their address, rather than shipping the device back and forth to reset the ACL, you can simply give the driver the private key of one of these extra accounts and they may map using that account. This would allow you to have no down time. Note that if you choose this method, do not share them a 12-word seed phrase, as that is the same for all of your accounts within Phantom, but each address has a unique private key.

8) Any Manager accounts that you'd like to share control over your fleet with should be added to the fleet *before* creating ACLs. If an account's role is set as Manager after the ACL has been added to the HDC, it will not have access to modify or remove the ACL on that dashcam.
