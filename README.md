<div align="center">
  <h1 align="center">TweetFeed</h1>

  <p align="center">
    Feeds of IOCs posted on Twitter
    <br />
    <br />
    <strong>Web version at <a href="https://tweetfeed.live/">TweetFeed.live</a></strong>
  </p>

  ![TweetFeed.live](https://raw.githubusercontent.com/TweetFeed/TweetFeed.github.io/main/img/TweetFeed_live.PNG)
</div>

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
		<th colspan=4>2022-07-31 01:45:44 (UTC)</th>
	</tr>
    <tr>
            <th>Today</th>
            <th>Last 7 days</th>
            <th>Last 30 days</th>
            <th>Last 365 days</th>
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
| **:link: URLs** | 15 | 2227 | 12571 | 138086 |
| **:globe_with_meridians: Domains** | 0 | 1173 | 3452 | 22452 |
| **:triangular_flag_on_post: IPs** | 8 | 738 | 4046 | 65573 |
| **:1234: SHA256** | 1 | 130 | 479 | 36987 |
| **:1234: MD5** | 0 | 48 | 273 | 2723 |

#### Tags

| Tag | Today | Week | Month | Year |
| :--- | :---: | :---: | :---: | :---: |
| **#phishing** | 19 | 3490 | 16760 | 171955 |
| **#scam** | 2 | 1174 | 4295 | 23578 |
| **#malware** | 1 | 147 | 783 | 22168 |
| **#maldoc** | 0 | 7 | 31 | 165 |
| **#ransomware** | 0 | 6 | 50 | 648 |
| **#banker** | 0 | 0 | 0 | 45 |
| **#AgentTesla** | 0 | 16 | 32 | 5408 |
| **#Alienbot** | 0 | 0 | 0 | 85 |
| **#BazarLoader** | 0 | 0 | 0 | 310 |
| **#CobaltStrike** | 0 | 281 | 1410 | 23394 |
| **#Dridex** | 0 | 0 | 0 | 5471 |
| **#Emotet** | 0 | 0 | 73 | 1613 |
| **#FluBot** | 0 | 0 | 0 | 30 |
| **#Follina** | 0 | 5 | 22 | 121 |
| **#Formbook** | 0 | 2 | 4 | 4850 |
| **#GootLoader** | 0 | 0 | 1 | 820 |
| **#GuLoader** | 0 | 10 | 17 | 386 |
| **#Hancitor** | 0 | 0 | 0 | 156 |
| **#IcedID** | 0 | 13 | 44 | 354 |
| **#Lazarus** | 0 | 3 | 4 | 108 |
| **#Lokibot** | 0 | 12 | 43 | 1548 |
| **#log4j** | 0 | 2 | 3 | 247 |
| **#Log4shell** | 0 | 1 | 1 | 231 |
| **#ProxyShell** | 0 | 0 | 0 | 111 |
| **#Qakbot** | 0 | 0 | 7 | 382 |
| **#Raccoon** | 0 | 0 | 2 | 1518 |
| **#RedLine** | 0 | 4 | 18 | 4137 |
| **#Remcos** | 0 | 0 | 2 | 993 |
| **#Spring4Shell** | 0 | 0 | 0 | 26 |
| **#SquirrelWaffle** | 0 | 0 | 0 | 53 |
| **#Trickbot** | 0 | 0 | 0 | 155 |
| **#Ursnif** | 0 | 0 | 21 | 437 |

#### Top reporters (today)

| Number | User | IOCs | 
| :--- | :---: | :---: | 
| **#1** | [ecarlesi](https://twitter.com/ecarlesi) | 12 |
| **#2** | [RdpSnitch](https://twitter.com/RdpSnitch) | 4 |
| **#3** | [harugasumi](https://twitter.com/harugasumi) | 2 |
| **#4** | [AP_Zenmashi](https://twitter.com/AP_Zenmashi) | 2 |
| **#5** | [phishunt_io](https://twitter.com/phishunt_io) | 2 |
| **#6** | [micham](https://twitter.com/micham) | 1 |
| **#7** | [HeliosCert](https://twitter.com/HeliosCert) | 1 |
| **#8** | [-](https://twitter.com/-) | 0 |
| **#9** | [-](https://twitter.com/-) | 0 |
| **#10** | [-](https://twitter.com/-) | 0 |

## How it works?
Search tweets that contain certain tags **or** that are posted by certain *infosec* people.

### Tags being searched
##### *(not case sensitive)*
```
- #phishing
- #scam
- #malware
- #maldoc
- #ransomware
- #banker
- #AgentTesla
- #Alienbot
- #BazarLoader
- #CobaltStrike
- #Dridex
- #Emotet
- #FluBot
- #Follina
- #Formbook
- #GootLoader
- #GuLoader
- #Hancitor
- #IcedID
- #Lazarus
- #Lokibot
- #log4j
- #Log4shell
- #ProxyShell
- #Qakbot
- #Raccoon
- #RedLine
- #Remcos
- #Spring4Shell
- #SquirrelWaffle
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
    | where not(ipv4_is_private(RemoteIP))
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
'XXX' // Some URL/Domain you want to whitelist.
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
