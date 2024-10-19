# Ripping Disks

## 1st Time Setup

1. Download [MakeMKV](https://www.makemkv.com/)
    1. if ripping BluRays you'll need a license. This is [free and can be found here](https://forum.makemkv.com/forum/viewtopic.php?t=1053) while MakeMKV is in Beta
1. In MakeMKV
    - Click the Wrench Icon
    - Click the "General" Tab
    - Check the box for "Expert Mode" (this will let you edit the name of the output files)

## Common Steps for Movies and TV Shows

1. Locate what you plan to extract from a disk on one of
    - TMDB (The Movie DB)
    - TVDB (Television DB)
    - IMDB (Internet Movie Database)
1. Pay attention to the Title and Year.
    - TV Show Example:
        - Firefly (2002) [TVDB](https://www.thetvdb.com/series/firefly) [IMDB](https://www.imdb.com/title/tt0303461/)
    - Movie Example:
        - Serenity (2005) [TMDB](https://www.themoviedb.org/movie/16320-serenity?language=en-US) [IMDB](https://www.imdb.com/title/tt0379786/)
1. Move on to [TV Show](/#tv-Show) or [Movie](/#movie) instructions. (Click the link to jump there)

## TV Show

### Creating your output folders

1. Open File Explorer and go to the folder where you want to put the TV Series.
1. Make a folder with the name of your series (found in the DB above). Then make a subfolder for the season. (if you haven't already)
   - Example: `Firefly (2002)/Season 1/`
1. If you move on to another season, then add a folder for that season under the series folder.
```
Example:

Firefly (2002)
-- Season 1
-- Season 2
```

### Getting your settings ready

1. Open MakeMKV.
1. Click on the 🔧 (Wrench) icon in MakeMKV.
1. Go to the `Advanced` Tab.
1. Put the text `{NAME1}{M2}` into the box next to "Output file name template". This will make renaming your files easier later.
1. Click the `OK` button.

### Ripping a Disk

1. Now that your settings are right, put your disk in the drive and click the big 📀 (DVD Drive) Icon to scan the disk
1. You should now have a "DVD disc" and list of titles that can be pulled off the disk.
1. Click on the top item who's type is "DVD Disc".
1. To the right under "Properties", name the disk you are ripping `Title (Year) - S##D#` where `Title (Year)` comes from above, `S##` is the season number like `S01`, and `D#` is the disk number for the season like `D1`
   - Example: `Firefly (2002) - S01D1`
1. Clicking in any blank space will cause the rename to show on the left and all the titles should have the new name.
1. Deselect any title on the disk that are not needed (this could be bonus features, or if there is a title that spans all episodes)
1. Click the 📂 (folder) next to the "Output Folder" text box.
1. Find and select the season folder you made to put your episodes in. After clicking "Select Folder", the text box should look approximately like `/path/to/your/videos/Name of Show/Season #/`.
1. At this point we're ready to go! Click the Hard Drive Icon with an arrow in the top right to start ripping MKV files!
1. At the end you should have files that look like 
```
Firefly (2002)
  Season 1
    Firefly (2002) - S01D101.mkv
    Firefly (2002) - S01D102.mkv
    Firefly (2002) - S01D103.mkv
```
11. At this point, you can eject your disk and start a new disk. Go back to [Ripping a Disk](#ripping-a-disk) if you have more disks to do.
1. If you are done with all your disks, it will look something like
```
Firefly (2002)
  Season 1
    # First Disk
    Firefly (2002) - S01D101.mkv
    Firefly (2002) - S01D102.mkv
    Firefly (2002) - S01D103.mkv
    #Second Disk
    Firefly (2002) - S01D201.mkv
    Firefly (2002) - S01D202.mkv
    Firefly (2002) - S01D203.mkv
```
13. Now you need to make sure that your episodes are properly labeled. If your disks are in order and there is no gaps between episodes, then you can use a program like [AdvancedRenamer](https://www.advancedrenamer.com/download) to rename the regex pattern `D\d+` to a 2 digit ascending number prefixed with an E (Example: `E01`).
    - Instructions TBD on this.
1. If you have gaps or your episodes are out of order, then you may need to do some (or a lot) of manual work here.
1. Once you are done, your episodes should look something like this
```
Firefly (2002)
  Season 1
    Firefly (2002) - S01E01.mkv
    Firefly (2002) - S01E02.mkv
    Firefly (2002) - S01E03.mkv
    Firefly (2002) - S01E04.mkv
    Firefly (2002) - S01E05.mkv
    Firefly (2002) - S01E06.mkv
```
16. You're done with ripping the disks for this series! Proceed to [processing a rip to reformat it](#processing-a-rip-to-shrinkreformat-it)

## Movie
Note: these instructions are in progress

1. Make a folder with the above name
1. Tweak the settings for output file to be `{NAME1}`
1. Name the disk the above name.
1. Select any titles that need to be ripped (Likely only one title unless there is multiple versions on the disk)
    1. If there is more than 1 version name them with the suffix ` {Edition-EditionName}`
        - Example: ` {Edition-3D}`
        - Example: ` {Edition-Theatrical}`
    2. Note: if there is a wide and fullscreen version, it is likely that one is just a crop of the other. Rip both, but only keep the one with the larger frame.

# Processing a Rip to Shrink/Reformat it
Note: these instructions are in progress

## Common Steps

## DVD

## HD-DVD

## BluRay

## 4K-BluRay
