# YouTube-Checker-to-NewPipe
Replaces subscriptions from [NewPipe](https://newpipe.schabi.org/) with those exported by [YouTube Checker](https://github.com/XrXr/YoutubeSubscriptionChecker)

Basically I don’t really care to use an account for watching YouTube, so I use [YouTube Checker](https://github.com/XrXr/YoutubeSubscriptionChecker) as a Firefox addon on my desktop and [NewPipe](https://newpipe.schabi.org/) on my Android.  To synchronize my “subscriptions” between them, I created this little script.

*Warning:* This is a one way synchronization from [YouTube Checker](https://github.com/XrXr/YoutubeSubscriptionChecker) to [NewPipe](https://newpipe.schabi.org/).  The current version doesn’t try to merge subscriptions and you cannot synchronize from [NewPipe](https://newpipe.schabi.org/) to [YouTube Checker](https://github.com/XrXr/YoutubeSubscriptionChecker).  Maybe I will add this in the future, but right now this is simply not my use case.

## Dependencies
- Python3

## Usage
`./youtube-checker-to-newpipe.py subs.json newpipe-subscriptions.json`

A new file will be created with subscriptions from the YouTube Checker.  
After running this script, import the JSON file to replace your subscriptions.  

### Steps to export YouTube Checker subscriptions
1. Click on Settings  
2. Go to Import/Export  
3. Click the Export button  
4. Copy all of the output into a file (e.g. subs.json)

### Steps to import SkyTube subscriptions
1. Go to your subscriptions  
2. Click on Import/Export  
3. Select import from previous export and select the `newpipe-subscriptions.json`.

## Alternatives
If you prefer to use [SkyTube](https://skytube-app.com/), I’ve also created a script for that: [YouTube-Checker-to-SkyTube](https://github.com/jonasw234/YouTube-Checker-to-SkyTube)
