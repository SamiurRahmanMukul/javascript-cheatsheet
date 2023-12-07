# JavaScript Date Methods CheatSheet

```javascript
const currentDate = new Date();
```

| Methods              | Code Example                     | Result                          | Return Type |
| -------------------- | -------------------------------- | ------------------------------- | ----------- |
| getDate()            | currentDate.getDate()            | 7 (day of the month)            | number      |
| getDay()             | currentDate.getDay()             | 3 (day of the week, 0-6)        | number      |
| getMonth()           | currentDate.getMonth()           | 11 (month, 0-11)                | number      |
| getFullYear()        | currentDate.getFullYear()        | 2023                            | number      |
| getHours()           | currentDate.getHours()           | 15 (hour, 0-23)                 | number      |
| getMinutes()         | currentDate.getMinutes()         | 45                              | number      |
| getSeconds()         | currentDate.getSeconds()         | 30                              | number      |
| getMilliseconds()    | currentDate.getMilliseconds()    | 123                             | number      |
| getTime()            | currentDate.getTime()            | (timestamp)                     | number      |
| getTimezoneOffset()  | currentDate.getTimezoneOffset()  | (timezone offset in minutes)    | number      |
| setDate()            | currentDate.setDate(14)          | (sets day of the month to 14)   | number      |
| setMonth()           | currentDate.setMonth(5)          | (sets month to June, 0-11)      | number      |
| setFullYear()        | currentDate.setFullYear(2024)    | (sets full year to 2024)        | number      |
| setHours()           | currentDate.setHours(12)         | (sets hour to 12)               | number      |
| setMinutes()         | currentDate.setMinutes(30)       | (sets minute to 30)             | number      |
| setSeconds()         | currentDate.setSeconds(0)        | (sets second to 0)              | number      |
| setMilliseconds()    | currentDate.setMilliseconds(500) | (sets millisecond to 500)       | number      |
| setTime()            | currentDate.setTime(timestamp)   | (sets date to timestamp)        | number      |
| toDateString()       | currentDate.toDateString()       | "Tue Dec 07 2023"               | string      |
| toISOString()        | currentDate.toISOString()        | "2023-12-07T15:45:30.123Z"      | string      |
| toLocaleDateString() | currentDate.toLocaleDateString() | "12/7/2023"                     | string      |
| toLocaleTimeString() | currentDate.toLocaleTimeString() | "3:45:30 PM"                    | string      |
| toTimeString()       | currentDate.toTimeString()       | "15:45:30 GMT+0000 (UTC)"       | string      |
| toUTCString()        | currentDate.toUTCString()        | "Tue, 07 Dec 2023 15:45:30 GMT" | string      |
