# SSL, HTTPS, and Security resources

## setting up SSL cert
https://konklone.com/post/switch-to-https-now-for-free
 - great tutorial for all of StartSSL
https://www.linode.com/docs/security/ssl/obtaining-a-commercial-ssl-certificate
https://www.linode.com/docs/security/ssl/ssl-certificates-with-nginx
https://www.digitalocean.com/community/tutorials/how-to-create-an-ssl-certificate-on-nginx-for-ubuntu-14-04

# SSL/TLS checking
https://www.ssllabs.com/projects/documentation/index.html
https://www.ssllabs.com/projects/best-practices/index.html

## SSL/TLS specific nginx configuration
http://nginx.org/en/docs/http/ngx_http_ssl_module.html#ssl_stapling_responder
  - also ssl_trusted_certificate, ssl_stapling, ssl_session_tickets, ssl_sesion_cache
https://gist.github.com/konklone/6532544 - awesome Nginx configuration
https://gist.github.com/konklone/6532544#comment-915900 - excellent HTTP/www forwarding code for nginx

## Certificate keysize
https://www.rapidssl.com/2048-bit-certificate-compliance/

## general Nginx configuration
https://t37.net/nginx-optimization-understanding-sendfile-tcp_nodelay-and-tcp_nopush.html

## General SSL/TLS setup gudes
https://wiki.mozilla.org/Security/Server_Side_TLS
http://security.stackexchange.com/questions/51680/optimal-web-server-ssl-cipher-suite-configuration

## Protocol relative urls
http://www.paulirish.com/2010/the-protocol-relative-url/

# General SSL/TLS descriptions
http://www.moserware.com/2009/06/first-few-milliseconds-of-https.html

## HTTPS marketing
http://www.w3.org/blog/TAG/2015/01/23/securing-the-web/
https://www.eff.org/encrypt-the-web
https://www.eff.org/https-everywhere
http://blog.codinghorror.com/should-all-web-traffic-be-encrypted/

## Perfect forward secrecy
https://scotthelme.co.uk/perfect-forward-secrecy/
https://en.wikipedia.org/wiki/Forward_secrecy

## Ciphersuite setup
https://scotthelme.co.uk/squeezing-a-little-more-out-of-your-qualys-score/
  - sets DH to 4096 bit key to achieve 100 key exchange score on qualys
https://hynek.me/articles/hardening-your-web-servers-ssl-ciphers/
en.wikipedia.org/wiki/Cipher_suite

## Heartbleed
https://heartbleed.com
https://twitter.com/ivanristic/status/453280081897467905
  - Heartbleed does not defeat PFS unless attacker grabbed ticket keys for current sessions

## SSLv3 insecurity
https://community.qualys.com/blogs/securitylabs/2014/10/15/ssl-3-is-dead-killed-by-the-poodle-attack

## SHA1 vulnerability
https://shaaaaaaaaaaaaa.com/
https://www.schneier.com/blog/archives/2012/10/when_will_we_se.html

## RC4 vulnerability
http://blog.cloudflare.com/killing-rc4/
http://en.wikipedia.org/wiki/RC4
https://tools.ietf.org/html/draft-ietf-tls-prohibiting-rc4-01
www.theregister.co.uk/2013/09/06/nsa_cryptobreaking_bullrun_analysis/

## MD5 vulnerability
http://www.tedunangst.com/flak/post/the-long-tail-of-MD5
https://konklone.com/post/why-google-is-hurrying-the-web-to-kill-sha-1#an-attack-on-sha-1-feels-plenty-viable-to-me

## HSTS preload
https://hstspreload.appspot.com/

## Crypto algorithms
http://en.wikipedia.org/wiki/Triple_DES
http://en.wikipedia.org/wiki/SHA1

## SSL ratings
https://www.ssllabs.com/ssltest/analyze.html?d=fastmail.com&s=66.111.4.148&latest A+
https://www.ssllabs.com/ssltest/analyze.html?d=konklone.com A+
https://www.ssllabs.com/ssltest/analyze.html?d=scotthelme.co.uk A+ 100 key exchange (4096 bit key)

FB, Twitter, Goodreads: B
