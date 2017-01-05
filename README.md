# CVS

Docker container with alpine and cvs pserver

BUILD
-----

```console
docker build -t cvsgit/cvs .
```

VOLUME
------
```console
/var/cvsroot
```

ENV
---
```console
$CVS_USER #cvsuser
$CVS_PASSWD #cvspass
```

RUN
---
```console
docker run -d -p 2401:2401 alpine-cvs
```
