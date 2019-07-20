# PNGCamera

PNGCamera is an Arcturus Plugin by Harmonic.

Installing a plugin is simple! Simply place the `PNGCam-1.3.jar` file into your `/plugins` folder.

Remember once adding a Plugin you'll need to reboot Arcturus Emulator. Don't forget to give yourself (and sometimes users) permission to use any command, this can be done via your database `permissions` table via `acc_camera` set to `1`.

---

Create a Camera Folder structure.

XAMPP Example:\
`C:\xampp\htdocs\swfs\camera` and `C:\xampp\htdocs\swfs\camera\thumbnails`

Change your external_variables to the following:\
`navigator.thumbnail.url_base=https://mydomain.com/swfs/camera/thumbnails/`\
`stories.image_url_base=https://mydomain.com/swfs/camera/`

Download the required [Habbo.swf](http://www.mediafire.com/file/s1b9r875b38sof5/newpng.swf/file).


---

### Database Modifications

Launch Arcturus

Once Arcturus is open type `stop` to close, we do this to import the needed SQL modifications.

Go to your Database and open the `emulator_settings` table.

Then edit the following:

`camera.url = https://mydomain.com/swfs/camera/`

`imager.location.output.camera = C:\xampp\htdocs\swfs\camera\`

`imager.location.output.thumbnail = C:\xampp\htdocs\swfs\camera\thumbnails\`

`camera.enabled = 1`

`interaction_type` should be set to `external_image_png` for Camera Pic and Habbo Selfie and `interaction_modes_count` set to `0` in the `items_base` table.

---

This plugin has not been verified by TheGeneral/Wesley12312. Use this at your own risk. Always remember to make backups of your database before installation of third-party plugins.
