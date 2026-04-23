# DNS-blocklists
Public DNS blocklists focused on privacy, ads, trackers and Scam, Phishing. Maintained for Pi-hole, AdGuard Home, and other DNS filtering systems.



## Lists
 
| File | Description | URL |
|------|-------------|-----|
| `lists/tracker.txt` | Tracking domains (analytics, telemetry, fingerprinting and Advertisement) | https://raw.githubusercontent.com/Farin25/DNS-blocklists/main/lists/tracker.txt |
| `lists/scam.txt` | Scam and phishing domains | https://raw.githubusercontent.com/Farin25/DNS-blocklists/main/lists/scam.txt |
| `lists/combined.txt` | Tracker and Scam list combined|https://raw.githubusercontent.com/Farin25/DNS-blocklists/main/lists/combined.txt |
---

## Usage

### Pi-hole

Go to your Pi-hole Webinterface: `<pihole-ip>/admin`, log in and then go to **List and add the URL of the list you want:**

for Trackers and Advertisement:
```
https://raw.githubusercontent.com/Farin25/DNS-blocklists/main/lists/tracker.txt
```

for Scam and Phishing:
```
https://raw.githubusercontent.com/Farin25/DNS-blocklists/main/lists/scam.txt
```

for all combined:
```
https://raw.githubusercontent.com/Farin25/DNS-blocklists/main/lists/combined.txt
```

Then run Update Gravity List under **Tools -> Update Gravity**.

<details>
<summary> 
 
#### Optional: RegEx filter (Recommended)</summary>

Set up the RegEx filter in Pi-hole under **Domains → RegEx filter**.

> [!IMPORTANT]  
> RegEx filters are very strict and may break legitimate services. Add them one by one and test after each.

**General tracking** Blocks domains used to track your behavior across websites:
```
(^|\.)tracking\.
```

**Google advertising** Blocks Google's ad delivery and bidding network:
```
(^|\.)doubleclick\.net$
```
```
(^|\.)googlesyndication\.com$
```

**YouTube ads** Blocks the SDK that loads ads before and during YouTube videos:
```
(^|\.)imasdk\.googleapis\.com$
```

**Amazon advertising** Blocks Amazon's ad network and conversion tracking:
```
(^|\.)amazon-adsystem\.com$
```
```
(^|\.)aax-eu\.amazon-adsystem\.com$
```
```
(^|\.)fls\.amazon\.de$
```

**Prime Video analytics** Blocks viewership tracking on Prime Video:
```
(^|\.)smetrics\.primevideo\.com$
```

**Oracle Moat** Blocks ad measurement and viewability tracking used by large publishers:
```
(^|\.)moatads\.com$
```

**Conviva** Blocks video streaming analytics that track what you watch and for how long:
```
(^|\.)conviva\.com$
```

**Comscore** Blocks audience measurement tracking used by news sites and broadcasters:
```
(^|\.)scorecardresearch\.com$
```

**Joyn** Blocks ad and tracking infrastructure for the German streaming platform ProSiebenSat.1:
```
(^|\.)joyn\.de\.edgekey\.net$
```

</details>

## Links
- [Changelog](CHANGELOG.md)
- [Lists](lists/)

### Support, help and feedback
- [Discord](https://discord.gg/b2yDdCt5W)
- [Stoat](https://stt.gg/H4sHjKg0) 
- [Issue](https://github.com/Farin25/DNS-blocklists/issues)

## How can I contribute to the list?

### Do you want to add or remove a domain?

Then create an issue using the domain request template under the following link: [https://github.com/Farin25/DNS-blocklists/issues](https://github.com/Farin25/DNS-blocklists/issues).


## License

[MIT](LICENSE)