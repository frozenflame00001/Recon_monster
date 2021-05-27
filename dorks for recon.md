## 🚦 Advance Recon Dorks ##
<img src="https://raw.githubusercontent.com/frozenflame00001/Recon_monster/main/assets/images%20(1).png">
💡 **This dork list provides dorks for differnt functionalities . Such as , file searching , hidden information collecting , vulnerability analysis and many more.**
<br><br>
<b>Note ::</b> Replace the <b>hackerone.com</b> with your desired domain. And you are ready to go.
<br><br>
🔍 Directory listing vulnerabilities|
------------------ | 
```
site:hackerone.com intitle:index.of
```

🔍 Exposed Configuration files|
------------------ | 
```
site:hackerone.com ext:xml | ext:conf | ext:cnf | ext:reg | ext:inf | ext:rdp | ext:cfg | ext:txt | ext:ora | ext:ini
```

🔍 Exposed Database files|
------------------ | 
```
site:hackerone.com ext:sql | ext:dbf | ext:mdb
```

🔍 Exposed log files|
------------------ | 
```
site:hackerone.com ext:log
```

🔍 Backup and old files|
------------------ | 
```
site:hackerone.com ext:bkf | ext:bkp | ext:bak | ext:old | ext:backup
```

🔍 Login pages|
------------------ | 
```
site:hackerone.com inurl:login
```

🔍 SQL errors|
------------------ | 
```
site:hackerone.com intext:"sql syntax near" | intext:"syntax error has occurred" | intext:"incorrect syntax near" | intext:"unexpected end of SQL command" | intext:"Warning: mysql_connect()" | intext:"Warning: mysql_query()" | intext:"Warning: pg_connect()"
```

🔍 Publicly exposed documents|
------------------ | 
```
site:hackerone.com ext:doc | ext:docx | ext:odt | ext:pdf | ext:rtf | ext:sxw | ext:psw | ext:ppt | ext:pptx | ext:pps | ext:csv
```

🔍 phpinfo()|
------------------ | 
```
site:hackerone.com ext:php intitle:phpinfo "published by the PHP Group"
```

🔍 Finding Backdoors|
------------------ | 
```
site:hackerone.com inurl:shell | inurl:backdoor | inurl:wso | inurl:cmd | shadow | passwd | boothackerone.comi | inurl:backdoor
```

🔍 Install / Setup files|
------------------ | 
```
site:hackerone.com inurl:readme | inurl:license | inurl:install | inurl:setup | inurl:config
```

🔍 Open Redirects|
------------------ | 
```
site:hackerone.com inurl:redir | inurl:url | inurl:redirect | inurl:return | inurl:src=http | inurl:r=http
```

🔍 Apache STRUTS RCE|
------------------ | 
```
site:hackerone.com ext:action | ext:struts | ext:do
```

🔍 Find Pastebin or, other bin entries|
------------------ | 
```
site:pastebin.com | site:throwbin.io | site:ghostbin.co hackerone.com
```

🔍 .htaccess sensitive files|
------------------ | 
```
site:hackerone.com inurl:"/phpinfo.php" | inurl:".htaccess" | inurl:"/.git" hackerone.com -github
```

🔍 Find Subdomains|
------------------ | 
```
site:*.hackerone.com
```

🔍 Find Sub-Subdomains|
------------------ | 
```
site:*.*.hackerone.com
```

🔍 Find WordPress|
------------------ | 
```
site:hackerone.com inurl:wp- | inurl:wp-content | inurl:plugins | inurl:uploads | inurl:themes | inurl:download
```

🔍 Find WordPress #2|
------------------ | 
```
site:hackerone.com inurl:wp-content | inurl:wp-includes
```

🔍 Find WordPress [Wayback Machine]|
------------------ | 
```
http://wwwb-dedup.us.archive.org:8083/cdx/search?url=hackerone.com/&matchType=domain&collapse=digest&output=text&fl=original,timestamp&filter=urlkey:.*wp[-].*&limit=1000000&xx=
```

🔍 Search in GITHUB|
------------------ | 
```
https://github.com/search?q="*.hackerone.com"&type=host
```

🔍 Search in OpenBugBounty|
------------------ | 
```
https://www.openbugbounty.org/search/?search=hackerone.com&type=host
```

🔍 Search in Reddit|
------------------ | 
```
https://www.reddit.com/search/?q=hackerone.com&source=recent
```

🔍 Test CrossDomain|
------------------ | 
```
http://hackerone.com/crossdomain.xml
```

🔍 Check in ThreatCrowd|
------------------ | 
```
https://threatcrowd.org/domain.php?domain=hackerone.com
```

🔍 Find .SWF file (Google)|
------------------ | 
```
inurl:hackerone.com ext:swf
```

🔍 Find .SWF file (Yandex)|
------------------ | 
```
https://yandex.com/search/touch/?text=site%3Ahackerone.com%20mime%3Aswf&lr=10530&redircnt=1619065165.1
```

🔍 Search SWF in WayBack Machine|
------------------ | 
```
https://web.archive.org/cdx/search?url=hackerone.com/&matchType=domain&collapse=urlkey&output=text&fl=original&filter=urlkey:.*swf&limit=100000&_=1507209148310
```

🔍 Search in WayBack Machine #2|
------------------ | 
```
https://web.archive.org/cdx/search?url=hackerone.com/&matchType=domain&collapse=urlkey&output=text&fl=original&filter=mimetype:application/x-shockwave-flash&limit=100000&_=1507209148310
```

🔍 Search in WayBack Machine #3|
------------------ | 
```
https://web.archive.org/web/*/hackerone.com/*
```

🔍 Search in WayBack Machine [List/All]|
------------------ | 
```
https://web.archive.org/web/*/hackerone.com/*
```

🔍 Check in crt.sh|
------------------ | 
```
https://crt.sh/?q=%25.hackerone.com
```

🔍 Check in CENSYS |
------------------ | 

IP-v4
```
https://censys.io/ipv4?q=hackerone.com
```
Domains
```
https://censys.io/domain?q=hackerone.com
```
Certs
```
https://censys.io/certificates?q=hackerone.com
```

🔍 Search in SHODAN|
------------------ | 
```
https://www.shodan.io/search?query=hackerone.com
```

🔍API end point WSDL|
------------------ |
```
site:hackerone.com filetype:wsdl | filetype:WSDL | ext:svc | inurl:wsdl | Filetype: ?wsdl | inurl:asmx?wsdl | inurl:jws?wsdl | intitle:_vti_bin/sites.asmx?wsdl | inurl:_vti_bin/sites.asmx?wsdl
```

🔍What CMS? |
----------------- |
```
https://whatcms.org/?s=hackerone.com
```

🔍3rd party exposure|
----------------- |
```
site:http://ideone.com | site:http://codebeautify.org | site:http://codeshare.io | site:http://codepen.io | site:http://repl.it | site:http://justpaste.it | site:http://pastebin.com | site:http://jsfiddle.net | site:http://trello.com | site:*.atlassian.net | site:bitbucket.org "hackerone.com"
```

