# Sonarr_Parsarr

This will remove stalled torrents and add them to the blocklist.

It will send an API call to sonarr to get all the active downoalds.  
It will then itterate through the list of torrents, and mark all the stalled (Warning status) sorrents with a strike.
It will remove a strike for any torrent with a "Downloading" status

For any torrent that reaches 3 strikes, it will send an API call to sonarr to remove the problem torrent and add it to the blocklist.

This will also trigger a new search for the same eppisode.


Dont forget to add your Sonarr API key.

I added this as a task in Task Scheduler to run every 10 minutes.
If you are having issues with the Task Scheduler not running the script, Make sure the CSV file is in the same directory as the script.  
