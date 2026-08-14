# SimplyPrint Client

Run the SimplyPrint Client alongside Home Assistant and connect supported 3D
printers on your local network to SimplyPrint.

## Install

1. Add the SimplyPrint app repository to Home Assistant.
2. Select **SimplyPrint Client** in **Settings → Apps** and choose **Install**.
3. Start the app and optionally enable **Start on boot** and **Show in sidebar**.
4. Select **Open Web UI** and follow the SimplyPrint setup to add your printers.

No Home Assistant configuration is required. Printer accounts and normal client
settings are managed from the SimplyPrint web interface.

## Access and printer discovery

Open SimplyPrint from Home Assistant. Your Home Assistant session also signs you
in to the SimplyPrint interface, so there is no separate local password.

The app connects directly to your local network so it can find printers using
mDNS, SSDP, and manufacturer discovery protocols. If a printer is not found,
check that:

- Home Assistant and the printer are on the same local network;
- multicast or client isolation is not blocking traffic between them; and
- LAN or local-network access is enabled on the printer.

Home Assistant automatically assigns the app an available internal port. You do
not need to select or expose a port.

## Updates

Updates are installed by Home Assistant, not from inside SimplyPrint. When an
update is available, open **Settings → Apps → SimplyPrint Client** and select
**Update**. Home Assistant downloads the new container image and keeps your app
data. You can also enable automatic updates on that page.

The update channel shown inside SimplyPrint is read-only because the app version
is selected by the Home Assistant app repository.

## Backups

Home Assistant backups include the app's printer configuration, settings, and
other persistent data. The app is briefly stopped while its data is backed up.

## Support

For help using SimplyPrint, contact [SimplyPrint support](https://simplyprint.io/contact).
For Home Assistant packaging problems, use the repository issue tracker.

## License

The SimplyPrint Client is proprietary software. Installing this app does not
grant permission to copy, modify, or redistribute the client or its container
image except as expressly authorized by SimplyPrint ApS.
