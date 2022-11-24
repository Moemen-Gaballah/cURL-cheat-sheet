cURL Cheat Sheet [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
===============
<hr>
<p align="center">
    <img alt="cURL" src="./cURL.svg" height="190" width="455">
</p>
<hr>


cURL Cheat Sheet
===============


## Setup

```
you can use Git Bash in Windows if not exist in cmd
```

##### cURL version:
```
$ curl -V
```

##### Show cURL options:
```
$ curl --help
```
##### Get a single resource via URI:
```
$ curl https://jsonplaceholder.typicode.com/posts/1
```

##### Get a single resource via URI and show response header:
```
$ curl -i https://jsonplaceholder.typicode.com/posts/1
```

##### Show response header only:
```
$ curl -I https://jsonplaceholder.typicode.com/posts/1
```
####OR
```
$ curl --head https://jsonplaceholder.typicode.com/posts/1
```

##### Download response to file with a special name:
```
$ curl -o filename.txt https://jsonplaceholder.typicode.com/posts/1
```

##### Download response with limit size:
```
$  curl -O https://jsonplaceholder.typicode.com/megafamous.png
```

##### Download response with max size:
```
$  curl -O --limit-rate 1000B https://jsonplaceholder.typicode.com/posts
```

##### Send POST with data (-d or --data):
```
$ curl -X PUT -d "title=Hello&body=Hello World" https://jsonplaceholder.typicode.com/posts
```

##### Send request with method PUT To update data (-d or --data):
```
$ curl -X PUT --data "title=Hello01&body=Hello World Update" https://jsonplaceholder.typicode.com/posts/2
```

##### Send request with method DELETE To delete item:
```
$ curl -X DELETE https://jsonplaceholder.typicode.com/posts/2
```

##### basic authentication email:password
```
$ curl -u moemengaballa@gmail.com:12345678 https://site.com/login
```

##### basic authentication using token with curl

```
$ curl --header "Authorization: Bearer xxxxxxxxx" https://host.com/
```

##### request if url redirect (301 Moved) complete to redirect
```
$ curl -L https://google.com
```

##### upload file as FileZilla ftp to server
```
$ curl -u test@host.com:123456 -T hello.txt ftp://ftp.host.com
```

##### download file as FileZilla ftp
```
$ curl -u test@host.com:123456 -O hello.txt ftp://ftp.host.com/hello.txt
```

##### to ignore SSL certificate issues
```
$ curl --insecure https://www.google.com.eg/
```

##### Get SSL certificate information from web remote site
```
$ curl --insecure -vvI https://www.google.com.eg/
```
<hr>

## Reference

* [cURL Docs](https://curl.se/docs/)
* [Basic cURL Tutorial](https://www.youtube.com/watch?v=7XUibDYw4mc&ab_channel=TraversyMedia)

<hr>
