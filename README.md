# Sonarr_Parsarr

This will remove stalled torrents and add them to the blocklist.

It will send an API call to sonarr to get all the active downoalds.  
It will then itterate through the list of torrents, and mark all the stalled (Warning status) sorrents with a strike.
It will remove a strike for any torrent with a "Downloading" status

For any torrent that reaches 3 strikes, it will send an API call to sonarr to remove the problem torrent and add it to the blocklist.

This will also trigger a new search for the same eppisode.
