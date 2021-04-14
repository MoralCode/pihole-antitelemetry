# pihole-antitelemetry
[Research](https://www.scss.tcd.ie/doug.leith/apple_google.pdf) shows Google collects 20x more data from Android than Apple collects from iOS. Block both using these pihole lists.

## Project Goals

The goal of these blocklists is to to provide an easy blocklist for the domains in the paper to make it easy for people to block as much passive, idle collection of personal data as possible while providing choice when it comes to breaking functionality of existing apps. 

This is a community curated list that focusses fairly narrowly on domains from the linked paper (or similar sources) that are used by large tech companies to collect telemetry from our devices while they are idle. The intention is to create a list that maintainers of existing lists (see below) can study or integrate into their own lists or otherwise use to help the community.

These lists are mainly focussed on Apple and Google because they were the subjects of the paper.

## The lists
For a list of domains that should not break anything, use `telemetry-domains.txt`.

If you want to also block domains that are not well-tested, add `telemetry-domains_beta.txt` to the list. 

Domains that are known to break user-facing services or apps are moved to `telemetry-domains_borked.txt` for use at your own risk.

These lists are maintained with help from the community. Any efforts to help sort domains into the correct blocklists will help others better block non-consensual telemetry.

## Existing lists
- [NextDNS apple list](https://github.com/nextdns/metadata/blob/master/privacy/native/apple)
- [mischosts apple telemetry list](https://github.com/llacb47/mischosts/blob/master/apple-telemetry)
- https://decloudus.com/
- https://filterlists.com/
- https://github.com/crazy-max/WindowsSpyBlocker
- 