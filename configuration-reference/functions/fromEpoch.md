---
description: This section contains reference documentation for the fromEpoch functions.
---

# fromEpoch

Convert epoch <Time Unit> to epoch milliseconds.
The following time units are supported:

* SECONDS
* MINUTES
* HOURS
* DAYS

## Signature

> FromEpoch<TIME_UNIT>(timeIn<Time_UNIT>)

## Usage Examples

```sql
select FromEpochSeconds(1613472303) AS epochMillis
FROM ignoreMe
```

| epochMillis   |
| ------------- |
| 1613472303000 |

```sql
select FromEpochMinutes(26891205) AS epochMillis
FROM ignoreMe
```

| epochMillis   |
| ------------- |
| 1613472300000 |

```sql
select FromEpochHours(448186) AS epochMillis
FROM ignoreMe
```

| epochMillis   |
| ------------- |
| 1613469600000 |

```sql
select FromEpochDays(18674) AS epochMillis
FROM ignoreMe
```

| epochMillis   |
| ------------- |
| 1613433600000 |