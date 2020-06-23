```
git clone git@github.com:myminseok/print-request.git
cd print-request
cf push

git clone git@github.com:myminseok/nginx-proxy.git
cd nginx-proxy
cf push
```

```
curl -kv -X POST -H 'Content-type: application/json' \
--data '{"text":"This is a line of text.\nAnd this is another one."}'  \
https://nginx-proxy.cfapps.io/print-request
```

```

   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT ----- Request Start ----->
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT /mkimprint
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT Host: mkimprint.cfapps.io
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT User-Agent: curl/7.64.1
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT Content-Length: 60
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT Accept: */*
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT B3: 2008e2eeaeeff39d-2008e2eeaeeff39d
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT Content-Type: application/json
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-B3-Spanid: 2008e2eeaeeff39d
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-B3-Traceid: 2008e2eeaeeff39d
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Cf-Applicationid: 0e82e97b-d569-4dec-9bc3-804d2d764036
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Cf-Instanceid: 6de43a4d-5ecd-4074-6de7-39bf
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Cf-Instanceindex: 0
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Forwarded-For: 14.34.56.49, 10.10.2.144, 3.88.180.182, 10.10.66.188
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Forwarded-Port: 443
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Forwarded-Proto: https
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Request-Start: 1592928714242
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Vcap-Request-Id: 08412c70-98bd-4194-6258-c1f513c4beb5
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT Host: mkimprint.cfapps.io
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT User-Agent: curl/7.64.1
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT Content-Length: 60
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT Accept: */*
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT B3: 2008e2eeaeeff39d-2008e2eeaeeff39d
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT Content-Type: application/json
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-B3-Spanid: 2008e2eeaeeff39d
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-B3-Traceid: 2008e2eeaeeff39d
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Cf-Applicationid: 0e82e97b-d569-4dec-9bc3-804d2d764036
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Cf-Instanceid: 6de43a4d-5ecd-4074-6de7-39bf
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Cf-Instanceindex: 0
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Forwarded-For: 14.34.56.49, 10.10.2.144, 3.88.180.182, 10.10.66.188
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Forwarded-Port: 443
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Forwarded-Proto: https
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Request-Start: 1592928714242
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT X-Vcap-Request-Id: 08412c70-98bd-4194-6258-c1f513c4beb5
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] ERR 10.249.147.111 - - [23/Jun/2020 16:11:54] "POST /mkimprint HTTP/1.1" 200 -
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT b'{"text":"This is a line of text.\\nAnd this is another one."}'
   2020-06-24T01:11:54.25+0900 [APP/PROC/WEB/0] OUT <----- Request End -----
```


https://webhook.site/
https://httpbin.org
