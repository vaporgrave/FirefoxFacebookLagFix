# Facebook Lag Fix for Firefox Quantum 

A fix addressing the overwhelming CPU/RAM load caused by having Facebook open.  This was accomplished using the uBlock Origin 1.14.10 add-on and a combination of dynamic filtering rules on Firefox Quantum 57.0b5 (64-bit).  So far that is the only environment I have tested this in.
<br>
<br>

# Installation

### Firefox Quantum 57.0b5 (64-bit) 

```
https://www.mozilla.org/en-US/firefox/channel/desktop/#beta
```

### uBlock Origin 1.14.10

```
https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/
```

```
Add the uBlock Origin extension to Firefox. 
```

### uBlock Origin Settings & Dynamic Filters + Final Steps

Now head over to:

```
https://github.com/vaporgrave/FirefoxFacebookLagFix/releases/tag/v1.0
```

where you will download two text files named: 

```
uBlockOriginLagFixSettings.txt & LagFixDynFilteringRules.txt
```

Once you have downloaded both text files type "about:addons" in to Firefox's address bar.  This will open the Add-ons Manager.  Locate uBlock Origin on the list and click the 'Options' button, scroll to the bottom of the page that appears and click on the "Open the Dashboard" link.

You will now be in the uBlock Origin Dashboard.  Make sure you have the "Settings" tab selected.  At the bottom of that page is a button that says "Restore from file...", click that and upload the "uBlockOriginLagFixSettings.txt" file you downloaded.  Next, go to the "My Rules" tab and click the "Import from file..." button underneath "Temporary Rules" and upload the "LagFixDynFilteringRules.txt" file you downloaded.  Click the "Commit" and that will make the rules permanent so you don't have to upload a text file each time you start your browser.

Make sure uBlock Origin is turned on by clicking it's icon on your browser's toolbar and then clicking on the grey power button, that once selected will turn blue.

When you navigate to "https://www.facebook.com" the page will not be pretty, but it is functional.  Profile pictures will be missing, that's the only aesthetic issue I discovered.  Besides that, you should notice a massive decrease in the amount of memory and processing power being used by Firefox to have Facebook open.   I went from ~70% CPU usage with jumps to 99%, and ~60%-80% RAM usage to ~1-10% CPU and ~20%-30% RAM.
<br>
<br>

Hopefully this fix works for you.
Enjoy!
