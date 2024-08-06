### TODO
- [ ] Check character sequence problem
- [ ] `How often does inReach Mini 2 check for messages?
every hour When you send a message, your device listens for replies for 10 minutes. The device also checks for new messages every hour.` To test.

### Garmin transmission

### Step-by-Step utilization
1. A message come from Garmin InReach with the request params for the grib to download.
2. The server will read the message and create a gribmail request to Squid servers
3. When the email arrives, the server will compact the grib file using lossless compression.
4. Server split the compressed file into $$n = file\_dim/max\_msg\_length$$ For now $max\_msg\_length = 120$, cause of limitations of garmin max msg length.


### Protocols
