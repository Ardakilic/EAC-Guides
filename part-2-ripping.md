# How to Rip CDs Perfectly on Windows Using Exact Audio Copy (EAC) Part 2: Ripping

## Prerequisites

1. You've set up EAC using Part 1 of my guide.
2. You have a music CD you want to rip. An original copy, not a burned one on a CD-R or CD-RW.

> **Tip:** Click on any image in this guide to view it at full resolution.

## Open EAC

Insert your CD into your CD drive and open EAC. A CTDB Metadata Lookup window will pop up.

[![Step 1](/img/eac-ripping/step-01.png)](/img/eac-ripping/step-01.png)

With this window you can prepopulate metadata fields in EAC using info from [MusicBrainz](https://musicbrainz.org/) (music note icon), [Discogs](https://www.discogs.com/) (vinyl icon), or [freeDB](http://www.freedb.org/) (freeDB icon).

Select the best option for your CD and click OK.

## Tagging

[![Step 2](/img/eac-ripping/step-02.png)](/img/eac-ripping/step-02.png)

If you prepopulated fields in the previous step then you only have to edit tags to your liking instead of typing every single tag in by hand. Don't forget to check for spelling mistakes. Having to rerip an entire CD because of a typo really sucks.

I would make sure at least these fields are filled out correctly before ripping:

* Track number (for each track)
* Title (for each track)
* CD Artist
* CD Title (the album name)
* Year
* CD Number (on the right side of the main window)
* Number Of CDs (on the right side of the main window)

> If your CD contains music by Various Artists then edit the CD Artist tag to be Various Artists and set the individual Artist tag for each track using the Artist column in the table. Filling out at least one field in the Artist column will cause the Various Artists file naming scheme to kick in too.

[![Step 3](/img/eac-ripping/step-03.png)](/img/eac-ripping/step-03.png)

If you don't want to worry about which words should be capitalized then you can capitalize the first letter of each word in all tags using the action shown in the image above. I always do this so I don't end up wasting time fretting over a few characters.

[![Step 4](/img/eac-ripping/step-04.png)](/img/eac-ripping/step-04.png)

The action shown in the above image will remove spaces you might not notice at the beginning or end of tags.

## Gap Detection & CUE Sheet

[![Step 5](/img/eac-ripping/step-05.png)](/img/eac-ripping/step-05.png)

A small window will pop up. Wait for it to finish.

[![Step 6](/img/eac-ripping/step-06.png)](/img/eac-ripping/step-06.png)

A small window will pop up. Wait for it to finish.

## Ripping

[![Step 7](/img/eac-ripping/step-07.png)](/img/eac-ripping/step-07.png)

An Extracting Audio Data window will pop up. It will take from 30 minutes up to 2 hours rip your CD depending on how scratched it is.

If your CD is too scratched then there's a chance that EAC will get a bunch of read errors while trying to read a heavily scratched area of the CD. If EAC seems to not be moving forward because of errors and the Est. Remaining time keeps going up then there's not much you can do except rip another copy of your CD that's in better condition.

[![Step 8](/img/eac-ripping/step-08.png)](/img/eac-ripping/step-08.png)

Click OK after ripping is complete. The image above shows it took about 30 minutes to rip my unscratched CD. Pretty quick for 19 tracks.

## Wrap Up

[![Step 9](/img/eac-ripping/step-09.png)](/img/eac-ripping/step-09.png)

The image above shows the results of the rip: the audio files (.flac), a cue sheet (.cue), and a status report (.log). Keeping the log is important because it is proof that each track on the CD was ripped perfectly.

Keep the cue sheet too. It's needed if you ever want to burn a copy of the CD you just ripped.

Open the log file and confirm that at the bottom it says that all tracks were accurately ripped and that no errors occurred. The output from the CUETools DB Plugin at the bottom should also say that each track was accurately ripped.

And that's it. You're done!
