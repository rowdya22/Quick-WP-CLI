WARNING: THE CREATOR(S) OF THIS SCRIPT ARE NOT LIABLE FOR DAMAGES OF ANY KIND. IF YOU DO NOT KNOW WHAT YOU ARE DOING, DON'T DO IT.


DEPENDENCIES
------------
 1. [Quick WP-CLI requires WP-CLI to be installed in order to function](http://wp-cli.org/)
 2. [Integrates with wp-tools](https://github.com/bluehost/wp-tools)
 3. [Pulls from wpspeed](https://github.com/miles-cm/wpspeed)

Quick-WP-CLI
============
Wrapper for WP-CLI commands used for troubleshooting WordPress sites. Also contains useful bash functions.
WP-CLI must be installed already on the hosting server. All commands used can be found here:
http://wp-cli.org/commands/

If you experience issues alias `wp` to where WP-CLI is installed.

How To Use This Tool
--------------------

After connecting by SSH run the following command in your WordPress directory:

    . <(curl -sS https://raw.githubusercontent.com/rowdya22/Quick-WP-CLI/master/qwpcli)

Available commands:
===================

qwpcli - Main Menu
------------------

        ___       _     __     _      _____      _______   ____
      / __ \__ __(_)___/ /__  | | /| / / _ \____/ ___/ /  /  _/  
     / /_/ / // / / __/  '_/  | |/ |/ / ___/___/ /__/ /___/ /   
     \___\_\_,_/_/\__/_/\_\   |__/|__/_/       \___/____/___/     
    
    What would you like added to QWPCLI? Let me know! https://github.com/rowdya22
    Type qwpcli to return to this menu:
    
    What would you like to work on?                            
    
       wpstats   - Show Version, URL, DB Info, Number of Available Updates
       wpcore    - Check Versions, Verify Checksums, Replace Core Files
       wpdb      - Optimize and Repair, URL Rewrite
       wpplugin  - List, (De)activate, Update, Install
       wptheme   - List, Change, Update, Install
       wpurl     - List and Change URLs
       wpuser    - Create User, Set Passwords, Change Roles
       wpupdate  - Check For or Run Updates, Configure Auto Updates
       wpconfig  - Configure wp-config.php Options
       wpwsod    - Guided Walkthrough to Fix WSOD
       wpglobal  - Run Commands Across All WordPress Installs (Advanced)
       wpmore    - More Commands (Global Actions, WP Tools, DB List)

wpstats - Show Version, URL, DB Info, Number of Available Updates
-----------------------------------------------------------------

    WPCLI Check:    [OK] 
    Checksums:      [OK] 
    Eval Plugins:   [CHECK]
    Eval Themes:    [CHECK]
 
    WP Version:     #.#.#
    Site URL:       https://example.com
    Home URL:       https://example.com
    Stylesheet:     twentyseventeen
    Template:       twentyseventeen

    Database Conn:  Success  
    Database Name:  db_name
    Database User:  db_user
    Database Pass:  PASSWORD
    Database Host:  localhost 
    Database Prfx:  wp_ 

    PHP Version:    #.#.#   	 Max Input Vars:  6000 
    Core Updates:   #  		     Memory Limit:    256M 
    Plugin Updates: # of #  	 Post Max Size:   256M 
    Theme Updates:  # of #  	 Upload Max Size: 256M

wpcore - Check Versions, Verify Checksums, Replace Core Files
-------------------------------------------------------------

    WordPress version: 
    Database revision: 
    TinyMCE version:   
    Package language:  
    
    Core Options:
    (1) Check Version
    (2) Verify-Checksums
    (3) Replace Core Files
    (4) Flush Permalinks
    (5) Exit
    
    	Selection: 

wpdb - Optimize and Repair, URL Rewrite
---------------------------------------

    DB Conn: 
    DB User: 
    DB Pass: 
    DB Host: 
    DB Name: 
    DB Prfx: 
    
    Database Options:
    (1) Optimize and Repair
    (2) URL Rewrite
    (3) Clear Expired Transients
    (4) Clear Orphaned Post Meta
    (5) Exit
    
    	Selection:

wpplugin - List, (De)activate, Update, Install
----------------------------------------------

    Active Plugins: 
    Total Plugins:  
    
    Plugin Options:
    (1) List
    (2) Activate/Deactivate
    (3) Deactivate All
    (4) Restore Active Plugins
    (5) Install
    (6) Install Mojo
    (7) Install Endurance Caching
    (8) Exit
    
    	Selection: 

wptheme - List, Change, Update, Install
---------------------------------------

    Template: 
    Stylesheet: 
    
    Theme Options:
    (1) List
    (2) Change
    (3) Install and Activate Default Theme
    (4) Install Themes
    (5) Exit
    
    	Selection:

 

wpurl - List and Change URLs
----------------------------

    Site URL:
    
    URL Options:
    (1) Change URLs
    (2) List URLs
    (3) Exit
    
    	Selection: 

wpuser - Create User, Set Passwords, Change Roles
-------------------------------------------------

    User Options:
    (1) List Users
    (2) Create Temp User
    (3) Remove Temp User
    (4) Change Password
    (5) Send Password Reset Email
    (6) Change User Roles
    (7) Change Username
    (8) Exit
    
    	Selection:

wpupdate - Check For or Run Updates, Configure Auto Updates
-----------------------------------------------------------

    Update Options:
    (1) Core
    (2) Plugins
    (3) Themes
    (4) All For This Install
    (5) Check Available Updates
    (6) Disable Auto Updates (WordPress Tools Only)
    (7) Update Endurance Cache
    (8) Exit
    
    	Selection: 

wpbackup - Backup Site and Database to Folder or tar.gz
-------------------------------------------------------
    Which configuration changes would you like to make?
      Select Options:
        (1) AUTOSAVE_INTERVAL
        (2) DISALLOW_FILE_EDIT
        (3) EMPTY_TRASH_DAYS
        (4) NOBLOGREDIRECT
        (5) WP_AUTO_UPDATE_CORE
        (6) WP_DEBUG
        (7) WP_MAX_MEMORY_LIMIT
        (8) WP_MEMORY_LIMIT
        (9) WP_POST_REVISIONS

wpbackup - Backup Site and Database to Folder, zip or tar.gz
-------------------------------------------------------

wpworks - Install Updates, Optimize DB, Run Fixes
-------------------------------------------------

wpglobal - Run Commands Across All WordPress Installs (Advanced)
----------------------------------------------------------------

       _______     __        __  ___      __  _                
      / ___/ /__  / /  ___ _/ / / _ |____/ /_(_)__  ___  ___        
     / (_ / / _ \/ _ \/ _  / / / __ / __/ __/ / _ \/ _ \(_-<          
     \___/_/\___/_.__/\_,_/_/ /_/ |_\__/\__/_/\___/_//_/___/    
    
    What global actions would you like to take? 
    
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
    
    Want to run another command? use gcmd [COMMAND] to run any command in all WordPress directories!
    
    	Selection: 


wpmore - More Commands (Global Actions, WP Tools, DB List)
----------------------------------------------------------------------

    WordPress Specific:
       wpboost   - Boost Memory Limits and php.ini Values
       wpworks   - Install Updates, Optimize DB, Run Fixes
       wpfix     - Run Fixes (Flush Permalinks/Cache, DB Cleanup)
       wpbackup  - Backup Files and Database to Folder or tar.gz
       wpmigrate - Move WordPress to Another Directory
       dblist    - Lists Database Names and wp-config.php Locations
       wpspeed   - Runs WordPress Speed Checks
       wpopt     - Basic Site Optimization and Suggestions
       wpinstall - Install WordPress From Scratch
       wptools   - Show WordPress Tools Functions
       wpcheck   - Perl Based Plugin/Theme Check
       wpcleanup - Remove All QWPCLI Generated Files
    Helpful Functions:
       fcount    - Lists Number of Files in Current Directory
       dirsize   - Sorts Directory Contents by Size
       editini   - Push Common Settings to php.ini
       editinisr - Search/Replace Values in the php.ini
    Troubleshooting:
       mailtest  - Checks PHP Mail Function
       slowmysql - Displays Slow MySQL Queries


WP Tools
--------

      _      _____    ______          __  
     | | /| / / _ \  /_  __/__  ___  / /__                    
     | |/ |/ / ___/   / / / _ \/ _ \/ (_-<                       
     |__/|__/_/      /_/  \___/\___/_/___/                     
    
    This menu allows you to tap into the power of WordPress Tools. To skip the menu,
    type wptools and press tab twice to view options. All actions viewable in the 
    WordPress Tools GUI. Choose a Function below:
    
    (1) Backup  - Backup site through WordPress Tools (May not include all content)
    (2) Restore - Restore site & database from existing WordPress Tools backup
    (3) Upgrade - Backup and update site, plugins, themes. If errors exist revert.
    (4) Exit

WP Install
----------

      _      _____    ____           __         __ __   
     | | /| / / _ \  /  _/___   ___ / /_ ___ _ / // /    
     | |/ |/ / ___/ _/ / / _ \ (_-</ __// _ `// // /     
     |__/|__/_/    /___//_//_//___/\__/ \_,_//_//_/      
    
    This setup will guide you through a manual WordPress install.
    
    Make sure you are in the folder you want to install WordPress and
    there are no existing WordPress files.
    
    
    ---To begin create a database in cPanel and then enter the needed information---

WP Optimization
---------------

      _      _____    ____       __  _       _          __  _         
     | | /| / / _ \  / __ \___  / /_(_)_ _  (_)__ ___ _/ /_(_)__  ___ 
     | |/ |/ / ___/ / /_/ / _ \/ __/ /  ' \/ /_ // _  / __/ / _ \/ _ \
     |__/|__/_/     \____/ .__/\__/_/_/_/_/_//__/\_,_/\__/_/\___/_//_/
                        /_/                                           
    
    WARNING: THIS IS AN ADVANCED MENU. MAKE SURE THAT YOU KNOW WHAT YOU ARE DOING! 
    Check if there is existing optimization code in the .htaccess before modifying. If code is duplicated it can cause the site to break. 
     
    
    (1) WP Speed Report
    (2) Backup .htaccess
    (3) Enable Gzip Compression (.htaccess)
    (4) Enable Expired Headers (.htaccess)
    (5) Revert Changes
    (6) Quick Optimize 
    (7) Install Recommended Plugins (Manual Setup)
    (8) Install Endurance Caching (No Configuration Required)
    (9) Exit


