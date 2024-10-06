# Ripping Disks

## 1st Time Setup

1. Download [MakeMKV](https://www.makemkv.com/)
    1. if ripping BluRays you'll need a license. This is [free and can be found here](https://forum.makemkv.com/forum/viewtopic.php?t=1053) while MakeMKV is in Beta
1. In MakeMKV
    - Click the Wrench Icon
    - Click the "General" Tab
    - Check the box for "Expert Mode" (this will let you edit the name of the output files)

## Common Steps

1. Locate what you plan to extract from a disk on one of
    - TMDB (The Movie DB)
    - TVDB (Television DB)
    - IMDB (Internet Movie Database)
1. Pay attention to the Title and Year.
    - TV Show Example:
        - Firefly (2002) [TVDB](https://www.thetvdb.com/series/firefly) [IMDB](https://www.imdb.com/title/tt0303461/)
    - Movie Example:
        - Serenity (2005) [TMDB](https://www.themoviedb.org/movie/16320-serenity?language=en-US) [IMDB](https://www.imdb.com/title/tt0379786/)

## Multi-Disk TV Show

1. Make a folder with the above name. Then make a subfolder for the season.
```
Example:

Firefly (2002)
-- Season 1
```
2. Tweak the settings for output file to be `{NAME1}{M2}`
2. Name the disk you are ripping `Title (Year) - S#D#` where `S##` is the season number like `S01` and `D#` is the disk number for the season like `D1`
2. Deselect any title on the disk that are not needed (this could be bonus features, or if there is a title that spans all episodes)
2. The final results will be something like 
```
# First Disk
Firefly (2002) - S01D101.mkv
Firefly (2002) - S01D102.mkv
Firefly (2002) - S01D103.mkv

#Second Disk
Firefly (2002) - S01D201.mkv
Firefly (2002) - S01D202.mkv
Firefly (2002) - S01D203.mkv
```
6. Use a program like [AdvancedRenamer](https://www.advancedrenamer.com/download) to rename the regex pattern `D\d+` to a 2 digit ascending number prefixed with an E (Example: `E01`).
6. Now the output will look something like
```
Firefly (2002) - S01E01.mkv
Firefly (2002) - S01E02.mkv
Firefly (2002) - S01E03.mkv
Firefly (2002) - S01E04.mkv
Firefly (2002) - S01E05.mkv
Firefly (2002) - S01E06.mkv
```

## Movie

1. Make a folder with the above name
1. Tweak the settings for output file to be `{NAME1}`
1. Name the disk the above name.
1. Select any titles that need to be ripped (Likely only one title unless there is multiple versions on the disk)
    1. If there is more than 1 version name them with the suffix ` {Edition-EditionName}`
        - Example: ` {Edition-3D}`
        - Example: ` {Edition-Theatrical}`
    2. Note: if there is a wide and fullscreen version, it is likely that one is just a crop of the other. Rip both, but only keep the one with the larger frame.

# Processing a Rip to Shrink/Reformat it

## Common Steps

## DVD

## HD-DVD

## BluRay

## 4K-BluRay
