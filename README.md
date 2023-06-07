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

### Find exposed FTP services

> site:target.com intitle:"index of" inurl:ftp

> site:target.com filetype:url +inurl:"ftp://" +inurl:";@"

> site:target.com intitle:"FTP root at"

> site:target.com inurl:FTP "ftp root at"

> site:target.com name size "Last modified" inurl:ftp

> site:target.com "Parent Directory" "Last modified" ftp

### Find exposed documents

> site:"target[.]com" ext:doc | ext:docx | ext:odt | ext:pdf | ext:rtf | ext:sxw | ext:psw | ext:ppt | ext:pptx | ext:pps | ext:csv

### Find exposed git files

> site:target.com "index of" inurl:.git

> site:target.com "intitle:"index of" .git/hooks/

> site:target.com filetype:git | ext:git

### Directory listings

> site:target.com intext:"index of /"

> site:target.com intitle:"index of" "docker-compose.yml"

> site:target.com intitle:"index of"|"access_token.json"

> site:target.com intitle:"index of" "config.json"

> site:target.com intitle:"index of" "service-Account-Credentials.json" | "creds.json"

> site:target.com intitle:"index of" "db.json"

> site:target.com intitle:"index of" "credentials.json"

> site:target.com intitle:"index of" "awsconfig.json"

> site:target.com intext:"index of" /etc/passwd

> site:target.com intext:"index of" /etc/shadow

> site:target.com "index of" id_rsa

> site:target.com "index of" private.key

> site:target.com "index of" inurl:.git

> site:target.com "intitle:"index of" .git/hooks/

### PHP extension w/ parameters

> site:target.com ext:php inurl:?

### Disclosed XSS and Open Redirects

> site:openbugbounty.org inurl:reports intext:"target.com"

### Juicy Extensions

> site:"target[.]com" ext:log | ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:bak | ext:backup | ext:swp | ext:old | ext:~ | ext:git | ext:svn | ext:htpasswd | ext:htaccess

### Code Leaks / External websites leaks

> site:pastebin.com "target.com"

> site:jsfiddle.net "target.com"

> site:codebeautify.org "target.com"

> site:codepen.io "target.com"

> site:scribd.com "target.com"

> site:npmjs.com "target.com"

> site:npm.runkit.com "target.com"

> site:libraries.co "target.com"

> site:ycombinator.com "target.com"

> site:coggle.it "target.com"

> site:papaly.com "target.com"

> site:trello.com "target.com"

> site:prezi.com "target.com"

> site:jsdelivr.net "target.com"

> site:codeshare.io "target.com"

> site:sharecode.io "target.com"

> site:repl.it "target.com"

> site:gitter.im "target.com"

> site:bitbucket.org "target.com"

> site:zoom.us "target.com"

> site:atlassian.com "target.com"

> inurl:gitlab "target.com"

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

> inurl:"url=" | inurl:"return=" | inurl:"next=" | inurl:"redir=" | inurl:"http" | inurl:"%3Dhttp" | inurl:"%3D%2F" | inurl:"redirect"= | inurl:"redirecturl=" | inurl:"redirect_url=" | inurl:"returnurl=" | inurl:"relaystate=" | inurl:"forward=" | inurl:"forwardurl=" | inurl:"forward_url=" | inurl:"uri=" | inurl:"dest=" | inurl:"destination=" site:target.com

### SQLi Prone Parameters

> inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:target.com

### SSRF Prone Parameters

> inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain=  | inurl:page= inurl:& site:target.com

### LFI Prone Parameters

> inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:target.com

### RCE Prone Parameters

> inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read=  | inurl:ping= inurl:& site:target.com

### SQL errors

> site:target.com intext:"sql syntax near" | intext:"syntax error has occurred" | intext:"incorrect syntax near" | intext:"unexpected end of SQL command" | intext:"Warning: mysql_connect()" | intext:"Warning: mysql_query()" | intext:"Warning: pg_connect()"

### Configuration files

> inurl:config | inurl:env | inurl:setting | inurl:backup | ext:xml | ext:conf | ext:cnf | ext:reg | ext:inf | ext:rdp | ext:cfg | ext:txt | ext:ora | ext:ini site:target.com

> site:target.com intitle:"index of" inurl:app.conf

> site:target.com intitle:"index of" inurl:conf

> site:target.com filetype:conf

> site:target.com configuration filetype:txt

> site:target.com inurl:config.inc

> site:target.com password host inurl:config filetype:txt

> site:target.com inurl:config password host

> site:target.com filetype:conf

> site:target.com inurl:conf.xml

> site:target.com inurl:conf.js

> site:target.com inurl:conf.json

> site:target.com inurl:configuration.json

> site:target.com inurl:configuration.js

> site:target.com inurl:configuration.xml

> site:target.com inurl:config secret host

> site:target.com inurl:secret filetype:yaml

> site:target.com inurl:conf filetype:xml

> site:target.com inurl:Makefile.toml

> site:target.com inurl:Makefile 

### Sensitive Parameters

> inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:target[.]com

### JFrog Artifactory

> site:jfrog.io "target[.]com"

### Firebase

> site:firebaseio.com "target[.]com"

### API Docs

> inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"target[.]com"

> site:target.com inurl:/swagger-ui.html

> site:target.com inurl:/api/swagger

> site:target.com inurl:/api/v1/docs | inurl:/api/v2/docs | inurl:/api/v3/docs

> site:target.com inurl:/api/apidocs

### File upload endpoints

> site:target.com ”choose file”

### Dependency confusion (packages files)

> site:*target.com inurl:/ui/package.json

> site:*target.com inurl:/ui/package-lock.json

> site:*target.com inurl:/package.json

### Cached versions

> cache:target.com

### Linked websites

> link:target.com

### Find employees

> site:linkedin.com "target[.]com"

### Bug Bounty programs and Vulnerability Disclosure Programs

> "submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"

> site:*/security.txt "bounty"

### Apache

> site:target.com inurl:server-status apache

> site:target.com filetype:log intext:org.apache.hadoop.hdfs

> site:target.com intext:"This is Apache Hadoop release" "Local Logs"

> site:target.com intitle:"Apache HTTP Server" intitle:"documentation"

> site:target.com intitle:"Apache Status" "Apache Server Status for"

> site:target.com intitle:"Apache Status" | intext:"Apache Server Status"

> site:target.com intitle:"Apache Tomcat"

> site:target.com intitle:"Apache2 Debian Default Page: It works"  

> site:target.com intitle:"Apache::Status" (inurl:server-status | inurl:status.html | inurl:apache.html)

> site:target.com intitle:"Object not found" netware "apache 1.."

> site:target.com intitle:"Object not found!" intext:"Apache/2.0.* (Linux/SuSE)"

> site:target.com intext:Apache/2.2.29 (Unix) mod_ssl/2.2.29 | intitle:"Index of /"

> site:target.com "seeing this instead" intitle:"test page for apache"

> site:target.com intitle:"Test Page for Apache" "It Worked!"

### Nginx

> site:target.com intitle:"index of" "nginx.log"

> site:target.com intitle:"index of" "nginx"

> site:target.com intitle:Test Page for the Nginx HTTP Server on Fedora

> site:target.com intitle:\"Welcome to nginx!\" intext:\"Welcome to nginx on Debian!\" intext:\"Thank you for\"

> site:target.com intitle: "Welcome to nginx!" + "Thank you for using nginx."

> site:target.com inurl:nginx_status

> site:target.com inurl:nginx.conf nginx site:github.com

### PhpMyAdmin

> site:target.com " phpMyAdmin MySQL-Dump" "INSERT INTO" -"the"

> site:target.com " phpMyAdmin MySQL-Dump" filetype:txt

> site:target.com "# phpMyAdmin MySQL-Dump" "INSERT INTO" -"the"

> site:target.com "# phpMyAdmin MySQL-Dump" filetype:txt

> site:target.com "Index of" inurl:phpmyadmin

> site:target.com "Welcome to phpMyAdmin" " Create new database"

> site:target.com "Welcome to phpMyAdmin" + "Username:" + "Password:" + "Language:" + "Afrikaans"

> site:target.com "Welcome to phpMyAdmin" AND " Create new database"

> site:target.com "phpMyAdmin MySQL-Dump" "INSERT INTO" -"the"

> site:target.com "phpMyAdmin MySQL-Dump" filetype:txt

> site:target.com "phpMyAdmin" "running on" inurl:"main.php"

> site:target.com ext:sql intext:"-- phpMyAdmin SQL Dump" -site:github.*

> site:target.com filetype:sql "phpmyAdmin SQL Dump" (pass|password|passwd|pwd)

> site:target.com filetype:sql intext:wp_users phpmyadmin

> site:target.com intext:"phpMyAdmin MySQL-Dump" "INSERT INTO" -"the"

> site:target.com intext:"phpMyAdmin MySQL-Dump" filetype:txt

> site:target.com intext:"phpMyAdmin" "running on" inurl:"main.php"

> site:target.com intitle:"Index of" phpmyadmin

> site:target.com intitle:"index of /phpmyadmin" modified

> site:target.com intitle:phpMyAdmin

> site:target.com intitle:phpMyAdmin "Welcome to phpMyAdmin *" "running on as root@"

> site:target.com intitle:phpMyAdmin "Welcome to phpMyAdmin ***" "running on * as root@*"

> site:target.com inurl:"/phpmyadmin/user_password.php

> site:target.com inurl:"/phpmyadmin/user_password.php" -inurl:git

> site:target.com inurl:"phpmyadmin/index.php" intext:"[ Edit ] [ Create PHP Code ] [ Refresh ]"

> site:target.com inurl:.php? intext:CHARACTER_SETS,COLLATIONS, ?intitle:phpmyadmin

> site:target.com inurl:/phpMyAdmin/setup/index.php?phpMyAdmin=

> site:target.com inurl:/phpmyadmin/changelog.php -github -gitlab

> site:target.com inurl:/phpmyadmin/index.php?db=

> site:target.com inurl:\"/phpmyadmin/user_password.php

> site:target.com inurl:main.php Welcome to phpMyAdmin

> site:target.com inurl:main.php phpMyAdmin

> site:target.com inurl:phpmyadmin/index.php & (intext:username & password & "Welcome to")

> site:target.com inurl:phpmyadmin/themes intext:"pmahomme"

> site:target.com phpMyAdmin SQL Dump

> site:target.com phpMyAdmin dumps

> site:target.com inurl:phpldapadmin/

> site:target.com inutl:pma/

> site:target.com inurl:phppgadmin/

> site:target.com you really should fix this security hole by setting a password for user '.root'. inurl:/phpmyadmin intitle:localhost

### Grafana

> site:target.com intitle:"grafana" inurl:"/grafana/login" "Forgot your password"

> site:target.com intitle:"Grafana - Home" inurl:/orgid

> site:target.com inurl:login "Welcome to Grafana"

> site:target.com "Welcome to Grafana" inurl:/orgid

> site:target.com intitle:"Welcome to Grafana"

### WordPress

> site:target.com inurl:/wp-admin/admin-ajax.php

> site:target.com intext:"Index" inurl:"wp-" -wordpress.org -stackexchange -github

> site:target.com inurl:"/wp-json/wp/v2/users/" "id":1,"name":" -wordpress.stackexchange.com -stackoverflow.com

> site:target.com inurl:"/wp-content/uploads"

> site:target.com inurl:"wp-register.php" -wordpress.com -wordpress.org -github

> site:target.com intitle:"index of" "wp-config.php.bak"

> site:target.com "is proudly powered by WordPress"

> site:target.com "plugins/wp-db-backup/wp-db-backup.php"

> site:target.com filetype:txt inurl:wp-config.txt

> site:target.com intext:"the WordPress" inurl:wp-config ext:txt

> site:target.com inurl:"/wp-content/plugins/wp-mobile-detector/" ext:php

> site:target.com inurl:"/wp-content/wpclone-temp/wpclone_backup/"

> site:target.com inurl:"/wp-login.php?action=lostpassword"

> site:target.com inurl:"wp-contentpluginsall-in-one-seo-pack"

> site:target.com inurl:"wp-download.php?dl_id="

> site:target.com inurl:"wp-license.php?file=../..//wp-config"

> site:target.com inurl:"wp-security-audit-log" ext:log

> site:target.com inurl:/wp-content/plugins/fgallery/

> site:target.com inurl:/wp-content/plugins/inboundio-marketing/

> site:target.com inurl:/wp-content/plugins/seo-pressor/classes/

> site:target.com inurl:/wp-content/plugins/video-synchro-pdf

> site:target.com inurl:/wp-content/plugins/wpSS/

> site:target.com inurl:/wp-content/themes/tigin/

> site:target.com inurl:/wp-content/themes/xunjin/

> site:target.com inurl:/wp-content/uploads/ filetype:sql

> site:target.com inurl:/wp-content/uploads/ninja-forms/ intitle:"index of"

> site:target.com inurl:/wp-content/uploads/wp-backup-plus/

> site:target.com inurl:/wp-content/w3tc/dbcache/

> site:target.com inurl:/wp-content/wpbackitup_backups

> site:target.com inurl:/wp-includes/certificates/

> site:target.com inurl:wp-config.php intext:DB_PASSWORD

> site:target.com inurl:wp-content intext:backup-db

> site:target.com inurl:wp-login.php?action=register

> site:target.com inurl:wp-mail.php  + "There doesn't seem to be any new mail."

### Drupal

> site:target.com intext:"Powered by" & intext:Drupal & inurl:user

> site:target.com intext:"Powered by Drupal" inurl:"/node/1" -drupal.com -drupal.org -github

> site:target.com inurl:"sites/all/modules/ckeditor" -drupalcode.org

### Joomla

> site:target.com site:*/joomla/login

> site:target.com inurl:"/libraries/joomla/database/"

> site:target.com inurl:"/v1/config/application"

> site:target.com "Consola de Joomla! Debug" inurl:index.php

> site:target.com "Joomla! Administration Login" inurl:"/index.php"

> site:target.com "com_joom12pic"

> site:targer.com "com_joomlaflashfun"

> site:target.com "index.php?option=com_news_portal" or "Powered by iJoomla News Portal"

> site:target.com "powered by joomla 3.2" OR "powered by joomla 3.3" OR "powered by joomla 3.4"

> site:target.com Joomla Component com_eportfolio Upload Vulnerability

> site:target.com "com_ijoomla_rss"

> site:target.com index2.php?option=com_joomlaboard

> site:target.com intext:"joomla! 1.6 - Open Source Content Management"

> site:target.com intext:"joomla! 1.7 - Open Source Content Management"

> site:target.com intext:"~~Joomla1.txt" title:"Index of /"

> site:target.com intext:Joomla 1.6 inurl:index.php/login

> site:target.com intext:Joomla 1.6 inurl:index.php/registration

> site:target.com intext:Joomla 1.7 inurl:index.php/login

> site:target.com intext:Joomla 1.7 inurl:index.php/registration

> site:target.com intitle:"Index of /" "joomla_update.php"

> site:target.com intitle:"Joomla - Web Installer"

> site:target.com inurl:"com_ijoomla_archive"

> site:traget.com inurl:"com_joomlaradiov5"

> site:target.com inurl:"index.php?option=com_bookjoomlas"

> site:target.com inurl:com_joomladate

> site:target.com inurl:com_joomradio

> site:target.com inurl:component/content/

> site:target.com inurl:component/content/?view=featured&format=feed&type=atom*

> site:target.com inurl:index.php/plugins

> site:target.com inurl:index.php/rss=feed

> site:target.com inurl:index.php/using-joomla/extensions/modules/ intext:joomla! 1.7

> site:target.com inurl:index.php/using-joomla/extensions/modules/19-sample-data-articles/joomla/50-upgraders

> site:target.com inurl:index.php/using-joomla/extensions/plugins?format=feed&type=rss

> site:target.com inurl:index.php/using/joomla

> site:target.com inurl:index.php?format=feed&type=atom

> site:target.com inurl:index.php?format=feed&type=rss

> site:target.com inurl:index.php?option=com_joomlaconnect_be

> site:target.com inurl:index.php?option=com_joomradio

> silte:target.com inurl:using-joomla/extensions/templates/beez5/home-page-beez5

> site:target.com inurl:joomla3.txt filetype:txt

### Magento

> site:target.com "Log in" "Magento is a trademark of Magento Inc."

> site:target.com php jembut.php "/account/forgotpassword"

> site:target.com php jembut.php "/adminhtml/default/default/"

> site:target.com php jembut.php "/catalog/seo_sitemap/category/"

> site:target.com php jembut.php "/catalogsearch/advanced"

> site:target.com php jembut.php "/catalogsearch/result/"

> site:target.com php jembut.php "/catalogsearch/result?q="

> site:target.com php jembut.php "/catalogsearch/term/popular/"
 
> site:target.com php jembut.php "/customer/account/"

> site:target.com php jembut.php "/customer/account/login/referer/"

> site:target.com php jembut.php "/default/sales/"

> site:target.com php jembut.php "/firecheckout/"

> site:target.com php jembut.php "/frontend/enterprise/"

> site:target.com php jembut.php "/index.php/catalog/seo_sitemap/category/"

> site:target.com php jembut.php "/index.php/catalogsearch/term/popular/"

> site:target.com php jembut.php "/js/mage/"

> site:target.com php jembut.php "/sales/guest/form/"

> site:target.com php jembut.php "/skin/adminhtml/default/"

> site:target.com php jembut.php "/skin/frontend/"

> site:target.com php jembut.php "Login or Create an Account. Registered Customers. If you have an account with us, log in using your email address. *Email Address. *Password. Login"

> site:target.com php jembut.php "index.php/account/forgotpassword"

> site:target.com php jembut.php "index.php/adminhtml/default/default

> site:target.com php jembut.php "index.php/catalogsearch/advanced"

> site:target.com php jembut.php "index.php/catalogsearch/result/"

> site:target.com php jembut.php "index.php/catalogsearch/result?q="

> site:target.com php jembut.php "index.php/customer/account/"

> site:target.com php jembut.php "index.php/customer/account/login/referer/"

> site:target.com php jembut.php "index.php/default/sales/"

> site:target.com php jembut.php "index.php/sales/guest/"

> site:target.com php jembut.php "index.php/sales/guest/form/"

> site:target.com php jembut.php "inurl:/account/create/"

> site:target.com php jembut.php "inurl:/catalogsearch/advanced"

> site:target.com php jembut.php "inurl:/catalogsearch/result/"

> site:target.com php jembut.php "inurl:/catalogsearch/result?q="

> site:target.com php jembut.php "inurl:/customer/account/"

> site:target.com php jembut.php "inurl:/customer/account/login/referer/"

> site:target.com php jembut.php "inurl:/default/sales/"

> site:target.com php jembut.php "inurl:/sales/guest/form/"

> site:target.com php jembut.php "inurl:lib/3Dsecure/"  

> site:target.com php jembut.php "inurl:lib/LinLibertineFont/"

> site:target.com php jembut.php "inurl:lib/flex/"

> site:target.com php jembut.php "inurl:lib/googlecheckout/"

> site:target.com php jembut.php "inurl:skin/frontend/base/"

> site:target.com php jembut.php "inurl:skin/frontend/default/blank/"

> site:target.com php jembut.php "inurl:skin/frontend/default/blue/"

> site:target.com php jembut.php "inurl:skin/frontend/default/default/"

> site:target.com php jembut.php "inurl:skin/frontend/default/french/"

> site:target.com php jembut.php "inurl:skin/frontend/default/german/"

> site:target.com php jembut.php "inurl:skin/frontend/default/iphone/"

> site:target.com php jembut.php "inurl:skin/frontend/default/modern/"

### Symfony

> site:target.com intitle:"index of" "symfony/config"

> site:target.com inurl:"_fragment" | inurl:"_profiler"

> site:target.com inurl:"_profiler/phpinfo"

> site:target.com inurl:"_profiler/open"

### Ruby on rails

> inurl:"index.rb" "target.com"

> inurl:"/config/database.yml" "target.com"

> inurl:"/config/initializers/secret_token.rb" "target.com"

> inurl:"/db/seeds.rb" "target.com"

> inurl:"/db/development.sqlite3" "target.com"


---

Medium articles for more dorks:

https://thegrayarea.tech/5-google-dorks-every-hacker-needs-to-know-fed21022a906

https://infosecwriteups.com/uncover-hidden-gems-in-the-cloud-with-google-dorks-8621e56a329d

https://infosecwriteups.com/10-google-dorks-for-sensitive-data-9454b09edc12

Top Parameters:

https://github.com/lutfumertceylan/top25-parameter

Proviesec dorks:

https://github.com/Proviesec/google-dorks
