---
execution:
- concurrency: 50
hold-for: 3m
ramp-up: 2m

scenario: Choose Flight
scenarios:
Choose Flight:
requests:
-label: blazedemo
method: GET
url: http://blazedemo.com/
label: reserve
method: POST
url: http://blazedemo.com/reserve.php
body:
fromPort: Paris
toPort: Buenos Aires,
