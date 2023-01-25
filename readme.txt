steps for hosting a website
1) buy a domain from godaddy,namecheap or other website
2) after buyin domain change nameserver if you use any other dns management cms like cloudfare
3) for cloudfare go website add your site
4) add the domain proceed enable desired options 
5) cloudfare will show there nameservers copy them and go to domain buying website and in the dns management of godaddy change the nameservers to cloudfare
6) this will reflect in some minutes or hours.
after reflectiond done
7) open cloudflare and go to your site now 
-------------
8) go to whm create new account
add your domain like emergency24.in
give them standard package or ask sir which package should be given
create username and password for cpannel
now you will get the ip of cpannel 
---------------------
9) go to cloudflare open the site like emergency 24.in 
go to dns 
add A record given Name = @(means pointing to same domain emergency24.in and in the content paste the ip of whm cpannel in a record)
now add cname(means canonical name like www and in content @ )

if(any previous a record or cname exist delete them 

10) for email or other changes add mx records or spf value same if any my record or spf value remain delete them
---------------
now add ssl to the website

in clouflare go to SSL/TLS
enable in Full(strict) mode
on ssl recommender
then go in origin server create certificate
on origin pulls
then edge certificates
on always use https
in hsts settings 
a)enable hsts
max header (6months recommended)
subdomain option off
preload on
no sniff header on
tls on
hhtps reqwrites on









