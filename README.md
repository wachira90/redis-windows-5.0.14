# redis-windows-5.0.14
redis on windows 5.0.14

## start redis on windows with config

```bat
redis-server.exe redis.conf
```

## result

```
Microsoft Windows [Version 10.0.19045.2673]
(c) Microsoft Corporation. All rights reserved.

D:\db\redis64-5>redis-server.exe redis.conf
[12108] 15 Mar 21:08:44.325 # oO0OoO0OoO0Oo Redis is starting oO0OoO0OoO0Oo
[12108] 15 Mar 21:08:44.325 # Redis version=5.0.14.1, bits=64, commit=ec77f72d, modified=0, pid=12108, just started
[12108] 15 Mar 21:08:44.327 # Configuration loaded
                _._
           _.-``__ ''-._
      _.-``    `.  `_.  ''-._           Redis 5.0.14.1 (ec77f72d/0) 64 bit
  .-`` .-```.  ```\/    _.,_ ''-._
 (    '      ,       .-`  | `,    )     Running in standalone mode
 |`-._`-...-` __...-.``-._|'` _.-'|     Port: 6379
 |    `-._   `._    /     _.-'    |     PID: 12108
  `-._    `-._  `-./  _.-'    _.-'
 |`-._`-._    `-.__.-'    _.-'_.-'|
 |    `-._`-._        _.-'_.-'    |           http://redis.io
  `-._    `-._`-.__.-'_.-'    _.-'
 |`-._`-._    `-.__.-'    _.-'_.-'|
 |    `-._`-._        _.-'_.-'    |
  `-._    `-._`-.__.-'_.-'    _.-'
      `-._    `-.__.-'    _.-'
          `-._        _.-'
              `-.__.-'

[12108] 15 Mar 21:08:44.346 # Server initialized
[12108] 15 Mar 21:08:44.347 * Ready to accept connections
```

## set password

edit redis.conf

```
requirepass passhere
```

## test

```
127.0.0.1:6379> set mykey myvalue
(error) NOAUTH Authentication required.
```
