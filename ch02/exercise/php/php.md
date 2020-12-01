### Exam 2. php 컨테이너 실행하기

**hello.php**

```
<?php phpinfo() ?>
```

**run**

```
$ docker run --rm \
  -v $(pwd)/hello.php:/app/hello.php \
  php:7 \
  php /app/hello.php

```