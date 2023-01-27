# Best Practices When Setting Up a Hivemapper Fleet

> **Note**
> Please read through the top level [README](../readme.md) first

If you already have dashcams distributed to drivers and you'd like to begin using the Fleet Features, you'll need to create new accounts for all fleet
members. The Hivemapper system wants to ensure that every account that is part of a fleet has not been used to sign in to Hivemapper before. 
This is to ensure that any pending rewards will not be split.

When adding a new driver to your fleet through the [Hivemapper Explorer](https://hivemapper.com/explorer), the system should automatically detect
if the account you are attempting to add has been seen before. 

It is recommended to build out your entire fleet of drivers within the Fleet Dashboard so that when you set the ACL on the dashcams, all drivers
will be added. This will save you from having to manage multiple ACLs. In the future, you will be able to select which drivers you want (and don't want)
to have access to specific dashcams.

It is also recommended to create an extra account that is controlled by yourself and add it to the fleet. You should then promote this account to Manager 
status within the Fleet Dashboard. This is a fallback measure should you lose access to your main account. This will allow you to remove the ACL from each
dashcam, and you'll be able to start a fresh fleet at that point.

When adding a Driver to your fleet, there is a 5 minute window for them to accept the Join Fleet invitation. Be sure to be in contact with them when 
taking this step to ensure a smooth experience.

If you have a fleet that is distributed outside of where you live, you can use the Manager status to promote any trusted drivers in a region to become
a proxy for yourself to help with setting, modifying or removing an ACL should there be a need. 

If you don't have anyone in a region that you can promote as manager, another recommendation would be to create some extra accounts that you control the 
private keys to and add them to your fleet. If a driver loses access to their address, rather than shipping the device back and forth to reset the ACL,
you can simply give the driver the private key of one of these extra accounts and they may map using that account. This would allow you to have no down
time.

Any manager accounts that you'd like to share control over your fleet with should be added to the fleet *before* creating ACLs. If an account is set as
manager after the ACL has been added to the HDC, it will not have access to modify or remove the ACL on that dashcam.
