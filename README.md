# Linux Configuration Project

## IP address
52.26.106.90

## SSH port
2200

## Website URL
[Catalog App](http://ec2-52-26-106-90.us-west-2.compute.amazonaws.com)

## Software Installed

### apache2
Used to serve more the website application

### postgresql and postgresql-contrib
Used to install PostgreSQL. PostgreSQL is a powerful, open source object-relational database system.

### libapache2-mod-wsgi and python-dev
Used to install Mod_wsgi. Mod_wsgi is an Apache HTTP server mod that enables Apache to serve Flask applications.

### python-pip
Used to install pip. pip is a package management system used to install and manage software packages written in Python

### fail2ban
Used to install fail2ban. The fail2ban service is useful for protecting login entry points

## Configuration changes made

1. Add new user named grader and grant this user sudo permissions. Using adduser and gpasswd command.
2. Update all currently installed packages using apt-get update command.
3. Configure the local timezone to UTC using dpkg-reconfigure tzdata command.
4. Change the SSH port from 22 to 2200. Opening /etc/ssh/sshd_config file.
5. Configure the Uncomplicated Firewall (UFW) using ufw command. Denying all incoming request and allowing only the ports 2200(ssh), 80(http) and 123(ntp).
6. Install and configure Apache to serve a Python mod_wsgi application. Creating /etc/apache2/sites-available/CatalogApp.conf file to serve Catalog App website using port 80.
7. Set up a virtual environment to keep the application and its dependencies isolated from the main system. Using virtualenv command.
8. Install PostgreSQL and create user catalog to have limited permission to catalog database.  
9. Install git, to clone and set up the Catalog App project.
10. Install fail2ban to check the Apache logs for patterns that indicate malicious activity.

## RSA key
-----BEGIN RSA PRIVATE KEY-----
MIIEowIBAAKCAQEAtYKnnWsCSgTRUiZ+fFRaD3BTaHG63SXXG4/OWFFBRz9qWLAh
bcZlGqhHTzJlS9ZgyOseUTwOd2mY7omF4ZbMihErLLTO5D0+qMIKimjAHgUd/m7K
yqr7HURzm+8EJx1c2tElrq9YuojDc8tgPRMIL6SXtg7TYMImWhAzhnLlKzpu+NZO
tul4mQFpBHfq2PcYPcNBgIO+TcSAOhEYQHqpBHwbC83po70N46EjboZELS1lsAwf
KdKK60kviLQIHeOVjGiPsxjD8HtEu2lAedDv4AaxWOpeCcEc8Ern1XE2GcUno6Pt
KE9Q4Drt12zt+YRmtNKb+1NeTvzwhdKPB6RBCQIDAQABAoIBAFCNrI+bNwfcfX0k
4kuRL+rcIdgfaRvOOFneB2iAnyTcivjTKfLK8oHTHtqR9gyjFo70cZ8BtTXfomRy
mf0U7K91kSClGZCHcbB5dS4Z8PEhuj75snwhR5Kkl14jxEcLq/LckQmmfg1CtuND
5fEU6jQiqsW8bKjrYRPlTsijYvs8koTWI4jjs5G17o/LlIv6EU1cSXPnw0mJK3lK
QoSRZXALNvVUKKO6VK/OLwjnN3jbEWTk67K7oki2jNVTCnwV790VaaSI5ayoJ2Qc
VcLE+z7K7HXeLfK9xEQraQVhk/eJzUTstFs6wauxosCILLYVO9GPnuANSaR0QXtX
zWnpbNECgYEA60BuWm+gFQCELl0TZvvgp7tVAtdlT3qrjNhNeSgWKnLpri+ybLrn
uCMb9RCsZoiCYi9MhKaVzJVo6pkdovtc1uD4P9tQ8Ez1i90kmOdc6addibUMnONX
68CbIPpyyUkKPqqPG4sgqlizSWhLmFr+XB64pCB05Utwk7+mOJN44S0CgYEAxYTW
44CDidX3GuZA9i9lhWazJ9X9DgmaWIBnz8wOLxxsWUMhmv65QO0Bb/cvTSuIdudL
mX6jy3Ax4inP+mB6eb4hm9RF0ExKEm7Shd5+f5CUkLM4P06ILuO65Epbi39TDPdE
tPS5TBHJH6qdA9kt3+0GJsn6Gq220qIyohTNsM0CgYBLB6OqiEuAJ0gBGYJkqBTA
qki0vUn8jV1FcH9VEunu4/OPsHqxnvLkkZ4LDSRPF16uPfOjoxXHyCdMG0WOg6ja
h6nlg+dOnNz7nK5dbfz+MHjuwKWjLAcQk79mRzpw5DC2R+OYn0jty5hy4yapEuxp
KQsunYNq1iKznL5A8RfuiQKBgHDpN05mMMuinNeruIcDIS3ZP6EOGtLjenANN0r6
g0E7JlUAoz1PT+dllOTEkS20LRaLshPU6R1qzZlT/ahLbrgZkGzcM+yXL+DJqV8N
iZKyu7rcONM3uXHUjQnj1+Eur/NBhu1K2II7yJVpmsiQZkET5ehWnbqSg2h1gCxX
aB4hAoGBAM7aa0G7CXcOtAa2CHUBPpOo6tPfJh+6HFtht5jpg3SVFWeiPOF7is1l
+unIm2v8cF0qYoZH1rSdFl0vBtz0nKSRK0zy8vrIhLrHYI6f+w3xctVHqOYJJAyz
L2IUNY6PgFgTwpQr+Rl/rZyqoKw1YZ5VKLXbM7ePrF7xz9YR+/tY
-----END RSA PRIVATE KEY-----
