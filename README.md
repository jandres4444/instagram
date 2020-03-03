
Built with [mgp25's amazing Instagram Private API Wrapper for PHP](https://github.com/mgp25/Instagram-API/).
# Note
Please read this **entire** document as it has *very* important information about the script. If you create an issue that can be solved by reading this document, it will be ignored.

1. Install PHP, of course...
2. Goto the [most release release]
3. Download the `update.php` file and place it in its own folder
4. Run the script with `php update.php` and let it install the script
5. Edit the `USERNAME` and `PASSWORD` inside of the `config.php` file to your Instagram username/password.
6. Run the `goLive.php` script. (`php goLive.php`)

* Robust Installer/Updater
  * To install read the [Live Setup](#live-setup) section
  * To check for/apply an update just do `php update.php`
    * If you want to try beta features just do: `php update.php --beta`
* Web Control Panel
  * Use by doing `php goLive.php --web`
  * By default, you can access the control panel by going to `127.0.0.1` in your browser
    * You can change this by editing the `WEB_PORT` option in the `config.php` from `80` to some other number and then going to `127.0.0.1:PORT` where `PORT` is the number you changed it to
* Supports Accounts with 2FA
* View Live Chat/Likes (Windows/Mac Only)
* Execute Commands to Comment, Wave, Pin Comments, Show Questions, and more...
* Launch & Start OBS Automatically (Windows Only)
* Infinite Stream: Stream forever with no user input! (Windows/Mac Only)
  * Accomplished by doing: `php goLive.php -i -d`
  * Windows Users with OBS can do `php goLive.php -i -d --obs` for absolutely no input from the user required
* Archived Stream Statistics
  * Accomplished by doing: `php checkVod.php` 24 hours within archiving a stream
