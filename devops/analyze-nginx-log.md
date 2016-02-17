#Analyze nginx access log

To decrease the bottleneck in the visit to our web servers we need a method to diagnose the response time of each request. The ops guys already aggregates logs for us on a daily basis. But how to read a log piece like this:

```
10.173.45.61 - - [04/Feb/2016:00:00:09 +0800] "GET /api/accounts/IGET/ANDROID/1009469/balance HTTP/1.0" 200 52 "-" "-" "0.020"
```

Some fields may be guessed out. I need to stress that the last one is the response time. It is critical for it controls the overall speed of our service. And the `52` is the response sent which means the data exchange.

Holding all the raw data it is impossible to gain insights. Fortunately I searched a tool called [GoAccess](http://goaccess.io/). It is a real time web log analyzer aiming to help us analyze nginx logs on the fly.