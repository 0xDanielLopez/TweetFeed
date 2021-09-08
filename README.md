# TweetFeed
Collecting Indicators Of Compromise (IOCs) posted on Twitter in order to search them in your environment.

> #BlueTeam :large_blue_circle:

## Content

- [Data collected](#data-collected)
- [Some statistics](#some-statistics)
- [How it works](#how-it-works)
- [Hunting IOCs via Microsoft Defender](#hunting-IOCs-via-Microsoft-Defender)
- [Author](#author)
- [Disclaimer](#disclaimer)

## Data collected

<table>
    <thead>
        <tr>
		<th colspan=4><b>Feeds</b></th>
        </tr>
    </thead>
    <tbody>
	<tr>
		<th colspan=4>2021-09-08 01:50:34 (UTC)</th>
	</tr>
        <tr>
            <td>:clipboard: <a href="https://github.com/0xDanielLopez/TweetFeed/blob/master/today.csv">Today</a> (<a href="https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/today.csv">raw</a>)</td>
            <td>:clipboard: <a href="https://github.com/0xDanielLopez/TweetFeed/blob/master/week.csv">Week</a> (<a href="https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/week.csv">raw</a>)</td>
            <td>:clipboard: <a href="https://github.com/0xDanielLopez/TweetFeed/blob/master/month.csv">Month</a> (<a href="https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/month.csv">raw</a>)</td>
            <td>:clipboard: <a href="https://github.com/0xDanielLopez/TweetFeed/blob/master/year.csv">Year</a> (<a href="https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/year.csv">raw</a>)</td>
        </tr>
    </tbody>
</table>

#### Output example 

<table>
	<thead>
		<tr>
			<th><sub>Date (UTC)</sub></th>
			<th><sub>SourceUser</sub></th>
			<th><sub>Type</sub></th>
			<th><sub>Value</sub></th>
			<th><sub>Tags</sub></th>
			<th><sub>Tweet</sub></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><sub>2021-08-14 02:26:32</sub></td>
			<td><sub>phishunt_io</sub></td>
			<td><sub>url</sub></td>
			<td><sub>https://netflix.us2.cards/</sub></td>
			<td><sub>#phishing #scam</sub></td>
			<td><sub>https://twitter.com/phishunt_io/status/1426369619422502917</sub></td>
		</tr>
		<tr>
			<td><sub>2021-08-17 12:15:00</sub></td>
			<td><sub>TheDFIRReport</sub></td>
			<td><sub>ip</sub></td>
			<td><sub>185.56.76.94</sub></td>
			<td><sub>#Trickbot</sub></td>
			<td><sub>https://twitter.com/TheDFIRReport/status/1427604874053578756</sub></td>
		</tr>
	</tbody>
</table>

## Some statistics

#### IOCs

| IOC | Today | Week | Month | Year |
| :--- | :---: | :---: | :---: | :---: |
| **:link: URLs** | 47 | 1772 | 7810 | 7858 |
| **:globe_with_meridians: Domains** | 2 | 275 | 769 | 770 |
| **:triangular_flag_on_post: IPs** | 40 | 1258 | 4905 | 4931 |
| **:1234: SHA256** | 0 | 537 | 2182 | 2188 |
| **:1234: MD5** | 0 | 45 | 259 | 259 |

#### Tags

| Tag | Today | Week | Month | Year |
| :--- | :---: | :---: | :---: | :---: |
| **#phishing** | 83 | 2377 | 10345 | 10405 |
| **#scam** | 4 | 344 | 1107 | 1112 |
| **#malware** | 4 | 484 | 2459 | 2471 |
| **#ransomware** | 1 | 11 | 94 | 94 |
| **#banker** | 0 | 0 | 0 | 0 |
| **#AgentTesla** | 0 | 155 | 610 | 610 |
| **#Alienbot** | 0 | 15 | 72 | 72 |
| **#BazarLoader** | 0 | 19 | 40 | 40 |
| **#CobaltStrike** | 1 | 444 | 958 | 958 |
| **#Dridex** | 0 | 101 | 155 | 155 |
| **#FluBot** | 0 | 4 | 5 | 5 |
| **#Lokibot** | 0 | 24 | 109 | 109 |
| **#ProxyShell** | 0 | 7 | 36 | 36 |
| **#Trickbot** | 0 | 3 | 21 | 21 |
| **#Ursnif** | 0 | 14 | 57 | 57 |

#### Top reporters (today)

| Number | User | IOCs | 
| :--- | :---: | :---: | 
| **#1** | [romonlyht](https://twitter.com/romonlyht) | 50 |
| **#2** | [KesaGataMe0](https://twitter.com/KesaGataMe0) | 13 |
| **#3** | [secbird1](https://twitter.com/secbird1) | 11 |
| **#4** | [ecarlesi](https://twitter.com/ecarlesi) | 6 |
| **#5** | [pingineer_jp](https://twitter.com/pingineer_jp) | 2 |
| **#6** | [CardanoPhishing](https://twitter.com/CardanoPhishing) | 2 |
| **#7** | [MalwarePatrol](https://twitter.com/MalwarePatrol) | 1 |
| **#8** | [drb_ra](https://twitter.com/drb_ra) | 1 |
| **#9** | [harugasumi](https://twitter.com/harugasumi) | 1 |
| **#10** | [neonprimetime](https://twitter.com/neonprimetime) | 1 |

## How it works?
Search tweets that contain certain tags **or** that are posted by certain *infosec* people.

### Tags being searched
##### *(not case sensitive)*
```
- #phishing
- #scam
- #malware
- #ransomware
- #banker
- #AgentTesla
- #Alienbot
- #BazarLoader
- #CobaltStrike
- #Dridex
- #FluBot
- #Lokibot
- #ProxyShell
- #Trickbot
- #Ursnif
```


### Also search Tweets posted by
##### *(these are trusted folks that sometimes don't use tags)*
<big><pre>
[**TweetFeed list**](https://twitter.com/i/lists/1423693426437001224)
</pre></big>


### IOCs being collected
```
- URL
- Domain
- IP address
- SHA256 hash
- MD5 hash
```

## Hunting IOCs via Microsoft Defender

**1. Search `SHA256` hashes with `yearly` tweets feed**
```kusto
let MaxAge = ago(30d);
let SHA256_whitelist = pack_array(
'XXX' // Some SHA256 hash you want to whitelist.
);
let TweetFeed = materialize (
    (externaldata(report:string)
    [@"https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/year.csv"]
    with (format = "txt"))
    | extend report = parse_csv(report)
    | extend Type = tostring(report[2])
    | where Type == 'sha256'
    | extend SHA256 = tostring(report[3])
    | where SHA256 !in(SHA256_whitelist)
    | extend Tag = tostring(report[4])
    | extend Tweet = tostring(report[5])
    | project SHA256, Tag, Tweet 
);
union (
    TweetFeed
    | join (
        DeviceProcessEvents
        | where Timestamp > MaxAge
    ) on SHA256
), (
    TweetFeed
    | join (
        DeviceFileEvents
        | where Timestamp > MaxAge
    ) on SHA256
), ( 
    TweetFeed
    | join (
        DeviceImageLoadEvents
        | where Timestamp > MaxAge
    ) on SHA256
) | project Timestamp, DeviceName, FileName, FolderPath, SHA256, Tag, Tweet
```

<br>

**2. Search `IP addresses` with `monthly` tweets feed**
```kusto
let MaxAge = ago(30d);
let IPaddress_whitelist = pack_array(
'XXX' // Some IP address you want to whitelist.
);
let TweetFeed = materialize (
    (externaldata(report:string)
    [@"https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/month.csv"]
    with (format = "txt"))
    | extend report = parse_csv(report)
    | extend Type = tostring(report[2])
    | where Type == 'ip'
    | extend RemoteIP = tostring(report[3])
    | where RemoteIP !in(IPaddress_whitelist)
    | extend Tag = tostring(report[4])
    | extend Tweet = tostring(report[5])
    | project RemoteIP, Tag, Tweet 
);
union (
TweetFeed
    | join (
        DeviceNetworkEvents
    | where Timestamp > MaxAge
    ) on RemoteIP
) | project Timestamp, DeviceName, RemoteIP, Tag, Tweet
```

<br>

**3. Search `urls` and `domains` with `weekly` tweets feed**
```kusto
let MaxAge = ago(30d);
let domain_whitelist = pack_array(
'XXX', // Some URL/Domain you want to whitelist.
);
let TweetFeed = materialize (
    (externaldata(report:string)
    [@"https://raw.githubusercontent.com/0xDanielLopez/TweetFeed/master/week.csv"]
    with (format = "txt"))
    | extend report = parse_csv(report)
    | extend Type = tostring(report[2])
    | where Type in('url','domain')
    | extend RemoteUrl = tostring(report[3])
    | where RemoteUrl !in(domain_whitelist)
    | extend Tag = tostring(report[4])
    | extend Tweet = tostring(report[5])
    | project RemoteUrl, Tag, Tweet 
);
union (
TweetFeed
    | join (
        DeviceNetworkEvents
    | where Timestamp > MaxAge
    ) on RemoteUrl
) | project Timestamp, DeviceName, RemoteUrl, Tag, Tweet
```

## Author
* [**Daniel López**](https://twitter.com/0xDanielLopez)

<!--- ![Twitter](https://img.icons8.com/officexs/16/000000/twitter.png) --->

## Disclaimer

Please note that all the data is collected from Twitter and sorted/served here as it is on best effort.

I have tried to tune as much as possible the searches trying to collect only valuable info. However please consider making your own analysis before taking any action related to these IOCs.

Anyway feel free to reach me out regarding any False Positive or to provide any kind of feedback.

<hr>

By the Community for the Community