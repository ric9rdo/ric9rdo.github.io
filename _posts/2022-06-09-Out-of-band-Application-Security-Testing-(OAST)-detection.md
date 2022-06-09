---
layout: article
title: Out-of-band Application Security Testing (OAST) detection
mathjax: true
---

Detection rule for Out-of-band application security testing (OAST), often used by pentesters to detect vulnerabilities. If someone uses such tool/technique, we will get an incident in Sentinel.

 

- Out-of-band application security testing (OAST) uses external servers to see otherwise invisible vulnerabilities. It was introduced to further improve the DAST (dynamic application security testing) model. 

- OAST operates dynamically, sending payloads to a running application. These payloads pass through the application’s processing in the normal way. If a payload is ever handled in an unsafe manner, it effectively performs some in-place instrumentation to change the application’s behavior, causing it to make a network interaction (typically DNS) with an external system. The contents of that interaction allow the OAST tool to report the precise type of vulnerability and the input point that can be used to trigger it. 

- OAST uses standard external domains to share the organization’s information. These external domains are configured to explore vulnerabilities in the corporate environment. 

If these external domains are observed in logs, we should reach the machine owner to understand whether is a legitimate business risk assessment or can be a reconnaissance activity to explore vulnerabilities: interact.sh, oast.pro, oast.live, oast.site, oast.online, oast.fun, oast.me, burpcollaborator.net, oastify.com, canarytokens.com, requestbin.net, dnslog.cn. 

 


### Sentinel Query

```

DnsEvents
| where Name has '.interact.sh' or Name has '.oast.pro' or Name has '.oast.live' or Name has '.oast.site' or Name has '.oast.online' or Name has '.oast.fun' or Name has '.oast.me' or Name has '.burpcollaborator.net' or Name has '.oastify.com' or Name has '.canarytokens.com' or Name has '.requestbin.net' or Name has '.dnslog.cn'
| distinct Name, Computer

```

<>

### If you want to know more on this, check: 
https://youtu.be/hLAuacX3CbQ

https://portswigger.net/blog/oast-out-of-band-application-security-testing,  

https://portswigger.net/burp/application-security-testing/oast,   

https://omercitak.com/out-of-band-attacks-en/