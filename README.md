# BD Hijri Date API

This API provides official Hijri (Islamic) dates based on moon sightings in Bangladesh, as determined by the Islamic Foundation Bangladesh. It allows conversion of any Gregorian date from January 2025 onward to the corresponding Hijri date.

## Base URL

```
https://bd-hijri-dates.qomarhsn.com
```

## API Usage

### Get Hijri Date

```
GET /?date=DD-MM-YYYY
```

**Parameters**:

* `date` (optional): A Gregorian date in `DD-MM-YYYY` format.
  If omitted, the API returns today's date.

**Examples**:

1. Get today’s Hijri date:

   ```
   https://bd-hijri-dates.qomarhsn.com
   ```

2. Get the Hijri date for March 10, 2025:

   ```
   https://bd-hijri-dates.qomarhsn.com/?date=10-03-2025
   ```

**Response**:

```json
{
  "gregorianDate": "10-03-2025",
  "hijriDate": "09-09-1446"
}
```

## Notes

1. **Date Format**: Always use the `DD-MM-YYYY` format (e.g., `01-01-2025`)
2. **Supported Range**: Only dates from January 2025 onward are supported
3. **Data Updates**:

   * New months are added following announcements by the Islamic Foundation Bangladesh
   * Updates typically occur before each new Islamic month
   * The GitHub repository is automatically synced with the API

## Support

For support or to contribute:

* Start a discussion at [GitHub Discussions](https://github.com/qomarhsn/bd-hijri-dates/discussions)

## License

All data is available under the [GPLv3 License](LICENSE).