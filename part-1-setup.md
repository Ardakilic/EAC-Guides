# How to Rip CDs Perfectly on Windows Using Exact Audio Copy (EAC) Part 1: Setup

## What You Need

1. A laptop computer, desktop computer, or virtual machine running Windows 7, 8, or 10.
2. A CD drive internal to your computer or an external USB CD drive.
3. A relatively popular music CD. An original copy, not a burned one on a CD-R or CD-RW.
4. Exact Audio Copy. At the time of writing this post the latest version of EAC is v1.3. Always use the latest version of EAC. You can download EAC for Windows [here](http://www.exactaudiocopy.de/en/index.php/resources/download/).

> **Tip:** Click on any image in this guide to view it at full resolution.

## Installation

Download the EAC installer and save it to your Desktop. Double click on the installer and go through the on-screen prompts as normal until you get to the Choose Components section.

[![Step 1](/img/eac-setup/step-01.png)](/img/eac-setup/step-01.png)

Change the options on your screen so that it matches the image above and then click Install.

## Open EAC

After opening EAC you'll be greeted with the window below.

[![Step 2](/img/eac-setup/step-02.png)](/img/eac-setup/step-02.png)

Click Cancel. We won't be using the setup wizard.

Now take your relatively popular CD and insert it into your CD drive. Look for the window below to show up.

[![Step 3](/img/eac-setup/step-03.png)](/img/eac-setup/step-03.png)

If it doesn't, keep trying other CDs until it does. Once it does, click Configure.

[![Step 4](/img/eac-setup/step-04.png)](/img/eac-setup/step-04.png)

After it's done configuring you'll see the screen above. Click OK.

## EAC Options

Go to the menu bar in the top left-hand corner of EAC and select EAC Options.

[![Step 5](/img/eac-setup/step-05.png)](/img/eac-setup/step-05.png)

> Go to the tab displayed in each image below and make your settings match what's shown in each image.

[![Step 6](/img/eac-setup/step-06.png)](/img/eac-setup/step-06.png)

[![Step 7](/img/eac-setup/step-07.png)](/img/eac-setup/step-07.png)

[![Step 8](/img/eac-setup/step-08.png)](/img/eac-setup/step-08.png)

[![Step 9](/img/eac-setup/step-09.png)](/img/eac-setup/step-09.png)

For easy modification of the settings above you can copy and paste the text below.

Naming Scheme:
```
%tracknr2% - %title%
```

Various Artists Naming Scheme:
```
%tracknr2% - %artist% - %title%
```

[![Step 10](/img/eac-setup/step-10.png)](/img/eac-setup/step-10.png)

In the settings above the only thing I changed was the replacement character for a colon (4th from the top) from a hyphen to a semicolon. This change makes it so each character replacement unique. Now if you a see a hyphen in a file name, there's only one thing it could be a replacement of: a backslash (2nd from the top).

[![Step 11](/img/eac-setup/step-11.png)](/img/eac-setup/step-11.png)

## Drive Options

Next, open Drive Options.

[![Step 12](/img/eac-setup/step-12.png)](/img/eac-setup/step-12.png)

> Go to the tab displayed in each image below and make your settings match what's shown in each image.

Click OK to dismiss the small dialog that pops up. You'll see the screen below.

[![Step 13](/img/eac-setup/step-13.png)](/img/eac-setup/step-13.png)

Make sure there is a CD in your CD drive and then click Detect Read Features.

[![Step 14](/img/eac-setup/step-14.png)](/img/eac-setup/step-14.png)

[![Step 15](/img/eac-setup/step-15.png)](/img/eac-setup/step-15.png)

The only feature we care about is Accurate Stream. Make a mental note of whether it says Yes or No for Accurate Stream for your CD drive and then click OK.

[![Step 16](/img/eac-setup/step-16.png)](/img/eac-setup/step-16.png)

Change your settings to match the image above. If Accurate Stream displayed No in the previous step for you, uncheck the Drive has 'Accurate Stream' feature box in your own settings. Regardless of what the results of the previous step showed for the Caching and C2 Error Info features for your CD drive, leave the Drive caches audio data box checked and the Drive is capable of retrieving C2 error information box unchecked like in the image above.

[![Step 17](/img/eac-setup/step-17.png)](/img/eac-setup/step-17.png)

Make sure there is a CD in your CD drive and then click Autodetect read command now.

[![Step 18](/img/eac-setup/step-18.png)](/img/eac-setup/step-18.png)

The correct option for your CD drive will be selected for you. You can see the read command it selected for my CD drive in the image above. It's ok if the read command for your CD drive is different than what's shown in the image above.

On the Offset / Speed tab you'll see the screen below.

[![Step 19](/img/eac-setup/step-19.png)](/img/eac-setup/step-19.png)

Next, we're going to find out whether or not the Overread into Lead-In and Lead-Out box should be checked.

To do this, start by unchecking the Use AccurateRip with this drive box.

[![Step 20](/img/eac-setup/step-20.png)](/img/eac-setup/step-20.png)

Next, make sure there is a CD in your CD drive and then click Detect read sample offset correction.

[![Step 21](/img/eac-setup/step-21.png)](/img/eac-setup/step-21.png)

Make a mental note of what it says for Overread and then click OK.

Back on the Offset / Speed tab, check Overread Lead-In and Lead-Out only if the result said that your drive can overread from both the Lead-In and Lead-Out, if it said Lead-Out and your Read sample offset correction value is positive, or if it said Lead-In and your Read sample offset correction value is negative. Otherwise, leave it unchecked.

[![Step 22](/img/eac-setup/step-22.png)](/img/eac-setup/step-22.png)

Before moving onto the next tab don't forget to check the Use AccurateRip with this drive box again like in the image above.

[![Step 23](/img/eac-setup/step-23.png)](/img/eac-setup/step-23.png)

There are three options for the Gap/Index retrieval method: Detection method A, B, and C. Apparently method A is the fastest and method C is the slowest. Pretty much every drive should work with the settings shown in the image above. If your CD drive stalls on detecting gaps or detects gaps that are obviously wrong like 30 second gaps on a non-live album, then try Detection methods B and C. If all detection methods fail, switch Detection accuracy from Secure to Accurate and try again.

## Compression Options

Next, open Compression Options.

[![Step 24](/img/eac-setup/step-24.png)](/img/eac-setup/step-24.png)

> Go to the tab displayed in each image below and make your settings match what's shown in each image.

[![Step 25](/img/eac-setup/step-25.png)](/img/eac-setup/step-25.png)

For easy modification of the Additional command-line options setting seen in the image above you can copy and paste one of the two sets of command-line parameters from the text below.

All Fields:
```
-8 -V -T "TRACKNUMBER=%tracknr%" -T "TITLE=%title%" -T "ARTIST=%artist%" -T "ALBUMARTIST=%albumartist%" -T "ALBUM=%albumtitle%" -T "DATE=%year%" -T "TOTALTRACKS=%numtracks%" -T "DISCNUMBER=%cdnumber%" -T "TOTALDISCS=%totalcds%" -T "PERFORMER=%albuminterpret%" -T "COMPOSER=%composer%" -T "GENRE=%genre%" %haslyrics%--tag-from-file=LYRICS="%lyricsfile%"%haslyrics% -T "COMMENT=%comment%" %source% -o %dest%
```

Minimal Fields:
```
-8 -V -T "TRACKNUMBER=%tracknr%" -T "TITLE=%title%" -T "ARTIST=%artist%" -T "ALBUMARTIST=%albumartist%" -T "ALBUM=%albumtitle%" -T "DATE=%year%" -T "TOTALTRACKS=%numtracks%" -T "DISCNUMBER=%cdnumber%" -T "TOTALDISCS=%totalcds%" %source% -o %dest%
```

[![Step 26](/img/eac-setup/step-26.png)](/img/eac-setup/step-26.png)

## Metadata Options

[![Step 27](/img/eac-setup/step-27.png)](/img/eac-setup/step-27.png)

> Go to the tab displayed in each image below and make your settings match what's shown in each image.

[![Step 28](/img/eac-setup/step-28.png)](/img/eac-setup/step-28.png)

Click the Show options of the selected metadata provider button shown in the image above.

[![Step 29](/img/eac-setup/step-29.png)](/img/eac-setup/step-29.png)

Modify the settings in the pop up window to look like the image above and then click OK.

[![Step 30](/img/eac-setup/step-30.png)](/img/eac-setup/step-30.png)

Literally put email@email.com in the Your e-mail address setting shown in the image above. After your settings match the image above, click Get active freedb server list. Finally, click OK at the bottom of the window to close out of Metadata options.

The last step is to save your configuration.

[![Step 31](/img/eac-setup/step-31.png)](/img/eac-setup/step-31.png)

You can find what's shown in the image above at the bottom of the main EAC window. Click the New button after you find it.

[![Step 32](/img/eac-setup/step-32.png)](/img/eac-setup/step-32.png)

Type in a name for your configuration profile and then click OK.

## Ripping

Now you're ready to rip CDs with EAC! Check out [Part 2](part-2-ripping.md) of my guide to learn how.
