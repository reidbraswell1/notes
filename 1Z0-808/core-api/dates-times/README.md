### Dates and Times using LocalDate and LocalTime

```java
  import java.time.*;
```

|Class | Description |
| --- | --- |
|Clock | A clock providing access to the current instant, date and time using a time-zone. |
|Duration | A time-based amount of time, such as '34.5 seconds'. |
|Instant | An instantaneous point on the time-line. |
|LocalDate | A date without a time-zone in the ISO-8601 calendar system, such as 2007-12-03. |
|LocalDateTime | A date-time without a time-zone in the ISO-8601 calendar system, such as 2007-12-03T10:15:30. |
|LocalTime | A time without a time-zone in the ISO-8601 calendar system, such as 10:15:30. |
|MonthDay | A month-day in the ISO-8601 calendar system, such as --12-03.|
|OffsetDateTime | A date-time with an offset from UTC/Greenwich in the ISO-8601 calendar system, such as 2007-12-03T10:15:30+01:00.|
|OffsetTime | A time with an offset from UTC/Greenwich in the ISO-8601 calendar system, such as 10:15:30+01:00. |
|Period | A date-based amount of time in the ISO-8601 calendar system, such as '2 years, 3 months and 4 days'. |
|Year | A year in the ISO-8601 calendar system, such as 2007. |
|YearMonth | A year-month in the ISO-8601 calendar system, such as 2007-12. |
|ZonedDateTime | A date-time with a time-zone in the ISO-8601 calendar system, such as 2007-12-03T10:15:30+01:00 Europe/Paris. |
|ZoneId | A time-zone ID, such as Europe/Paris. |
|ZoneOffset | A time-zone offset from Greenwich/UTC, such as +02:00. |  

##### For the exam LocalDate, LocalDateTime, LocalTime, Period  


#### Creating a Date or Date Time
| | Pre Java 8 | Java 8 |
| --- | --- | ---|
|import | import java.util.\*; | import java.time.\*; |
|create date | Date dt = new Date(); | LocalDate dt = LocalDate.now(); |
|create date & time | Date dt = new Date(); | LocalDateTime dt = LocalDateTime.now(); |
|2017-01-01| Calendar cal = Calendar.getInstance();<br/>cal.set(2017, Calendar.JANUARY, 1);<br/>Date jan = cal.getTime(); | LocalDate jan = LocalDate.of(2017,Month.JANUARY,1);|
|2017-01-01<br/>1a.| Calendar cal = new GregorianCalendar(2017,Calendar.JANUARY, 1);<br/>Date jan = cal.getTime(); | --- |
|2017-01-01<br/>1b.| Calendar cal = Calendar.getInstance();<br/>cal.set(2017,0, 1);<br/>Date jan = cal.getTime(); | LocalDate jan = LocalDate.of(2017, 1, 1); |

#### Date Manipulation
|Method|Description|
| --- | ---|
|plusHours()<br/>minusHours()|Add/Subtract the number of hours to the date.|
|plusMinutes()<br/>minusMinutes()|Add/Subtract the number of minutes to the date.|
|plusSeconds()<br/>minusSeconds()|Add/Subtract the number of seconds to the date.|
|plusDays()<br/>minusDays()|Add/Subtract the number of days to the date.|
|plusWeeks()<br/>minusWeeks()|Add/Subtract the number of weeks to the date.|
|plusMonths()<br/>minusMonths()|Add/Subtract the number of months to the date.|
|plusYears()<br/>minusYears()|Add/Subtract the number of years to the date.|

#### Period
|Modifier and Type| Method | Description|
| --- | --- | --- |
|Temporal |addTo(Temporal temporal) |Adds this period to the specified temporal object.|
|static Period|	between(LocalDate startDateInclusive, LocalDate endDateExclusive)|Obtains a Period consisting of the number of years, months, and days between two dates.|
|boolean |equals(Object obj) |Checks if this period is equal to another period.|
|static |Period |from(TemporalAmount amount) |Obtains an instance of Period from a temporal amount.|
|long |	get(TemporalUnit unit) | Gets the value of the requested unit.|
|IsoChronology |getChronology()|Gets the chronology of this period, which is the ISO calendar system.|
|int |getDays() |Gets the amount of days of this period.|
|int |	getMonths() | Gets the amount of months of this period. |
|List<TemporalUnit> |	getUnits() | Gets the set of units supported by this period.|
|int | getYears() | Gets the amount of years of this period. |
|int | hashCode() | A hash code for this period. |
boolean 	isNegative()
Checks if any of the three units of this period are negative.
boolean 	isZero()
Checks if all three units of this period are zero.
Period 	minus(TemporalAmount amountToSubtract)
Returns a copy of this period with the specified period subtracted.
Period 	minusDays(long daysToSubtract)
Returns a copy of this period with the specified days subtracted.
Period 	minusMonths(long monthsToSubtract)
Returns a copy of this period with the specified months subtracted.
Period 	minusYears(long yearsToSubtract)
Returns a copy of this period with the specified years subtracted.
Period 	multipliedBy(int scalar)
Returns a new instance with each element in this period multiplied by the specified scalar.
Period 	negated()
Returns a new instance with each amount in this period negated.
Period 	normalized()
Returns a copy of this period with the years and months normalized.
static Period 	of(int years, int months, int days)
Obtains a Period representing a number of years, months and days.
static Period 	ofDays(int days)
Obtains a Period representing a number of days.
static Period 	ofMonths(int months)
Obtains a Period representing a number of months.
static Period 	ofWeeks(int weeks)
Obtains a Period representing a number of weeks.
static Period 	ofYears(int years)
Obtains a Period representing a number of years.
static Period 	parse(CharSequence text)
Obtains a Period from a text string such as PnYnMnD.
Period 	plus(TemporalAmount amountToAdd)
Returns a copy of this period with the specified period added.
Period 	plusDays(long daysToAdd)
Returns a copy of this period with the specified days added.
Period 	plusMonths(long monthsToAdd)
Returns a copy of this period with the specified months added.
Period 	plusYears(long yearsToAdd)
Returns a copy of this period with the specified years added.
Temporal 	subtractFrom(Temporal temporal)
Subtracts this period from the specified temporal object.
String 	toString()
Outputs this period as a String, such as P6Y3M1D.
long 	toTotalMonths()
Gets the total number of months in this period.
Period 	withDays(int days)
Returns a copy of this period with the specified amount of days.
Period 	withMonths(int months)
Returns a copy of this period with the specified amount of months.
Period 	withYears(int years)
Returns a copy of this period with the specified amount of years.
