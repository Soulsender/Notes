### Port 80
```
301      GET        9l       28w      313c http://192.168.56.6/public => http://192.168.56.6/public/
200      GET      107l      370w     3833c http://192.168.56.6/
301      GET        9l       28w      310c http://192.168.56.6/src => http://192.168.56.6/src/
301      GET        9l       28w      310c http://192.168.56.6/app => http://192.168.56.6/app/
301      GET        9l       28w      313c http://192.168.56.6/vendor => http://192.168.56.6/vendor/
301      GET        9l       28w      317c http://192.168.56.6/extensions => http://192.168.56.6/extensions/
301      GET        9l       28w      319c http://192.168.56.6/public/files => http://192.168.56.6/public/files/
301      GET        9l       28w      320c http://192.168.56.6/public/thumbs => http://192.168.56.6/public/thumbs/
301      GET        9l       28w      319c http://192.168.56.6/public/theme => http://192.168.56.6/public/theme/
301      GET        9l       28w      324c http://192.168.56.6/public/extensions => http://192.168.56.6/public/extensions/

```
### Port 8080
```
[####################] - 1m    220546/220546  3019/s  http://192.168.56.6:8080/dev 
[####################] - 1m    220546/220546  3015/s  http://192.168.56.6:8080/ 
[####################] - 0s    220546/220546  0/s     http://192.168.56.6:8080/dev/files => Directory listing (add -e to scan)
[####################] - 0s    220546/220546  0/s     http://192.168.56.6:8080/dev/pages => Directory listing (add -e to scan)
[####################] - 0s    220546/220546  0/s     http://192.168.56.6:8080/dev/forms => Directory listing (add -e to scan)
[####################] - 0s    220546/220546  0/s     http://192.168.56.6:8080/dev/config => Directory listing (add -e to scan)
[####################] - 0s    220546/220546  0/s     http://192.168.56.6:8080/dev/stamps => Directory listing (add -e to scan)
┌[soul@xps15] [~] 

```