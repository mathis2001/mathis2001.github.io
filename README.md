# Google Dorks for Bug Bounty

A list of Google Dorks for Bug Bounty, Web Application Security, and Pentesting

<p>
Credits to TakSec: https://taksec.github.io/google-dorks-bug-bounty/
</p>

---

### Broad domain search w/ negative search

> site:target.com -www -shop -share -ir -mfa

### Find subdomains

> site:*.target.com

### PHP extension w/ parameters

> site:target.com ext:php inurl:?

### Disclosed XSS and Open Redirects

> site:openbugbounty.org inurl:reports intext:"target.com"

### Juicy Extensions

> site:"target[.]com" ext:log | ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:bak | ext:backup | ext:swp | ext:old | ext:~ | ext:git | ext:svn | ext:htpasswd | ext:htaccess

### Code Leaks

> site:pastebin.com "target.com"

> site:jsfiddle.net "target.com"

> site:codebeautify.org "target.com"

> site:codepen.io "target.com"

### Cloud Storage

> site:s3.amazonaws.com "target.com"

> site:blob.core.windows.net "target.com"

> site:googleapis.com "target.com"

> site:drive.google.com "target.com"

> site:dev.azure.com "target[.]com"

> site:onedrive.live.com "target[.]com"

> site:digitaloceanspaces.com "target[.]com"

> site:sharepoint.com "target[.]com"

> site:s3-external-1.amazonaws.com "target[.]com"

> site:s3.dualstack.us-east-1.amazonaws.com "target[.]com"

> site:dropbox.com/s "target[.]com"

> site:box.com/s "target[.]com"

> site:docs.google.com inurl:"/d/" "target[.]com"

### XSS prone parameters

> inurl:q= | inurl:s= | inurl:search= | inurl:query= inurl:& site:target.com

### Open Redirect prone parameters

> inurl:url= | inurl:return= | inurl:next= | inurl:redir= inurl:http site:target.com

### SQLi Prone Parameters

> inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:target.com

### SSRF Prone Parameters

> inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain=  | inurl:page= inurl:& site:target.com

### LFI Prone Parameters

> inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:target.com

### RCE Prone Parameters

> inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read=  | inurl:ping= inurl:& site:target.com

### High % inurl keywords

> inurl:config | inurl:env | inurl:setting | inurl:backup | inurl:admin | inurl:php site:target[.]com

### Sensitive Parameters

> inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:target[.]com

### JFrog Artifactory

> site:jfrog.io "target[.]com"

### Firebase

> site:firebaseio.com "target[.]com"

### API Docs

> inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"target[.]com"

### File upload endpoints

> site:target.com ”choose file”

## Dorks that work better w/o domain

### Bug Bounty programs and Vulnerability Disclosure Programs

> "submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"

> site:*/security.txt "bounty"

### Apache Server Status Exposed

> site:*/server-status apache

### WordPress

> inurl:/wp-admin/admin-ajax.php

### Drupal

> intext:"Powered by" & intext:Drupal & inurl:user

### Joomla

> site:*/joomla/login


---

Medium articles for more dorks:

https://thegrayarea.tech/5-google-dorks-every-hacker-needs-to-know-fed21022a906

https://infosecwriteups.com/uncover-hidden-gems-in-the-cloud-with-google-dorks-8621e56a329d

https://infosecwriteups.com/10-google-dorks-for-sensitive-data-9454b09edc12

Top Parameters:

https://github.com/lutfumertceylan/top25-parameter

Proviesec dorks:

https://github.com/Proviesec/google-dorks
