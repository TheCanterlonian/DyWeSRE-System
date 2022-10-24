# DyWeSRE-System
pronounced /die-wess-ree/ OR /die-wess-ur/ whichever you wish

Dynamic Web Server Redirection Entryway System

A collection of smaller systems working together to create an affordable solution to web hosting that allows home users to host websites from behind dynamically addressed internet access services.

By default the system described would use a web request of this page: http://checkip.dyndns.org/

The rate limit at current writing for this service is 300 requests per minute or 5 requests per second as listed here: https://help.dyn.com/managed-dns-api-rate-limit/

The system is intended to at most update every second and at least every hour so this limit is well within the intended accessing rate performed by the system.

for the ip checking portion of the system i used dynipmon:

https://github.com/TheCanterlonian/dynipmon

for connecting to the fixed static ip server i used sere:

https://github.com/TheCanterlonian/sere

for accepting connections from the dynamically allocated ip server i used serelo:

https://github.com/TheCanterlonian/serelo

These 3 parts all make up a whole system for managing dynamically assigned ips as if they were static ips.

Unfortunately this system only works if you recieve a public ip address, certain ISPs will not do this.

