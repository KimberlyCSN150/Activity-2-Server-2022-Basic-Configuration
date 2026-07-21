# Activity 2: Server 2022 Basic Configuration

Baseline configuration applied to a fresh Windows Server 2022 install before it takes on any specific role.

## Objective
Get the server to a known-good starting state: updated, named, networked, and reachable remotely.

## Steps

- [ ] Log in to the server
- [ ] Pin Server Manager to the taskbar
- [ ] Uncheck "Start Server Manager automatically at logon" (Manage → Server Manager Properties)
- [ ] Rename the computer (e.g. `XXWS2K22-DC`, using your initials) and reboot
- [ ] Turn off Microsoft Defender Firewall for Domain, Public, and Private profiles *(lab/testing only — not production practice)*
- [ ] Enable Remote Desktop ("Allow remote connections to this computer")
- [ ] Assign a static IP: `192.168.10.100/24`, gateway `192.168.10.1`, DNS `192.168.10.100`, alternate DNS `8.8.8.8`
- [ ] Set the time zone to Eastern Time
- [ ] Capture a screenshot confirming the settings

## Notes
- Disabling the firewall entirely is a lab shortcut, not something to carry into a real deployment — it's done here just to remove a variable while testing connectivity.
- This same sequence is reused as a base template in later activities (e.g. configuring the client workstation).

## Screenshots to capture
- [ ] Server Manager showing updated time zone and network settings

 <img width="1081" height="680" alt="image" src="https://github.com/user-attachments/assets/7e2dd1dd-78b1-44ae-83fc-c895abe73964" />
