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

Go to your Pi-hole Webinterface: `<pihole-ip>/admin`, log in and then go to settings and add the URL of the list you want:

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

## Links
- [Changelog](CHANGELOG.md)
- [Lists](lists/)

## How can I contribute to the list?

### Do you want to add or remove a domain?

Then create an issue using the domain request template under the following link: [https://github.com/Farin25/DNS-blocklists/issues](https://github.com/Farin25/DNS-blocklists/issues).


## License

[MIT](LICENSE)