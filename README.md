# DEPENDENCIES
[Quick WP-CLI requires WP-CLI to be installed in order to function](http://wp-cli.org/)

[Integrates with wp-tools](https://github.com/bluehost/wp-tools)

[Pulls from wpspeed](https://github.com/miles-cm/wpspeed)

# Quick-WP-CLI
Wrapper for WP-CLI commands used for troubleshooting WordPress sites. Also contains useful bash functions.

WP-CLI must be installed already on the hosting server. All commands used can be found here:
http://wp-cli.org/commands/

## How To Use This Tool
After connecting by SSH run the following command in your WordPress directory:

    . <(curl -sS https://raw.githubusercontent.com/rowdya22/Quick-WP-CLI/master/qwpcli)

## Available commands:

### qwpcli - Main Menu

### wpstats - Show Version, URL, DB Info, Number of Available Updates

### wpcore - Check Versions, Verify Checksums, Replace Core Files
Core Options:
   
(1) Check Version

(2) Verify-Checksums

(3) Replace Core Files

(4) Flush Permalinks

(5) Exit

### wpdb - Optimize and Repair, URL Rewrite
Database Options:

(1) Optimize and Repair

(2) URL Rewrite

(3) Clear Expired Transients

(4) Clear Orphaned Post Meta

(5) Exit

### wpplugin - List, (De)activate, Update, Install
Plugin Options:

(1) List

(2) Activate/Deactivate

(3) Deactivate All

(4) Restore Active Plugins

(5) Install

(6) Install Mojo

(7) Install Endurance Caching

(8) Exit

### wptheme - List, Change, Update, Install
Theme Options:

(1) List

(2) Change

(3) Install and Activate Default Theme

(4) Install Themes

(5) Exit

### wpurl - List and Change URLs
URL Options:

(1) Change URLs

(2) List URLs

(3) Exit

### wpuser - Create User, Set Passwords, Change Roles
User Options:

(1) List Users

(2) Create Temp User

(3) Remove Temp User

(4) Change Password

(5) Send Password Reset Email

(6) Change User Roles

(7) Change Username

(8) Exit

### wpupdate - Check For or Run Updates, Configure Auto Updates
Update Options:

(1) Core

(2) Plugins

(3) Themes

(4) All For This Install

(5) Check Available Updates

(6) Disable Auto Updates

(7) Exit

### wpbackup - Backup Site and Database to Folder or tar.gz
### wpworks - Install Updates, Optimize DB, Run Fixes
### wpglobal - Run Commands Across All WordPress Installs (Advanced) 

(1) Replace Core With Existing Version

(2) Install Updates, Flush Rewrite Rules, Flush Cache, Opt & Repair DB

(3) Clear Transients, Optimize/Repair Database

(4) Update Core, Plugins, and Themes

(5) Verify Checksums

(6) Check For Available Updates

(7) Disable (Bluehost) Auto Updates

(8) Check Theme/Plugin Conflicts

(9) Overhall (Replace Core, Flush Permalinks, Flush Cache, Media Regenerate, Opt & Repair DB)

(0) Exit

### wpmore - More Commands (Global Actions, WSOD Fix, File Count, DB List)

### WordPress Specific:

   wpwsod    - Guided Walkthrough to Fix WSOD
   
   wpfix     - Run Fixes
   
   wpbackup  - Backup Files and Database to Folder or tar.gz
   
   dblist    - Lists Database Names and wp-config.php Locations
   
   wpspeed   - Runs WordPress Speed Checks
   
   wpopt     - Basic Site Optimization and Suggestions
   
   wpinstall - Install WordPress From Scratch 
   
   wptools   - Show WordPress Tools Functions 
   
   wpdbcheck - PHP Based DB Tests 
   
   wpcheck   - Perl Based Plugin/Theme Check 

### Helpful Functions:

   fcount    - Lists Number of Files in Current Directory
   
   dirsize   - Sorts Directory Contents by Size
  
### Troubleshooting:

   mailtest  - Checks PHP Mail Function
   
   slowmysql - Displays Slow MySQL Queries

### WP Tools
This menu allows you to tap into the power of WordPress Tools. To skip the menu, type wptools and press tab twice to view options. All actions viewable in the WordPress Tools GUI. Choose a Function below:

(1) Backup  - Backup site through WordPress Tools (May not include all content)

(2) Restore - Restore site & database from existing WordPress Tools backup

(3) Upgrade - Backup and update site, plugins, themes. If errors exist revert.

(4) Exit

### WP Install
This setup will guide you through a manual WordPress install.

Make sure you are in the folder you want to install WordPress and there are no existing WordPress files.

---To begin create a database in cPanel and then enter the needed information---

### WP Optimization

WARNING: THIS IS AN ADVANCED MENU. MAKE SURE THAT YOU KNOW WHAT YOU ARE DOING! 
Check if there is existing optimization code in the .htaccess before modifying. If code is duplicated it can cause the site to break. 
 
(1) WP Speed Report

(2) Backup .htaccess

(3) Enable Gzip Compression (.htaccess)

(4) Enable Expired Headers (.htaccess)

(5) Revert Changes

(6) Quick Optimize 

(7) Install Recommended Plugins (Manual Setup)

(8) Exit
