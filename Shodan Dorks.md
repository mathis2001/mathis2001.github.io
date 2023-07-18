# Shodan dorks for Bug Bounty

A list of Shodan Dorks for Bug Bounty, Web Application Security, and Pentesting

<p>
Credits to TakSec: https://taksec.github.io/google-dorks-bug-bounty/
</p>

---

### TEST

> site:target.com test

### Default passwords

> ssl:target.com default password

> ssl:target.com guest login ok

> ssl:target.com "admin/1234"

> ssl:target.com Sharename Type Comment port:445

> ssl:target.com ftpd Anonymous user logged in

> ssl:target.com basic realm="default"

> ssl:target.com " Default name:admin password: 1234"

> ssl:target.com password required but none set

> target.com default password

> target.com guest login ok

> target.com "admin/1234"

> target.com Sharename Type Comment port:445

> target.com ftpd Anonymous user logged in

> target.com basic realm="default"

> target.com " Default name:admin password: 1234"

> target.com password required but none set

### Exposed services

> ssl:target.com port:23 gateway console

> ssl:target.com "root@" port:23 -login -password -name -Session

> ssl:target.com NO password required for telnet access. </br>

> ssl:target.com "220" "230 Login successful." port:21

> ssl:target.com x-jenkins 200

> ssl:target.com Jenkins Unrestricted Dashboard

> ssl:target.com "X-Jenkins" "Set-Cookie: JSESSIONID" http.title:Dashboard

> ssl:target.com port:2375 product:"docker"

> ssl:target.com "Docker-Distribution-Api-Version: registry" "200 OK" -gitlab

> ssl:target.com product:tomcat

> ssl:target.com proftpd port:21

> ssl:target.com openssh:port22

> ssl:target.com port:25 product:exim

> ssl:target.com remote desktop port:3389

> ssl:target.com "authentication disabled" "RFB 003.008"

> ssl:target.com "authentication disabled" port:5900,5901

> ssl:target.com "Authentication: disabled" port:445

> ssl:target.com 200 http.title:"dashboard"

> ssl:target.com "MongoDB Server Information { "metrics":"

> ssl:target.com "Set-Cookie: mongo-express=" "200 OK"

> ssl:target.com kibana content-legth:217

> ssl:target.com http.title:"DisallowedHost at /"

> target.com port:23 gateway console

> target.com "root@" port:23 -login -password -name -Session

> target.com NO password required for telnet access. </br>

> target.com "220" "230 Login successful." port:21

> target.com x-jenkins 200

> target.com Jenkins Unrestricted Dashboard

> target.com "X-Jenkins" "Set-Cookie: JSESSIONID" http.title:Dashboard

> target.com port:2375 product:"docker"

> target.com "Docker-Distribution-Api-Version: registry" "200 OK" -gitlab

> target.com product:tomcat

> target.com proftpd port:21

> target.com openssh:port22

> target.com port:25 product:exim

> target.com remote desktop port:3389

> target.com "authentication disabled" "RFB 003.008"

> target.com "authentication disabled" port:5900,5901

> target.com "Authentication: disabled" port:445

> target.com 200 http.title:"dashboard"

> target.com "MongoDB Server Information { "metrics":"

> target.com "Set-Cookie: mongo-express=" "200 OK"

> target.com kibana content-legth:217

> target.com http.title:"DisallowedHost at /"

> target.com "Set-Cookie: webvpn"

> target.com "webvpn%3D"

> target.com Server:+xxxxxxxx-xxxxx+-ssl:"fortinet"

> target.com ssl:"fortinet"

> target.com title:"SSL+VPN+Service"

> target.com Server:+xxxxxxxx-xxxxx+ssl:"fortinet"

> target.com http.html_hash:-1454941180

> target.com http.favicon.hash:945408572

> target.com http.html_hash:-628873716

### Information gathering / disclosure

> ssl:target.com http.title:"Index of /" http.html:".pem"

> ssl:target.com http.title:"Directory Listing"

> ssl:target.com http.html:"* The wp-config.php creation script uses this file"

> ssl:target.com http.title:"phpmyadmin"

> ssl:target.com http.html:"def_wirelesspassword"

> ssl:target.com http.title:"phpinfo()"

> ssl:target.com http.title:"Apache Status"

> ssl:target.com http.title:"Oracle Weblogic Server Administration Console"

> ssl:target.com http.title:"Swagger UI"

> ssl:target.com "X-Debug-Token-Link" port:443

> ssl:target.com "AkamaiGHost"

> ssl:target.com "GHost"

> ssl:target.com "Cloudflare","Cf","Cf-cache","CF-Connection_IP"

> ssl:target.com "Cloudfront"

> ssl:target.com "X-API-Version"

> ssl:target.com "X-Amz-Bucket-Region"

> target.com http.title:"Index of /" http.html:".pem"

> target.com http.title:"Directory Listing"

> target.com http.html:"* The wp-config.php creation script uses this file"

> target.com http.title:"phpmyadmin"

> target.com http.html:"def_wirelesspassword"

> target.com http.title:"phpinfo()"

> target.com http.title:"Apache Status"

> target.com http.title:"Oracle Weblogic Server Administration Console"

> target.com http.title:"Swagger UI"

> target.com "X-Debug-Token-Link" port:443

> target.com "AkamaiGHost"

> target.com "GHost"

> target.com "Cloudflare","Cf","Cf-cache","CF-Connection_IP"

> target.com "Cloudfront"

> target.com "X-API-Version"

> target.com "X-Amz-Bucket-Region"

> target.com http.favicon.hash:116323821

### Domain takeover

> ssl:target.com http.html:"The specified bucket does not exist"

> ssl:target.com http.html:"Trying to access your account?"

> ssl:target.com http.html:"With GetResponse Landing Pages, lead generation has never been easier"

> ssl:target.com http.html:"No settings were found for this company:"

> ssl:target.com http.html:"is not a registered InCloud YouTrack"

> ssl:target.com http.html:"No Site For Domain"

> ssl:target.com http.html:"It looks like you may have taken a wrong turn somewhere. Don't worry...it happens to all of us."

> ssl:target.com http.html:"This job board website is either expired or its domain name is invalid."

> ssl:target.com http.html:"Non-hub domain, The URL you've accessed does not provide a hub."

> ssl:target.com http.html:"Do you want to register *.wordpress.com?"

> ssl:target.com http.html:"Hello! Sorry, but the website you&rsquo;re looking for doesn&rsquo;t exist."

> ssl:target.com http.html:"There isn't a GitHub Pages site here."

> target.com http.html:"The specified bucket does not exist"

> target.com http.html:"Trying to access your account?"

> target.com http.html:"With GetResponse Landing Pages, lead generation has never been easier"

> target.com http.html:"No settings were found for this company:"

> target.com http.html:"is not a registered InCloud YouTrack"

> target.com http.html:"No Site For Domain"

> target.com http.html:"It looks like you may have taken a wrong turn somewhere. Don't worry...it happens to all of us."

> target.com http.html:"This job board website is either expired or its domain name is invalid."

> target.com http.html:"Non-hub domain, The URL you've accessed does not provide a hub."

> target.com http.html:"Do you want to register *.wordpress.com?"

> target.com http.html:"Hello! Sorry, but the website you&rsquo;re looking for doesn&rsquo;t exist."

> target.com http.html:"There isn't a GitHub Pages site here."
