# Github dorks for Bug Bounty

A list of Github Dorks for Bug Bounty, Web Application Security, and Pentesting

<p>
Credits to TakSec: https://taksec.github.io/google-dorks-bug-bounty/
</p>

---

### TEST

> site:target.com test

### Secrets

> "target.com" private

> "target.com" ldap

> "target.com" password

> "target.com" passwd

> "target.com" pwd

> "target.com" secret

> "target.com" Jenkins

> "target.com" OTP

> "target.com" authorizition

> "target.com" ftp

> "target.com" dotfiles

> "target.com" JDBC

> "target.com" key-keys

> "target.com" send_keys-keys

> "target.com" send,key-keys

> "target.com" token

> "target.com" user

> "target.com" login-singin

> "target.com" passkey-passkeys

> "target.com" pass

> "target.com" SecretAccesKey

> "target.com" app_AWS_SECRET_ACCESS_KEY

> "target.com" AWS_SECRET_ACCESS_KEY

> "target.com" credentials

> "target.com" config

> "target.com" security_credentials

> "target.com" connectionstring

> "target.com" ssh2_auth_password

> "target.com" BD_PASSWORD

> "target.com" api_key

> "target.com" “api keys”

> "target.com" authorization_bearer:

> "target.com" oauth

> "target.com" auth

> "target.com" authentication

> "target.com" client_secret

> "target.com" api_token:

> "target.com" “api token”

> "target.com" client_id

> "target.com" user_password

> "target.com" user_pass

> "target.com" passcode

> "target.com" client_secret

> "target.com" password hash

> "target.com" user auth

> "target.com" api_hash

> "target.com" api_id

#bash / #Python / #sql / #php ...
language:<language> password
language:<language> pwd
language:<language> passwd
language:<language> secret
language:<language> private
language:<language> ldap
language:<language> ftp
language:<language> dotfiles
language:<language> JDBC
language:<language> key-keys
language:<language> send_keys-keys
language:<language> send,key-keys
language:<language> token
language:<language> user
language:<language> login-singin
language:<language> passkey-passkeys
language:<language> pass
language:<language> credentials
language:<language> config
language:<language> security_credentials
language:<language> connectionstring
language:<language> ssh2_auth_password
...
...

#Si vous trouvez un employé de la cible:
user:<users> linkedin
user:<users> full name
user:<users> https://
user:<users> ldap

#entreprise
org:<company> https://
org:<company> host:

### Vecteurs externes
  
> "target.com.atlassian"
  
> "target.com.okta"
  
> "corp.target.com"
  
> "jira.target.com"
  
> "target.com.oneline"
  
> "target.com.service-now"

### Generic
 
> "target.com" filename:manifest.xml
  
> "target.com" filename:travis.yml
  
> "target.com" filename:vim_settings.xml
  
> "target.com" filename:database
  
> "target.com" filename:prod.exs NOT prod.secret.exs
  
> "target.com" filename:prod.secret.exs
  
> "target.com" filename:.npmrc _auth
  
> "target.com" filename:.dockercfg auth
  
> "target.com" filename:WebServers.xml
  
> "target.com" filename:.bash_history
  
> "target.com" filename:sftp-config.json
  
> "target.com" filename:sftp.json path:.vscode
  
> "target.com" filename:secrets.yml password
  
> "target.com" filename:.esmtprc password
  
> "target.com" filename:passwd path:etc
  
> "target.com" filename:dbeaver-data-sources.xml
  
> "target.com" path:sites databases password
  
> "target.com" filename:config.php dbpasswd
  
> "target.com" filename:prod.secret.exs
  
> "target.com" filename:configuration.php JConfig password
  
> "target.com" filename:.sh_history
  
> "target.com" shodan_api_key language:python
  
> "target.com" filename:shadow path:etc
  
> "target.com" JEKYLL_GITHUB_TOKEN
  
> "target.com" filename:proftpdpasswd
  
> "target.com" filename:.pgpass
  
> "target.com" filename:idea14.key
  
> "target.com" filename:hub oauth_token
  
> "target.com" HEROKU_API_KEY language:json
  
> "target.com" HEROKU_API_KEY language:shell
  
> "target.com" SF_USERNAME salesforce
  
> "target.com" filename:.bash_profile aws
  
> "target.com" extension:json api.forecast.io
  
> "target.com" filename:.env MAIL_HOST=smtp.gmail.com
  
> "target.com" filename:wp-config.php
  
> "target.com" extension:sql mysql dump
  
> "target.com" filename:credentials aws_access_key_id
  
> "target.com" filename:id_rsa or filename:id_dsa
  
> "target.com" GitHub Dorks for Finding Languages
  
> "target.com" language:python username
  
> "target.com" language:php username
  
> "target.com" language:sql username
  
> "target.com" language:html password
  
> "target.com" language:perl password
  
> "target.com" language:shell username
  
> "target.com" language:java api
  
> "target.com" HOMEBREW_GITHUB_API_TOKEN language:shell

#Trouver des noms d'utilisateurs
user:name (user:admin)
org:name (org:google type:users)
in:login (<username> in:login)
in:name (<username> in:name)
fullname:firstname lastname (fullname:<name> <surname>)
in:email (data in:email)

#Utiliser les dates
created:<2012–04–05
created:>=2011–06–12
created:2016–02–07 location:iceland
created:2011–04–06..2013–01–14 <user> in:username

#Utiliser les extensions
extension:pem private
extension:ppk private
extension:sql mysql dump
extension:sql mysql dump password
extension:json api.forecast.io
extension:json mongolab.com
extension:yaml mongolab.com
[WFClient] Password= extension:ica
extension:avastlic “support.avast.com”
extension:json googleusercontent client_secret

#Autre
##Slack web hook
"https://hooks.slack[.]com/services/"
