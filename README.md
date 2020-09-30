# -public-NFC_PRINTER_STAGER
the public version, just the apk released, of the private repo https://github.com/NDZL/NFC_PRINTER_STAGER

NFC_PRINTER_STAGER aims at easing staging of Zebra printers, exploiting NFC and BT connections.

Instructions:
- bump a NFC-enabled device into a Zebra printer
- ensure your device has the BT on
- fill in one of the 4 slots (which have persistent memory) with any SGD/ZPL code
-- some predefined weblink endpoints come by default
- finally press one of the 3 BT buttons to try sending that code to the printer, the choice depends on the printer model and LinkOs version.
-- BTLE => Bluetooth Low Energy APIs are used
-- BT-I => Classic BT with Insecure API (https://techdocs.zebra.com/link-os/2-12/android/content/com/zebra/sdk/comm/BluetoothConnectionInsecure.html): on some printers might not ask PIN checking
-- BT-S => Classic BT with secured API (PIN always checked)

Tested on:
- Zebra TC51 Oreo and MC22 A10

Features Roadmap:
- Objects transfer (e.g. weblink certificates)
- Analytics 
- Logs retrieving (e.g. weblink logs)

License:
- MIT

Feel free to feedback any comments or NIR (new feature request)
Thank you for using NFC_PRINTER_STAGER!

n.dzl
