# TDT Export Protocol
Valerie's method for exporting photometry data collected in synapse to csvs.

# Overview
1. Folder structure
2. Export template
3. Exporting

# 1. Folder structure
Overarching folder structure should be as follows:

	COHORT:
•	DAY/EXPERIMENT PHASE
o	ANIMAL ID
	405.csv 
	470.csv
	TTL.csv

o	Bravo has found that it’s faster to create folders for each animal in the big export folder and move them once exported to a subfolder for each day [SCREENCAP THIS TOO]

# 2. Export template
	Files to export are organized in the following manner: [SCREENCAP HERE]

Type: 405, 470, TTL (THESE ARE ALL CURRENTLY SET FOR SYSTEM 1/A)

To change these to system 2/b, right click on the 405/470/TTL. This will open a menu that allows you to select the signal type. To change to B, select 45b for 405 and 47b for 470. TTL is Wav4 regardless of the system. [SCREENCAP HERE]

Export path: Each group of 405, 470, TTL is currently set to export to a folder named by experiment subject. (bravo has found that keeping paths as similar as possible between exports streamlines the process)

When changing cohorts (new experiment subject IDs), you must change the export paths for each file [SCREENCAP]:

Ie, ‘D:/T7 Shield/photometry/cohort3/D14/48_2/405.csv’ -> ‘D:/T7 Shield/photometry/cohort4/D1/12_2/405.csv’

# 3. Exporting 
-	Open the OpenBrowser application (should be on the desktop): [ICON HERE]
-	Load valerie’s photometry template: [INCLUDE .OBM FILE IN GITHUB REPO]
- Tank is loaded (Juan’s Dual Photometry nightmare)
- File to export: select the file to export by right clicking on the file name. this will open a menu that allows you to select the file of interest. Don’t worry about 405 vs 470 vs TTL for this step (this is specified by the Type you choose for the given file). These files are organized by the date they were recorded on, with the oldest on top and newest on the bottom. There are a lot of files. Relevant information (date recorded) will take a second to load, so either wait or scroll down all the way. (TIP: file names of recordings contain a lot of useful information. Assuming u used different animal IDs, files will be named accordingly, and will also contain the date (if you’re impatient)): [EXAMPLE FORMAT HERE WITH ID AND DATE BOLDED]
- Select and load the according files u want exported. Theres really no easy or fun way to do this.
- It may streamline things to do this one day at a time (since you will only be exporting 1 days worth of data at a time using bravo’s method). This also saves u some scrolling.
-	When the relevant information is loaded, select the files you want to export and export the selected rows. Once files are exported, open file manager to double check files were correctly populated, then copy folders into a folder for the Day you just exported data from. If you do not do this, this data will be saved over!
-	Repeat until all days of interest are exported. You should end up with folders of data that look like this [FLOW DIAGRAM]:
- Cohort -> days -> folders for each animal -> 405, 470, TTL
