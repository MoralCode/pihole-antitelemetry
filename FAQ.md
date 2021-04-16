# FAQ

Answers to questions that are frequently asked


## Why was this list created?

When the paper investigating apple and google's data collection practices was popular on reddit, there did not seem to be a blocklist to easily add those non-consensual, while-idle tracking domains to a pihole filter. This is that easy list.

This project is mainly intended to provide the community of pihole users and blocklist creators with a place to collaborate and contribute their findings about these domains so that everyone can better understand their purpose and if they can easily be blocked.

It is not my intention to create or maintain a separate list or spend tons of time constantly testing domains in depth to see if they break anything. 

Forks and pull requests are absolutely welcome if you would like to contribute

## Why hasnt there been any updates to the list for X weeks/months/years?

See [Why was this list created?](#why-was-this-list-created)


## Why wont you add domains from [other large tech company]?

This list focusses fairly narrowly on domains from paper linked in the README since there did not seem to be an easy blocklist for those domains when the paper was making the rounds on reddit. 

The intention for this list is not for me to create an entirely independent blocklist to try and block all telemetry ever. Other lists (see list in the README) have already gotten there first and have done a way better job. I encourage maintainers of other lists to incorporate these domains into their own lists


## Why is the blocklist empty?
Blocking is currently split into three lists as outlined in the README. These lists are for:
- domains that are confirmed not to cause any issues with any other services (the main list)
- domains that have not been tested enough (beta list)
- domains that definitely or will very likely break something not related to idle telemetry (borked list)
 
This was done so that users could chose what tradeoffs they want to make on the privacy vs convenience scale by choosing to add more than one of the above lists to combine the domains on them. 

As this is mainly a curiosity project, I dont have time to test every domain in depth to see if it breaks anything, so for now most of the domains are in the "beta"/untested list until there is a reasonable amount of certainly that things won't break. If there's a domain that is likely not to break things and is collecting "unnecessary" telemetry such as nearby MAC addresses, then feel free to file an issue and I will consider adding it to the main list based on the evidence or a popular vote in favor of the domain.


## Why are there only a few domains in the list?

This list is likely not like other blocklists you are used to since it is hand curated for the specific purpose of making domains from the paper (linked in the README) available for inclusion in pihole lists and enabling community discussion. It takes time to organize all the domains, figure out what they are for, place them on the appropriate list, and test to make sure they dont break things.

## I know of a blocklist that people may be interested in, can I add it to the README?

Sure, feel free to submit a pull request and I will review it. However Keep in mind that the goal of this project is to contribute to the community effort of building good domain block lists, not to become another service for listing the best blocklists.



## How do I update these lists?

Details on how to update the lists are documented in the `UPDATING.md` file