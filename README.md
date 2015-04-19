# Piwik ClickHeat Plugin

## Description
ClickHeat is a visual heatmap of clicks on a HTML page, showing hot and cold click zones. This plugin based on [Dugwood's ClickHeat version 1.14](https://github.com/dugwood/clickheat). It is an OpenSource software, released under GPL licence, and free of charge.

## Installation
Install it via Piwik Marketplace.

This plugin installer will make directories:
* yourpiwik/tmp/cache/clickheat/cache
* yourpiwik/tmp/cache/clickheat/logs.

This plugin uses a different tracker. Please click on the link "JavaScript" and put the special Javascript codes into your website.

## FAQ
__What exactly is included in this feature ?__

* pick up a siteid
* pick up a period
* pick up a browser type
* pick up a specific web page

__And what functions are not included in this feature ?__

* remove special addresses defined on the control panel.
* remove special browsers defined on the control panel.
* filters based on added segmentation

__Where is the coordinate information from the browser ?__

ClickHeat plugin uses text files to record the coordinate data of each browser in directory: yourpiwik/tmp/cache/clickheat/logs. 

__Does it withstands high traffics ?__

Unfortunately not. Because this plugin uses text files to record data. Therefore, please use this plugin to experiment or low traffics.

__New click data were added, but not updated heatmap. Why ?__

Plugin places heatmap images in the cache directory: yourpiwik/tmp/cache/clickheat/cache. Therefore when you suddenly met with such probrem, you can delete cache files (__do not delete cache directory__).

__Showed a heatmap, but not overlay a heatmap to the target web page. Why ?__

Check that your website does not set the HTTP header __X-FRAME-OPTIONS__ to __SAMEORIGIN__ as this will prevent this plugin from iframing your website for the heatmap report. Please see [Page Overlay Troubleshooting](http://piwik.org/docs/page-overlay/#page-overlay-troubleshooting), that is same problem. 

## Changelog
* 0.1.0 First beta

## License
GPL v3 or later

## Support
Please direct any feedback to [yamachan@piwikjapan.org](mailto:yamachan@piwikjapan.org).

