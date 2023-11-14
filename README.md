# RobloxSteamVRFixer
Fixes issue with SteamVR launching every time Roblox process is opened. Renames the directory for openvr and SteamVR temporarily so that SteamVR does not launch.

It should be noted that this is not a permanent fix and it is recommended to re-enable SteamVR when done using the Roblox application. SteamVR may update automatically and recreate the SteamVR and openvr folders, so the previous ones will need to be deleted in order for this code to work again.

If your files are stored in a different directory than the ones provided in the code, you will also need to find your SteamVR and openvr folders and change the paths accordingly.

# To-Do
* Add better error handling, currently just checks just attempts to change without checking first, raises flag if error in renaming operation.
* Let file paths be changed by user.
