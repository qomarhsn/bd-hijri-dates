# BD Hijri Date API

This is a simple API to fetch the Hijri (Islamic) date for a given Gregorian date based on moon sighting in Bangladesh, as per the Islamic Foundation Bangladesh. The API changes the Hijri date at Maghrib time according to Bangladesh time and returns the corresponding Hijri date for the provided Gregorian date.

## How to Use the API

### Endpoint
- Base URL:  
  `https://bd-hijri-dates.mail-d0c.workers.dev/`

### Request Format
To get the Hijri date for a specific Gregorian date, you can make a request with the following format:

```
https://bd-hijri-dates.mail-d0c.workers.dev/?date=DD-MM-YYYY
```

### Example
For example, if you want to get the Hijri date for March 10, 2025, your request will look like this:

```
https://bd-hijri-dates.mail-d0c.workers.dev/?date=10-03-2025
```

### Response
The API will return a JSON response with the Gregorian date and the corresponding Hijri date:

```json
{
  "gregorianDate": "10-03-2025",
  "hijriDate": "09-09-1446"
}
```

### Notes
- The `date` parameter in the query string should follow the format `DD-MM-YYYY`.
- The Hijri date will be updated based on moon sighting each month according to Bangladesh's local time.
- Currently, this API only has the Hijri dates for March 2025. Dates for January and February 2025 will be added, and all future months will be updated as they come.

## License

This project is open-source and available under the [GPLV3](LICENSE).
