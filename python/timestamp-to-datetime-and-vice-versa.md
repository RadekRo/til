# timestamp to datetime and vice-versa

Datestamp to timestamp (number of seconds from January 1, 1970)
```
from datetime import datetime

# current date and time
now = datetime.now()

# convert from datetime to timestamp

# with miliseconds such as: 23345435346.122343
ts_ms = datetime.timestamp(now) 

# without miliseconds such as: 23345435346
ts = int(datetime.timestamp(now)) 

print("Timestamp with miliseconds =", ts_ms)
print("Timestamp without miliseconds =", ts)
```
Output:\
Timestamp with miliseconds = 1682150794.573145\
Timestamp without miliseconds = 1682150794

Timestamp to date-time format
```
from datetime import datetime

# convert the timestamp to a datetime object in the local timezone
dt_object = datetime.fromtimestamp(ts)

# print the datetime object and its type
print("dt_object =", dt_object)
```
Output:\
dt_object = 2023-04-22 08:06:34

---
_Last update: 21 Apr 2023_ 