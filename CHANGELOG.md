# Changelog

## 3.0.1
- support for tcp:// conversion to http://

## 3.0.0
- swapped to use curl to address ssl certificate issues with php 5.6

## 2.7.2
- added x-use-https header check
- added max number of location redirects
- added custom settable message if x-use-https is found, so users can be told where to set their scripts
- if a redirect host is https, add ssl:// to remote_host

## 2.7.1
- added isset to headers['location'], line 306