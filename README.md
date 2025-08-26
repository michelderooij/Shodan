The following are queries which can be used or serve as an example when filtering results on [url=https://shodan.io/]shodan.io[/url]

EXCHANGE            PROTOCOL  FILTER
ANY                 ANY       Microsoft Exchange:
ANY                 OWA       X-OWA-Version
2007                OWA       X-OWA-Version: "8."
2010                OWA       X-OWA-Version: "14."
2013                OWA       X-OWA-Version: "15.0."
2016                OWA       X-OWA-Version: "15.1."
2019                OWA       X-OWA-Version: "15.2." -"15.2.2562"
SE                  OWA       X-OWA-Version: "15.2.2562"

2013/2016/2019/SE   

IIS         OS             FILTER
6.0         WS2003         Server: "Microsoft-IIS/6.0"
7.0	        WS2008	       Server: "Microsoft-IIS/7.0"
7.5	        WS2008R2	     Server: "Microsoft-IIS/7.5"
8.0         WS2012         Server: "Microsoft-IIS/8.0"
8.5         WS2012R2       Server: "Microsoft-IIS/8.5"
10.0        WS2016-WS2025  Server: "Microsoft-IIS/10.0" X-AspNet-Version: "4.0.30319"
