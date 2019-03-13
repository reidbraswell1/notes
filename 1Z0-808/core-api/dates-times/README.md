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

| | Pre Java 8 | Java 8 |
| --- | --- | ---|
|import | import java.util.\*; | import java.time.\*; |
|create date | Date dt = new Date(); | LocalDate dt = LocalDate.now(); |
|create date & time | Date dt = new Date(); | LocalDateTime dt = LocalDateTime.now(); |
