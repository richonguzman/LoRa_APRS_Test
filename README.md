# LoRa_APRS_Test

RAK4630 NRF52840 test Firmware for digirepeater

Instructions:

1) prepare confuration info (As the initial configuration wont find any digi_conf file with the configuration you should enter the following one):

"CALLSIGN,digiMode,symbol,overlay,comment,latitude,longitude,sendBatteryTelemetry,beaconInternal"

example: "AB1CDE-11,1,#,L,LoRa RAK4630 Test,0.0000000,0.0000000,Y,15"

- CALLSIGN = Replace with your Valid Ham Callsign
- digiMode = 1 for WIDE1-1, 2 for WIDE2-1
- symbol = #
- overlay = L
- comment = LoRa RAK4630 Test (donde use coma in comment)
- latitude = in degrees and better to have 7 decimals
- longitude = in degrees and better to have 7 decimals
- sendBatteryTelemetry = Y for yes, N for no.
- beaconInterval = 15 (minutes


2) press two times reset button to enter Virtual Disk bootloader mode: RAK4630 or RAK4631 external disc should appear in your PC/MAC/Linux OS

3) drag "firmware.uf2" file into the folder/external disk. It should reboot right away and you should get into any app that let you enter serial commands (Arduino IDE, VSCODE ...)


if you want to delete previous configuration , drag "NRF52840_DeleteConfig.uf2" into the folder/virtual disk when boards is in boot loader mode.


- 2024.09.17 Battery Pins correction proposal
- 2024.09.15 Alpha
