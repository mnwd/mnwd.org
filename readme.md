# Minnesota Web Development

## A Historical Note

This is the source of the current MNWD website. Both the group and the website are inactive at the moment; this material is provided for archival purposes. It is not available for reuse or redistribution. If you would like to make a contribution, please open an issue.

## Development

This is the repository for hacking on the MNWD website, usually located at http://mnwd.org.

To get up and running, simply drop this in a live docroot and go.  The site is entirely static at the moment.

### We are looking for contributions related to:
* Resources page
* Basic styles (no actual branding or themeing)
* Fixing of trivial errors
* Other cool things that you might develop and send to us in a pull request

### Sample Apache config
```
<VirtualHost *:80>
    DocumentRoot "/Sites/mnwd/public"
    ServerName mnwd.org
</VirtualHost>
```

### Sample nginx config
```
server {
    listen       *:80;
    server_name  mnwd.org www.mnwd.org;

    location / {
        root   /www/mnwd.org/public;
        index  index.html index.htm;
    }
}
```
