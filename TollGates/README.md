# TollGates

TollGates v1.0 is an Arcturus Plugin by Brandon.

Installing a plugin is simple! Simply place the `tollgates-1.0.jar` file into your `/plugins` folder.

Remember once adding a Plugin you'll need to reboot Arcturus Emulator. Don't forget to give yourself (and sometimes users) permission to use any command, this can be done via your database `permissions` table.

---

Give your users the ability to set tolls on one way gates. `:settoll <currency_type> <amount>` - add a toll to a gate To remove a toll use `:settoll <currency_type> 0`.


Any gates without tolls will function as normal one way gates! Use `:paytoll` to pay the toll fee.


Players can only pay for a toll when facing the gate Players can set up to 4 tolls at a time (surrounded by gates) Players cannot stack toll gates Players cannot pay diagonally Gates cannot have a negative toll amount Gates can only have 1 toll at a time

---

### Database Modifications

In the  `items_base` table change all `one_way_gate` furniture items `interaction_type` to `tollgate`.

Add `toll_set` and `toll_pay` to your `permissions` table or run the SQL below:


```sql
`ALTER TABLE `permissions` ADD COLUMN `toll_set` enum('0','1') CHARACTER SET utf8 COLLATE utf8_general_ci NOT NULL DEFAULT '1', ADD COLUMN `toll_pay` enum('0', '1') CHARACTER SET utf8 COLLATE utf8_general_ci NOT NULL DEFAULT '1';`
```

---

This plugin has not been verified by TheGeneral/Wesley12312. Use this at your own risk. Always remember to make backups of your database before installation of third-party plugins.
