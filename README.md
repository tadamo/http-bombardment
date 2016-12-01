# Purpose

Load tests HTTP requests. - I wanted to see timings on every request and the response.

# Directions

```
$ cd http-load-test
$ cpanm --install-deps .
$ ./http-bombardment -c=30 -r=2 -b="user:*****" https://example.com/foo/bar
```

# Docker usage
```
$ docker build -t http-bombardment .
$ docker run --rm -it http-bombardment -c 10 -r 2 -b="user:*****" https://example.com/foo/bar
```
# Other Options

`ab`: http://httpd.apache.org/docs/2.2/programs/ab.html

`siege`: https://www.joedog.org/siege-home/
