

# 2.0.17 (06/2014) #
## Import Games ##
  * bugfix: flatfile scrapers were broken

# 2.0.16 (06/2014) #
## General ##
  * bugfix: Delete Rom Collection dialog did not work language independent

## Import Games ##
  * bugfix: nfo import was broken with new version of elementtree

# 2.0.15 (05/2014) #
## General ##
  * add autoconfig support to Edit Rom Collection dialog
  * add and update languages
  * replace elementtree module with xml.etree
  * add new string ids with ids from 32000 to 32999

# 2.0.14 (04/2014) #
## Launch Games ##
  * add autoconfig support on Android

# 2.0.13 (03/2014) #
## Launch Games ##
  * fixed issues with launching games on Android

# 2.0.12 (03/2014) #
## General ##
  * workaround to update button labels with empty strings in Edit Rom Collection dialog

## Import Games ##
  * update moby scraper: reflect changes on page

## Launch Games ##
  * add option to suspend audio before launching games
  * add option to toggle screen mode before launching games

# 2.0.11 (10/2013) #
## General ##
  * configure RetroPlayer support per config wizard and UI

# 2.0.10 (09/2013) #
## General ##
  * bugfix: an error occured when creating a new config file

# 2.0.9 (09/2013) #
## Import Games ##
  * fix thegamesdb scraper: requests have been blocked by cloudflare

# 2.0.8 (09/2013) #
## Import Games ##
  * update moby scraper: reflect changes on page

# 2.0.7 (06/2013) #
## Import Games ##
  * updated list of thegamesdb platforms
  * bugfix: scraping games with (**) and [**] in name did not work in accurate mode

# 2.0.6 (04/2013) #
## General ##
  * update language files from Transifex (thanks to all translators!)
  * fixed typo in Edit Rom Collection dialog

## Import Games ##
  * try to scrape games with original name first (including (**) and [**])

## Launch Games ##
  * bugfix: check if delay parameters are available

# 2.0.5 (03/2013) #
## General ##
  * use xbmcvfs for file operations (better smb support and other improvements)
  * explicitly check for unicode characters when creating config.xml

## Launch Games ##
  * bugfix: launch game did not work from gameinfo screen
  * bugfix: issues with os.chdir in solo mode
  * always save viewstate before launching games

# 2.0.4 (03/2013) #
## General ##
  * added RCB to new "Game Add-ons" category in RetroPlayer branch

# 2.0.3 (02/2013) #
## General ##
  * check if RomCollections are available in config.xml. Launch config wizard if not.
  * check if games are available in MyGames.db. Launch game import if not.
  * check if we have access to rom and artwork paths. Cancel creation of config.xml if not.

## Import Games ##
  * always do a full reimport when in rescrape-mode
  * always do a full reimport when in local artwork-mode
  * better error handling after encoding errors during import
  * bugfix: checking subtitles during import did not work

## Browse Games ##
  * don't exit RCB when focus is on filter controls
  * always show game list after import. Also when import was canceled.
  * bugfix: check if database is available before gathering widget data

## Launch Games ##
  * add some more "intelligence" to applaunch.bat (solo mode)
  * use python 2.6 libraries for 7z handling (Windows only)
  * change working directory to emulator dir before launching game
  * libretro: added option to select gameclient manually
  * libretro: use "Edit game Command" to configure libretro cores per game

# 2.0.2 (02/2013) #
## Launch Games ##
  * bugfix: better handling of skin widget and solo mode
  * moved applaunch script files to addon\_data folder
  * new option: use VB script in solo mode
  * added startup delay to RCB service

# 2.0.1 (01/2013) #
## Launch Games ##
  * skin widget can invoke RCB to launch games
  * experimental: libretro support

# 2.0.0 (01/2013) #
## General ##
  * Frodo version bump

# 1.1.2 (01/2013) #
## General ##
  * bugfix: asking for Platform "Other" did not work in Add Rom Collection wizard
  * bugfix: no error message was shown after Add Rom Collection wizard
  * bugfix: old config.xml structure was not updated with MAME imageplacing options

## Browse Games ##
  * bugfix: issues with browsing games in Aeon Nox and Frodo RC3

## Launch Games ##
  * bugfix: using correct json command to toggle fullscreen
  * bugfix: backward compatibility for fullscreen toggle
  * new settings: pre- and post-launch delay

# 1.1.1 (12/2012) #
## General ##
  * bugfixes due to localization changes

# 1.1.0 (12/2012) #
## General ##
  * localization

## Import Games ##
  * error in scrape on startup: import message did not vanish anymore

## Browse Games ##
  * changed logic of applying filters: 1st click applies filter, 2nd click closes filter pane

# 1.0.9 (11/2012) #
## Browse Games ##
  * bugfix: MostPlayedRoms-widget in Aeon Nox caused RCB-loop on startup

# 1.0.8 (11/2012) #
## General ##
  * bugfix: script did not launch from home screen

## Browse Games ##
  * Frodo support: info dialog did not work anymore
  * Frodo support: change viewmode needs to be called manually since Frodo

# 1.0.7 (11/2012) #
## Browse Games ##
  * add fanart and launchCommand for skins to show on home screen

# 1.0.6 (11/2012) #
## Import Games ##
  * import of roms and artwork on smb shares (shares with username and password in path are not supported)
  * update archive.vg scraper to v2.0
  * bugfix: "Rom File Mask" changes after rescraping a single game
  * create artwork parent folder if not present

## Browse Games ##
  * Frodo support: games were not shown in Frodo nightlies (changes in addItem method)
  * provide properties of most played games for skins to show on home screen

## Launch Games ##
  * Frodo support: replace method executehttpapi with executejsonrpc
  * add option to exit disc selector without launching a game
  * bugfix: disc selector not working with games that have no description


# 1.0.5 (07/2012) #
## Import Games ##
  * "First 10 games could not be imported." -> option to continue and ignore error (patch submitted by pantherts)

## Launch Games ##
  * add before and after launch command (patch submitted by carabalb)
  * select disk in multi disk scenario (patch submitted by pantherts)
  * new option to use subprocess.Popen to launch emulators
  * using %PROGRAMFILES% variable in applaunch.bat

# 1.0.4 (05/2012) #
## Import Games ##
  * revert: bugfix for publisher / developer "989" caused problems

# 1.0.3 (05/2012) #
## General ##
  * open Addon settings from context menu

## Import Games ##
  * bugfix: error with publisher / developer "989"
  * bugfix: Import games with () in name with local single file scraper
  * change default values of "Don't import games without info / artwork"
  * re-scrape options:
    * rescrape single game
    * rescrape selection
  * new update option: don't overwrite properties with null values

# 1.0.2 (03/2012) #
## General ##
  * missing info / artwork dialog: select criteria to show or hide games with missing info / artwork
  * changed text of game description options in config wizard

## Import Games ##
  * bugfix: local nfo scraper did not find games with () in name

## Browse Games ##
  * bugfix: videos of games with "," in name did not play

# 0.9.9 (02/2012) #
## General ##
  * refactoring: move config wizard to separate module
  * refactoring: remove Camelot compatibility code
  * bugfix: remove and add Rom Collection in one turn caused errors

## Import Games ##
  * bugfix: import dialog is empty after "Edit offline scraper"

## Launch Games ##
  * bugfix: don't launch emulator if 7z file could not be extracted

# 0.9.8 (02/2012) #
## General ##
  * Add action 92 (backspace) to close dialogs

## Import Games ##
  * bugfix: Developer and Publisher not available in nfo files
  * set path to nfo folder
  * export nfo files on demand

# 0.9.7 (12/2011) #
## General ##
  * bugfix: loading skin files with PAL resolution might have failed

## Browse Games ##
  * bugfix: imageplacing option "Four small" did not work in Eden

# 0.9.6 (12/2011) #
## General ##
  * bugfix: config was not updated after Edit Rom Collection

## Import Games ##
  * new scraper: local artwork - don't scrape anything, just check for local artwork

## Browse Games ##
  * add video support to MAME views
  * Night skin: set focus on console filter when accessing filter controls

# 0.9.5 (12/2011) #
## Import Games ##
  * add archive.vg scraper to config.xml

## Browse Games ##
  * move autoplay video from script to skin
    * add new options to "Edit Rom Collection" dialog: autoplay video
    * remove imageplacing options with video support
  * improvement of browsing and list loading performance
  * more filter control interaction: all filter controls will be updated from left to right
  * add video support to Night showcase view
  * stop video when changing filters or launch context menu
  * bugfix: fullscreen video now works auto video playback is turned on
  * bugfix: game name does not change after video playback is stopped in game info dialog

# 0.9.4 (11/2011) #
## General ##
  * little refactoring of startup code (better timing and more stability)
  * don't crash when import zlib fails (not available with some python 2.6 distributions)

## Import Games ##
  * new scraper: http://archive.vg

## Browse Games ##
  * filter control interaction: update Genre, Year and Publisher filter when console is changed
  * short delay before applying filter selection
  * add background and extraImage1, 2, 3 to game info dialog
  * add console, version, perspective to game info dialog

# 0.9.3 (10/2011) #
## Browse Games ##
  * support different skins for game info view
  * don't reload game list when exiting game info view
  * small changes for better Eden compatibility

# 0.9.2 (10/2011) #
## General ##
  * ignore action id 0

## Game Import ##
  * add download url to nfo file
  * update thegamesdb scraper: download screenshot files
  * MAME scraper: revert change from 0.9.1

## Game Browsing ##
  * refactor game info window
    * video in game info window
  * add skin selection in addon settings: choose between Confluence, Night and Simplicity

# 0.9.1 (08/2011) #
## General ##
  * Edit Rom Collection dialog
    * friendly name for imageplacing options
    * wizard for new media path
    * default value for file mask
    * check if config.xml has errors before writing
  * Edit offline scrapers:
    * if descfilepergame = false: select path to game description (no file mask)
    * wizard for new scraper
    * select box with unused Rom Collection names
  * config wizard:
    * if descfilepergame = false: select path to game description (no file mask)
    * better support for standalone games
## Game Import ##
  * Import Options dialog
    * checkbox: Change scrapers for this run
  * stop import on general error
  * bugfix: error with [.md](.md) in rom path name (e.g. import of wrong images)
    * changed file check order: 1) rom name 2) game name
  * bugfix: error when using exactly 2 scrapers per rom collection
  * MAME scraper: removed scraping of flyer images

## Game Launching ##
  * support for standalone games: use "%ROM%" in emu Cmd

# 0.9.0 (06/2011) #
## General ##
  * reworked Confluence skin from PAL to 720p
  * slight usability changes in Confluence skin (navigation etc.)

## Game Browsing ##
  * reworked game info window in Confluence skin
  * favorites function
  * search function

# 0.8.12 (06/2011) #
  * Fixed whitespace issue on Xbox

# 0.8.11 (06/2011) #
  * bugfix: Edit Rom Collection dialog did not save changes in 0.8.10

# 0.8.10 (06/2011) #
  * platform.machine() caused errors on some Linux systems
  * updated scraper: thegamesdb.net

# 0.8.9 (06/2011) #
  * Eden compatibility: use xbmc.service instead of autoexec.py to perform startup tasks
  * use XBMC settings instead of status file to transfer status

# 0.8.7 (05/2011) #
  * removed option CACHESELECTION from caching options
  * bugfix game import: error with handling [.md](.md) in rom names

# 0.8.6 (05/2011) #
## General ##
  * complete "Edit Rom Collection" dialog: access all settings via UI
  * new dialog: "Edit Offline Scrapers"
  * new option: "Delete Rom Collection"
  * new option: "Clean database"
  * bugfix: fixed "autoexec.py not found" error
  * bugfix: set correct MAME properties when RC is created in local data mode

## Game Import ##
  * bugfix: using offline scrapers for MAME did not work

# 0.8.5 (04/2011) #
## General ##
  * using Dharma settings file as default

## Game Import ##
  * refactoring: code cleanup, little bug fixes, better error handling, ...
  * moved properties from Rom Collection to Scraper:
> > descfilePerGame, searchGameByCRC, useFoldernameAsCRC, useFilenameAsCRC
  * support regular expressions in diskPrefix
  * stop import when all games are imported with multigame scrapers

## Game Launching ##
  * support direct launching of savestates
    * specify savestatePath and saveStateParams per Rom Collection
    * RCB checks if savestate exists and offers to launch the savestate
  * new context menu option: Edit Game Command
    * save game specific command in database
    * replace %GAMECMD% with game specific command when launching the game
  * moved useEmuSolo from Addon settings to Rom Collection properties (config.xml)
  * new placholders in launchEmu: %ROMFILE%, %ROMNAME%, %GAME%, %ASKNUM%, %ASKTEXT%
  * check for multi rom games in zip files before launching

# 0.8.4 (04/2011) #
  * bug fix: adding more than 10 Rom Collections could cause database inconsistencies

# 0.8.3 (04/2011) #
  * encoding error workaround (Windows only)

# 0.8.2 (03/2011) #
## General ##
  * new option: Delete Game
  * bugfix: use uppercase "\Addon"-path in autoexec.py (Windows only)

## Configuration ##
  * option "Edit Rom Collection" in context menu
  * config wizard bugfixes and improvements

## Game Import ##
  * background scraping: start scraping on XBMC startup
  * encoding error fixes
  * better error handling on encoding errors

# 0.8.1 (02/2011) #
## General ##
  * rework of Confluence Thumbs view

## Game Import ##
  * scraping options: accurate, guess matches, select matches
  * new import options dialog (select Rom Collection, scraping mode and scrapers)
  * small fixes in MAME scraper


# 0.8.0 (01/2011) #
## General ##
  * added context menu
  * option "Add Rom Collection" available via context menu
  * reworked Confluence views

## Game Import ##
  * new scraper: maws.mameworld.info
  * rework of progress dialog (info about current scraper and current action)
  * bugfix: stop import when action is canceled

## Game Launching ##
  * detect games in zip and 7z archives and ask user which game to load


# 0.7.11 (12/2010) #
## General ##
  * no download of multiple images: check if file is available with different extension
  * bugfix: fallback images did not work in previous versions

## Xbox related ##
  * bugfix: Launching games on xbox was broken
  * set correct RomCollection-properties on xbox (create shortcuts, ...)
  * complete configuration can be done with the wizard (for roms and Xbox-games)

# 0.7.10 (12/2010) #
  * online scraping: improvements to sequel and subtitle handling


# 0.7.9 (12/2010) #
## Game Import ##
  * scraping game information and artwork from various online sources
  * current available scrapers: thegamesdb.net, giantbomb.com, mobygames.com
  * scraped artwork types: boxfront, boxback, cartridge, screenshot and fanart
  * create local nfo files while scraping
  * option to reimport local nfo files (possibility to add or edit game properties)
  * create info files about scrape results (missing game info, mismatches)

## Configuration ##
  * startup configuration wizard (create config.xml with most common options)
  * configure global settings via Addon Settings page
  * refactoring of config.xml structure
  * config.xml will be read at every start: no need to import settings anymore

# 0.6.1 (08/2010) #
## UI and general behaviour ##
  * fullscreen video browser
  * implemented different caching options: CACHEALL, CACHEITEM, CACHEITEMANDNEXT
  * added character filter: select games by first character
  * skinning support: all game properties are available in the skin xml now
  * delay videoplayback for one second: better behaviour when browsing the game list
  * added log level as parameter to config.xml
  * new option: preventUnfilteredSearch (unfiltered searches may cause problems with large rom collections)
  * commented config file
  * changed ordering in game list to case insensitive
  * support for pgup, pgdn, home, end
  * bugfix: don't restart video if we are playing the same file (while moving around but not changing selected game)

## Game Import ##
  * restructuring of import methods: scan large description files per game (previous version scanned the complete file at once causing out of memory errors on xbox)
  * changed behavior of progress dialog when importing games: progress update per game and not per rom collection
  * use default values for all settings: may keep config.xml more simple
  * check config.xml modification time at startup
  * new option: using foldername as crc value (useFoldernameAsCRC)
  * new option: using filename as crc value (useFilenameAsCRC)
  * ignore case when searching for media files (works also on linux)
  * limit number of subdirs when importing roms
  * bugfix: non-ascii chars in filenames during import
  * bugfix: unique constraint on game (name, romcollection)
  * bugfix: handle crc with leading zero
  * bugfix: handle game names with brackets [.md](.md)

## Game Launching ##
  * xbox support: able to launch emulators and xbox games
  * xbox support: create cut files for xbox on the fly (new settings: xboxCreateShortcut, xboxCreateShortcutAddRomfile, xboxCreateShortcutUseShortGamename)
  * toggle screenmode (fullscreen, minimized) if launching roms in non-solo mode

# 0.5.4 (08/2010) #
  * minimize XBMC before launching emulator
  * maximize XBMC after exiting emulator
  * using PAL as default resolution
  * new icon (thanks to freezy)
  * hungarian translation (thanks to alanwww1)

# 0.5.3 (08/2010) #
  * Dharma compatibility (installable via addon browser, slight code modifications with no impact to the end user)
  * changed the versioning scheme from Vx.y to x.y.z (this was needed to get this script submitted to the repo - and it is the better versioning scheme:))
  * no more writing to the scripts directory: all files will be written to userdata/addon\_data/script.games.rom.collection.browser. The file config.xml is still read from RCBs database directory. It will be backed up to the userdata directory after every "Import Settings" because XBMC will delete the complete RCB addon directory in case of an update.

# V0.5 (05/2010) #
## UI ##
  * new UI design (Confluence-like)
  * different views of the main window (Info, Info 2, Thumbs)
  * show video in main window
  * choose to show 1 big or 4 small images in Info and Info 2 view
  * configure different images for selected and non-selected items in Info or Thumbs view
  * better performance while loading game list
  * game counter
  * display console name of selected game
## Game Import ##
  * import images for developer, publisher, console or rom collection
  * find game in description file by crc value
  * check crc value of files inside a zip archive (1 file per archive only)
  * import roms in sub folders
  * more robust game description parser
  * check config.xml for common errors before importing
  * different log levels



# V0.4 (03/2010) #
  * new game info view: pressing info button when a game is selected will open a new window with additional game information
  * showing video in game info view
  * dynamic image placing: RCB has 8 different controls to show images. The image type (screenshot, cover, ...) can be configured for every control.
  * dynamic image types: there won't be fix image categories anymore. You can define your own image types (e.g. ingame screenshots, title screenshots, highscore screenshots, ...) and use this categories to configure image placing. Actually you could use 8 different image types or 7 image types and 1 video type (video window overlays one of the image controls).



# V0.3 (03/2010) #
  * solved problem with executing batch file in windows
  * using autoexec.py to launch RCB when restarting in solo mode
  * saving and loading view state when relaunching RCB
  * update entries during "import settings" and "update db"
  * added support for multiple rom paths per rom collection
  * importing games without game description
  * better performance while loading game list
  * added info label (shows information during import)
  * sort filter list items alphabetically
  * new Rom Collection property "ignoreOnScan": no changes to this collection during import
  * new Game properties (imported via description file): developer, reviewer, maxPlayers, rating, votes, url, region, media, perspective, controller
  * new global settings: showEntryAllConsoles, showEntryAllGenres, showEntryAllYears, showEntryAllPublisher, saveViewStateOnExit, saveViewStateOnLaunchEmu

# V0.2 (03/2010) #
  * parser bug fixes

# V0.1 (02/2010) #
  * initial version