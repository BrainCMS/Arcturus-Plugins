# BubbleAlerts

BubbleAlerts is an Arcturus Plugin by TheGeneral.

Installing a plugin is simple! Simply place the `bubbelalerts-1.jar` file into your `/plugins` folder.

Remember once adding a Plugin you'll need to reboot Arcturus Emulator. Don't forget to give yourself (and sometimes users) permission to use any command, this can be done via your database `permissions` table.

---

This plugin will give you additional notifications on the right side of the client.

For example:

* Notification when a friend logs in.
* Notification when a furniture is bought.
* Notification when you bought a limited furniture.
* Notification when one of your marketplace offers is bought.
* Notification when you get mentioned in a different room, click to visit.

![Plugin Preview][preview]

---

### Database Modifications

BubbleAlerts requires no database modification / SQL queries. The plugin may automatically create the required database changes upon relaunching Arcturus Emulator.

---

### Configuration

`bubblealerts.notif_friendonline.image -> ${image.library.url}notifications/figure?p=%figure%`

`bubblealerts.notif_friendonline.useimage -> 1`

`path.furniture.icons -> ${image.library.url}/icons/`

`bubblealerts.notif_purchase.limited -> 0`

`bubblealerts.notif_marketplace.enabled -> 1`

`generic.furniture.bought -> You just purchased %amount%%is_limited%%itemname%%limited_display%!`

`generic.furniture.sold -> Your %item% has been sold. Click here to claim your credits!`

`bubblealerts.notif_friendonline.enabled -> 1`

`bubblealerts.notif_purchase.enabled -> 1`

`bubblealerts.notif_friendonline.message -> %username% just logged in! Say hi!`

`bubblealerts.notif_mention.message -> %username% mentioned you. Click to visit %username% in %room_name%!`


---

This plugin has not been verified by TheGeneral/Wesley12312. Use this at your own risk. Always remember to make backups of your database before installation of third-party plugins.

[preview]: https://raw.githubusercontent.com/BrainCMS/Arcturus-Plugins/master/BubbleAlerts/preview.png "Plugin Preview"
