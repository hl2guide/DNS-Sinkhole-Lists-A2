
# DNS-Sinkhole-Lists-A2 [deprecated]

![Logo](https://images2.imgbox.com/f7/d1/eTBopT91_o.png)

## Important News 📰

### (as of April 7, 2020)

I've made the final decision to deprecate this repo since it isn't achieving my expected outcomes. No more commits will be made.

I advise that you consider making the switch (like I have) to using one of AdGuard's free products:
- AdGuard Home: https://github.com/AdguardTeam/AdGuardHome/wiki/Getting-Started#installation
- Browser Extension: https://adguard.com/en/adguard-browser-extension/overview.html
- AdGuard DNS (in Beta): https://adguard.com/en/adguard-dns/overview.html

## Description 📚

A collection of DNS Sinkhole lists for testing purposes.\
(not for use in production systems)

Lists are combined, cleaned, duplicates are removed and then are sorted alphabetically (nice and clean).

Each combined list consist of zones and domains in plaintext (not HOSTS text format) with one domain per line.

**These combined lists are not for use with the Windows HOSTS file**

A PowerShell script generates the lists and then commits to this repository about every 6 hours.

**It's too early for production usage therefore unless you're a tester please don't use it until it matures to version 1.0.**

There are four options:
 - combined (Australia and US users) **[my 1st recommendation]**
 - combined international (all other countries) **[my 2nd recommendation]**
 - combined (Australia and US users) - *Social Media Allowed*
 - combined international (all other countries) - *Social Media Allowed*

This **readme** created using https://stackedit.io

## How it Works ❓

The combined list contains:

1) a list of blocked TLDs (acts the basis)
2) a blacklist that contains blocked sites that are in trusted zones (e.g. .com)

Testers can test in these supported HOSTS/domain managers:

- DNS66 (Android, requires F-Droid app store)
- Technitium DNS Server (Windows or Linux)
- A PiHole device

Testers please use **only one** of the below raw text links.

## Combined List Files 🗃️

Pick one appropriate list from the below four:

| File Name | Description |
|--|--|
| [*COMBINED_LISTS_GENERATED/<br/>0_combined_blocklist.txt*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/COMBINED_LISTS_GENERATED/0_combined_blocklist.txt) | contains 'block_list', 'tld_blocklist'<br/>and 'tld_most_abused' and 'typosquatting_blocklist'<br/>*(users within North America or Australia)* |
| [*COMBINED_LISTS_GENERATED/<br/>0_combined_blocklist_international.txt*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/COMBINED_LISTS_GENERATED/0_combined_blocklist_international.txt) | ditto but for international users<br/>*(users who are outside of North America and Australia)* |
| [*COMBINED_LISTS_GENERATED/<br/>0_combined_blocklist <br/>(social media allowed).txt*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/COMBINED_LISTS_GENERATED/0_combined_blocklist%20%28social%20media%20allowed%29.txt) | contains 'block_list', 'tld_blocklist_international'<br/>and 'tld_most_abused' and 'typosquatting_blocklist'<br/>*(users within North America or Australia) - Social Media Allowed [not recommended]* |
| [*COMBINED_LISTS_GENERATED/<br/>0_combined_blocklist_international <br/>(social media allowed).txt*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/COMBINED_LISTS_GENERATED/0_combined_blocklist_international%20%28social%20media%20allowed%29.txt) | ditto but for international users<br/>*(for users outside of North America and Australia)  - Social Media Allowed [not recommended]* |

## Separated List Files 📂

For reference only.

| File Name | Description |
|--|--|
| [*allowed_zones.txt*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/allowed_zones.txt) | the *whitelist* of domains that are allowed |
| [*block_list.txt*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/block_list.txt)  | the **blacklist** for blocking base zones and then bad domains that fit into allowed zones (e.g. ending with .com) |
| [*tld_blocklist.txt*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/tld_blocklist.txt) | a list of **blocked TLDs** |
| [*tld_blocklist_international.txt*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/tld_blocklist_international.txt) | a list of **blocked TLDs** (international version) |
| [*tld_most_abused.txt*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/tld_most_abused.txt) | a list of the **most abused TLDs** |
| [*typosquatting_blocklist*](https://raw.githubusercontent.com/hl2guide/DNS-Sinkhole-Lists-A2/master/typosquatting_blocklist.txt) | a list of often mistyped domains for popular websites |

## Changelog 📜

### 26-11-2019 at 5PM AEST
- Extended testing phase out to at least March 2020

### 12-11-2019 at 5PM AEST
- Added more lists
- Cleaned up repo structure

### 05-10-2019 at 4PM AEST
- Added typosquatting domains for popular games to typosquatting list

### 23-09-2019 at 2AM AEST

- Rewrote the generator script to be modular and optimized
- Added typosquatting domains for frequently mistyped for the world's most popular websites
- Renamed blocklists for clarity and providing a table for options

### 27-08-2019 at 10PM AEST

- Added the world's most popular TLDs into the filter for included lists during generation

## Credits 😀

Credit and copyright belongs to the below list creators. Thanks for their tireless work :D

## Included Lists 🗂️

AdGuard Ad Domains\
Blocks ad serving domains.\
https://raw.githubusercontent.com/justdomains/blocklists/master/lists/adguarddns-justdomains.txt

AdHell List\
Blocks ad serving domains.\
https://getadhell.com/standard-package.txt

AnudeepND Blacklist\
Block ads, tracking and cryptomining domains.\
https://raw.githubusercontent.com/anudeepND/blacklist/master/adservers.txt

Blackbook List\
Blocks malicious domains.\
https://raw.githubusercontent.com/stamparm/blackbook/master/blackbook.txt

Blocklist Project - Crypto\
Blocks cryptomining domains.\
https://blocklist.site/app/dl/crypto

Blocklist Project - Drugs\
Blocks drug domains.\
https://blocklist.site/app/dl/drugs

Blocklist Project - Fake News\
Blocks fakenews domains.\
https://blocklist.site/app/dl/fakenews

Blocklist Project - Gambling\
Blocks gambling domains.\
https://blocklist.site/app/dl/gambling

Blocklist Project - Ransomware\
Blocks ransomware domains.\
https://blocklist.site/app/dl/ransomware

Blocklist Project - Scam\
Blocks scam domains.\
https://blocklist.site/app/dl/scam

Blocklist Project - Spam\
Blocks spam domains.\
https://blocklist.site/app/dl/spam

DeveloperDan Tracking List\
Blocks tracking domains.\
https://www.github.developerdan.com/hosts/lists/tracking-aggressive-extended.txt

DeveloperDan App Ads List\
Blocks ad domains.\
https://www.github.developerdan.com/hosts/lists/ads-and-tracking-extended.txt

Mobile App Ads Block List\
Blocks mobile app ad domains.\
https://raw.githubusercontent.com/evpne/socialblocklists/master/MobileAppsAds/appadsblocklist.txt

EasyList Ad Domains\
Blocks ad serving domains.\
https://raw.githubusercontent.com/justdomains/blocklists/master/lists/easylist-justdomains.txt

EasyPrivacy\
Blocks privacy invading domains.\
https://raw.githubusercontent.com/justdomains/blocklists/master/lists/easyprivacy-justdomains.txt

hemiipatu's Ads Domains\
Blocks ad domains.\
https://raw.githubusercontent.com/hemiipatu/Blocklists/master/advertisement.txt

hemiipatu's Phishing Domains\
Blocks phishing domains.\
https://raw.githubusercontent.com/hemiipatu/Blocklists/master/phishing.txt

hemiipatu's Ransomware Domains\
Blocks ransomware domains.\
https://raw.githubusercontent.com/hemiipatu/Blocklists/master/ransomware.txt

hemiipatu's Scam Domains\
Blocks scam domains.\
https://raw.githubusercontent.com/hemiipatu/Blocklists/master/scam.txt

hemiipatu's Spam Domains\
Blocks spam domains.\
https://raw.githubusercontent.com/hemiipatu/Blocklists/master/spam.txt

ios-trackers\
Blocks iOS trackers.\
https://raw.githubusercontent.com/jakejarvis/ios-trackers/master/blocklist.txt

ios-telemetry\
Blocks iOS telemetry.\
https://raw.githubusercontent.com/adversarialtools/ios-telemetry/master/blacklist

jwSpamSpy Spam Domains\
Blocks spam email domains.\
http://www.joewein.net/dl/bl/dom-bl.txt

Marcel Bischoff's Tracker Domains\
Blocks tracker domains.\
https://raw.githubusercontent.com/herrbischoff/trackers/master/trackers.txt

NoCoin\
Blocks coin miner domains.\
https://raw.githubusercontent.com/justdomains/blocklists/master/lists/nocoin-justdomains.txt

NoTracking Host Names List\
Blocks tracking domains.\
https://raw.githubusercontent.com/notracking/hosts-blocklists/master/hostnames.txt

NoTracking Domains List\
Blocks tracking domains.\
https://raw.githubusercontent.com/notracking/hosts-blocklists/master/domains.txt

NSABlocklist (pi-hole-edition)\
Blocks most known NSA / GCHQ / C.I.A. / F.B.I. spying servers.\
https://raw.githubusercontent.com/Cauchon/NSABlocklist-pi-hole-edition/master/HOSTS%20(excluding%20most%20GOV%20URLs)

Phishing Army Blocklist\
Blocks phishing domains.\
https://phishing.army/download/phishing_army_blocklist.txt

Shalla Malware Domains\
Blocks malware hosting domains.\
https://v.firebog.net/hosts/Shalla-mal.txt

Skype Ads Block List\
Blocks Skype ad domains.\
https://raw.githubusercontent.com/evpne/socialblocklists/master/Skype/skypeblocklist.txt

Smed79 Blacklist\
Blocks ads, tracking and mining domains.\
https://raw.githubusercontent.com/smed79/blacklist/master/hosts.txt

The Big List of Hacked Malware Web Sites\
Blocks malware, ransomware, viruses and trojan serving domains. \
https://raw.githubusercontent.com/mitchellkrogza/The-Big-List-of-Hacked-Malware-Web-Sites/master/hacked-domains.list

WindowsSpyBlocker 7\
Blocks Windows 7 telemetry domains.\
https://raw.githubusercontent.com/deathbybandaid/piholeparser/master/Subscribable-Lists/ParsedBlacklists/WindowsSpyBlocker7.txt

WindowsSpyBlocker 8.1\
Blocks Windows 8.1 telemetry domains.\
https://raw.githubusercontent.com/deathbybandaid/piholeparser/master/Subscribable-Lists/ParsedBlacklists/WindowsSpyBlocker81.txt

WindowsSpyBlocker\
Blocks Windows 10 telemetry domains.\
https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt

XionKzn Block List\
Blocks annoying ads, trackers and scam domains.\
https://raw.githubusercontent.com/XionKzn/PiHole-Lists/master/Blocklist.txt

Xlimit91 Block List\
Blocks annoying ads, trackers and scam domains.\
https://raw.githubusercontent.com/xlimit91/xlimit91-block-list/master/blacklist.txt

Blocklist.kowabit.de List\
Blocks ad serving domains.\
https://raw.githubusercontent.com/hectorm/hmirror/master/data/blocklist.kowabit.de/list.txt

Blockconvert List\
Malware, advert and tracking blacklist.\
https://raw.githubusercontent.com/mkb2091/blockconvert/master/blacklist.txt

Evil Domains List\
Blocks ad serving domains.\
https://raw.githubusercontent.com/hell-sh/Evil-Domains/master/evil-domains.txt

Vk496 List\
Blocks ad serving domains.\
https://raw.githubusercontent.com/vk496/hosts/master/hosts

abuse.ch URLhaus Malicious Hosts Blocklist\
Blocks malware domains.\
https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter-hosts.txt

Gift Card Killer\
Blocks Gift Card domains.\
https://raw.githubusercontent.com/TakoYachty/Gift-Card-Killer/master/giftcardkiller.txt

Joeylane Hosts List\
Blocks ad domains.\
https://raw.githubusercontent.com/joeylane/hosts/master/hosts

Magento Burner Domains\
Blocks burner domains.\
https://raw.githubusercontent.com/gwillem/magento-malware-scanner/master/rules/burner-domains.txt

PiHoleParser - Blocked Australian Domains\
\
https://raw.githubusercontent.com/deathbybandaid/piholeparser/master/Subscribable-Lists/CountryCodesLists/Australia.txt

PiHoleParser - Blocked British Domains\
\
https://raw.githubusercontent.com/deathbybandaid/piholeparser/master/Subscribable-Lists/CountryCodesLists/UnitedKingdom.txt

PiHoleParser - Blocked North American Domains\
\
https://raw.githubusercontent.com/deathbybandaid/piholeparser/master/Subscribable-Lists/CountryCodesLists/UnitedStatesofAmerica.txt

Pornaway Porn Ads Blocker\
Blocks ad domains.\
https://raw.githubusercontent.com/mhxion/pornaway/master/hosts/porn_ads.txt

PUA Maltrail List\
Blocks Possibly Unwanted Applications.\
https://raw.githubusercontent.com/stamparm/maltrail/master/trails/static/suspicious/pua.txt

R-a-y Ads List\
Blocks ad domains.\
https://raw.githubusercontent.com/r-a-y/mobile-hosts/master/AdguardMobileAds.txt

R-a-y Spyware List\
Blocks spyware domains.\
https://raw.githubusercontent.com/r-a-y/mobile-hosts/master/AdguardMobileSpyware.txt

SNAFU Block List\
Blocks ad domains.\
https://raw.githubusercontent.com/RooneyMcNibNug/pihole-stuff/master/SNAFU.txt

Soteria-Nou Domain-List Ads\
Blocks ad domains.\
https://raw.githubusercontent.com/soteria-nou/domain-list/master/ads.txt

Soteria-Nou Domain-List Affiliates\
Blocks unwanted affiliates.\
https://raw.githubusercontent.com/soteria-nou/domain-list/master/affiliate.txt

Soteria-Nou Domain-List Analytics\
Blocks analytics tracking.\
https://raw.githubusercontent.com/soteria-nou/domain-list/master/analytics.txt

Soteria-Nou Domain-List Blocked Widgets\
Blocks unwanted website widgets.\
https://raw.githubusercontent.com/soteria-nou/domain-list/master/widgets.txt

Soteria-Nou Domain-List Enrichments\
Blocks some enrichments.\
https://raw.githubusercontent.com/soteria-nou/domain-list/master/enrichments.txt

Soteria-Nou Domain-List Fake Sites\
Blocks fake sites.\
https://raw.githubusercontent.com/soteria-nou/domain-list/master/fake.txt

Yahoo Ad Servers\
Blocks some ads on Yahoo.\
https://raw.githubusercontent.com/XionKzn/PiHole-Lists/master/Yahoo_Ad_Servers.txt
