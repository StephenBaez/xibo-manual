<!--toc=getting_started-->
# Xibo 1.7.0-alpha - Codename "Tuttle"

This is a development preview release of Xibo. This release is the first of the development preview releases of Xibo working towards the release of Xibo 1.7.0, the next stable line of Xibo released. **This should NOT BE USED IN PRODUCTION.**.

You can download this release from [https://launchpad.net/xibo/1.7/1.7.0-alpha](https://launchpad.net/xibo/1.7/1.7.0-alpha)


## Requirements

You must use the 1.7.0-alpha version of the Windows Display Clients with this version of the Xibo CMS. The Ubuntu Client is not currently compatible with 1.7 series.

Xibo requires PHP 5.3.3 or higher. A full list of module requirements is presented at the point of installation - we'll even tell you which modules you're missing!

### Xibo for Windows

There are significant changes to the way display client settings are managed. All settings are now managed on the CMS except the settings required to connect to the CMS. You will need to manually migrate your settings into the CMS - we have provided sensible default values. See [display settings](index.php?toc=user_and_display&p=admin/displayprofiles) in the manual for more information.

The .NET Framework requirement has been raised to v4.

The IE rendering engine has been replaced with Chromium Embedded Framework.

## Upgrading

There are significant database schema changes between the 1.7 series of Xibo and prior releases. The upgrade wizard will take a prior database and convert it to a schema suitable for the 1.7 series to date. Note that this is a one-way conversion. **Please do not upgrade your production database to test Xibo 1.7 functionality, and then expect to run a prior series code base against that database.**

Instructions for cloning a Xibo database are available here [Clone Database](release_notes_clonedb.html "Clone Database").

*   Clone your existing Xibo database and grant permissions (see [Release Notes:Clone Database](release_notes_clonedb.html "Clone Database") for details)
*   Backup settings.php from your installation
*   Manually take a backup of your database
*   Replace your existing installation with the new version from the tar.gz or zip file. **Do not copy over the top.**
*   Replace your backup settings.php file in your Xibo installation directory
*   Browse to [http://your.server/path](http://your.server/path)as normal
*   You will be prompted that an upgrade is required.
*   Enter your xibo_admin password, and follow the upgrade wizard.
*   The upgrade should run, and finally ask you to log in as you would normally.

## Help

Please ask for help / advice in the Answers section of Launchpad: [https://answers.launchpad.net/xibo](https://answers.launchpad.net/xibo)

Please report any bugs in the Bugs section of Launchpad: [https://bugs.launchpad.net/xibo](https://bugs.launchpad.net/xibo) (if you're not sure that what you have found is a bug, please ask in the Answers section first!)

Please report any enhancement requests in the Blueprints section of Launchpad: [https://blueprints.launchpad.net/xibo](https://blueprints.launchpad.net/xibo)

When asking for assistance with this release, please make it clear that you're using the development preview and not a stable release of Xibo.

## Bug Fixes

For a full list of bug fixes please refer to the Release Project Page: [https://launchpad.net/xibo/1.7/1.7.0-alpha](https://launchpad.net/xibo/1.7/1.7.0-alpha)

## Known Issues and Limitations

This is a development preview release primarily intended for community testing. This release will most likely contain bugs.