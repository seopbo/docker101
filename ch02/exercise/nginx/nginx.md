### Exam 1. nginx 컨테이너 만들기

**index.html**

```
hello world
```

**run**

```
$ docker run -d --rm \
  -p 50000:80 \
  -v $(pwd)/index.html:/usr/share/nginx/html/index.html \
  nginx
```
