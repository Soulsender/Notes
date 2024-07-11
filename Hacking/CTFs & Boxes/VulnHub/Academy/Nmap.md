```
PORT   STATE SERVICE REASON  VERSION
21/tcp open  ftp     syn-ack vsftpd 3.0.3
| ftp-anon: Anonymous FTP login allowed (FTP code 230)
|_-rw-r--r--    1 1000     1000          776 May 30  2021 note.txt
| ftp-syst: 
|   STAT: 
| FTP server status:
|      Connected to ::ffff:192.168.56.1
|      Logged in as ftp
|      TYPE: ASCII
|      No session bandwidth limit
|      Session timeout in seconds is 300
|      Control connection is plain text
|      Data connections will be plain text
|      At session startup, client count was 1
|      vsFTPd 3.0.3 - secure, fast, stable
|_End of status
22/tcp open  ssh     syn-ack OpenSSH 7.9p1 Debian 10+deb10u2 (protocol 2.0)
| ssh-hostkey: 
|   2048 c7:44:58:86:90:fd:e4:de:5b:0d:bf:07:8d:05:5d:d7 (RSA)
| ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDIBuDzM6D8xmqki4fcCb1uEhi1lmznDpxYuviaBAbbHjCbMgiNZHBQj2gPjZcFhcgHkr5TtWv0slV3IyhbOZLvhaZUZu3HS/sm/Tz3heAx3C50MX1DcPNw3EpTDrzAwM5EsgnEEjAXPMXXG8JQ3X5k5xEbe2BoCBc1ZAxuLAXc2l3RyL/vrXCO2HappsmoZuX8OPchvtHSqBDjyQB/BDeb5VszUXTnb+utkE9bbZrFbYsa3Ed5JgOWMaxieKArHlECTpqlkdp5vSJ58iefVHwkq5qE2fap3G1HmcoI9RMNIT1AohXRQ8Hk5jQDr2xY8q6PjKGsxnw5YVmV7dx8j6aX
|   256 78:ec:47:0f:0f:53:aa:a6:05:48:84:80:94:76:a6:23 (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBDch5BCc2rqpCaaWap74M3GZ5y9APegx7XQyPXXIvxBgowvdssDnp119M5t59+djVOEoWiqKnaT0GQRpJWBs2Ig=
|   256 99:9c:39:11:dd:35:53:a0:29:11:20:c7:f8:bf:71:a4 (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIFHqfgMhJpRl/QNeg560fqH+J5jrVf0b/kUL9g94XZnp
80/tcp open  http    syn-ack Apache httpd 2.4.38 ((Debian))
| http-methods: 
|_  Supported Methods: OPTIONS HEAD GET POST
|_http-server-header: Apache/2.4.38 (Debian)
|_http-title: Apache2 Debian Default Page: It works
Service Info: OSs: Unix, Linux; CPE: cpe:/o:linux:linux_kernel

```