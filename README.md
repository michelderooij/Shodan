The following are queries that can be used or serve as an example when filtering results on [Shodan](https://shodan.io/)

# Exchange

| EXCHANGE          | PROTOCOL       | FILTER                                                            |
| ----------------- | -------------- | ----------------------------------------------------------------- |
| ANY               | ANY            | Microsoft Exchange:                                               |
| ANY               | OWA            | "X-OWA-Version" -http.status:302                                  |  
| 2007              | OWA            | "X-OWA-Version:8." -http.status:302                               |
| 2010              | OWA            | "X-OWA-Version:14." -http.status:302                              |
| 2013              | OWA            | "X-OWA-Version:15.0." -http.status:302                            |
| 2016              | OWA            | "X-OWA-Version:15.1." -http.status:302                            |
| 2019              | OWA            | "X-OWA-Version:15.2." -"X-OWA-Version:15.2.2562" -http.status:302 |
| SE                | OWA            | "X-OWA-Version:15.2.2562"                                         |
| ANY               | IMAP4          | product:exchange port:143,993                                     |
| ANY               | POP3           | product:exchange port:110,995                                     |
| ANY               | Autodiscover   | hostname:autodiscover X-OWA-Version:                              |
| ANY               | HTTP + TLSv1.3 | Microsoft Exchange: ssl.version:tlsv1.3 HTTP                      |
| ANY               | SMTP           | Product:Exchange port:25,465,587                                  |
| 2003              | ANY            | "Exchange 2003"                                                   |
| 2000              | ANY            | "Exchange 2000"                                                   |
| 5.5               | ANY            | "Exchange 5.5"                                                    |

# IIS / OS

| IIS         | OS             | FILTER                                                     |
| ----------- | -------------- | ---------------------------------------------------------- |
| 6.0         | WS2003         | Server: "Microsoft-IIS/6.0"                                |
| 7.0	        | WS2008	       | Server: "Microsoft-IIS/7.0"                                |
| 7.5	        | WS2008R2	     | Server: "Microsoft-IIS/7.5"                                |
| 8.0         | WS2012         | Server: "Microsoft-IIS/8.0"                                |
| 8.5         | WS2012R2       | Server: "Microsoft-IIS/8.5"                                |
| 10.0        | WS2016-WS2025  | Server: "Microsoft-IIS/10.0"|

