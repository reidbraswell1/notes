[calendar Doc](https://docs.python.org/3/library/calendar.html)
[datetime Doc](https://docs.python.org/3.7/library/datetime.html)

### Text Calendars

```python
  import calendar
  import datetime
  
  today = datetime.datetime.today()
  year = today.year
  month = today.month
  
  c = calendar.TextCalendar(calendar.SUNDAY)
  str = c.formatmonth(year,month)
  print(str)
  
  # Alternate Method
  calendar.setfirstweekday(calendar.SUNDAY)
  print(calendar.month(year,month))
```
```
      May 2019
Su Mo Tu We Th Fr Sa
          1  2  3  4
 5  6  7  8  9 10 11
12 13 14 15 16 17 18
19 20 21 22 23 24 25
26 27 28 29 30 31
```
### HTML Calendar

```python
  import calendar
  import datetime
  
  today = datetime.datetime.today()
  year = today.year
  month = today.month
  
  hc = calendar.HTMLCalendar(calendar.SUNDAY)
  str = hc.formatmonth(year,month)
  print(str)
```
```html
<table border="0" cellpadding="0" cellspacing="0" class="month">
<tr><th colspan="7" class="month">May 2019</th></tr>
<tr><th class="sun">Sun</th><th class="mon">Mon</th><th class="tue">Tue</th><th class="wed">Wed</th><th class="thu">Thu</th><th class="fri">Fri</th><th class="sat">Sat</th></tr>
<tr><td class="noday">&nbsp;</td><td class="noday">&nbsp;</td><td class="noday">&nbsp;</td><td class="wed">1</td><td class="thu">2</td><td class="fri">3</td><td class="sat">4</td></tr>
<tr><td class="sun">5</td><td class="mon">6</td><td class="tue">7</td><td class="wed">8</td><td class="thu">9</td><td class="fri">10</td><td class="sat">11</td></tr>
<tr><td class="sun">12</td><td class="mon">13</td><td class="tue">14</td><td class="wed">15</td><td class="thu">16</td><td class="fri">17</td><td class="sat">18</td></tr>
<tr><td class="sun">19</td><td class="mon">20</td><td class="tue">21</td><td class="wed">22</td><td class="thu">23</td><td class="fri">24</td><td class="sat">25</td></tr>
<tr><td class="sun">26</td><td class="mon">27</td><td class="tue">28</td><td class="wed">29</td><td class="thu">30</td><td class="fri">31</td><td class="noday">&nbsp;</td></tr>
</table>
```

[Back](../../../tree/python/README.md)
