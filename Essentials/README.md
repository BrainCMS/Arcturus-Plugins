# Essentials

Essentials is an Arcturus Plugin by TheGeneral.

Installing a plugin is simple! Simply place the `essentials-1.jar` file into your `/plugins` folder.

Remember once adding a Plugin you'll need to reboot Arcturus Emulator. Don't forget to give yourself (and sometimes users) permission to use any command, this can be done via your database `permissions` table.

---

Various fun commands for your hotel.

* :brb or :afk
* :bh (number)
* :buyroom (confirm)
* :closedice (number)
* :antieffects or :disableffects
* :explain (command)
* :hoverboard
* :hug (username)
* :kill (username)
* :kiss (username)
* :nuke (username)
* :pay (username) (type) (amount)
* :sellroom (amount)
* :set
* :slime (username)
* :welcome (username)

Texts and keys ("commands") can be edited via the `emulator_texts` table. For example to add "away" as a alias of brb and afk you can modify `essentials.cmd_brb.keys` and add away so it becomes `afk;brb;away;`

---

### Database Modifications

Essentials requires no database modification / SQL queries. The plugin may automatically create the required database changes upon relaunching Arcturus Emulator.

---

This plugin has not been verified by TheGeneral/Wesley12312. Use this at your own risk. Always remember to make backups of your database before installation of third-party plugins.
