# pihole-antitelemetry
[Research](https://www.scss.tcd.ie/doug.leith/apple_google.pdf) shows Google collects 20x more data from Android than Apple collects from iOS. Block both using these pihole lists.

The goal of these blocklists is to limit as much of this passive, while-idle telemetry as possible without breaking things. The intent is for this list to be used to supplement existing lists (see below) with domains from the paper linked above.

This project is currently a work-in progress. Feel free to contribute by submitting issues or pull requests.

## The lists
For a list of domains that should not break anything, use `telemetry-domains.txt`. If you want to also block domains that are not well-tested, add `telemetry-domains_beta.txt` to the list. known-broken domains are moved to `telemetry-domains_borked.txt`.

Any help with testing domains is appreceated


## Existing lists
- [NextDNS apple list](https://github.com/nextdns/metadata/blob/master/privacy/native/apple)
- [mischosts apple telemetry list](https://github.com/llacb47/mischosts/blob/master/apple-telemetry)
- https://decloudus.com/