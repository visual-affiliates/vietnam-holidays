# vietnam-holidays

Vietnam public holidays as plain JSON, one file per year. Every entry says whether the dates are officially confirmed and links the source it came from.

Built for booking, payroll and scheduling apps that need to close on the right days. I use the same data in my own studio and spa software.

## Files

| File | Contents |
|---|---|
| data/2026.json | Vietnamese Culture Day, 24 November 2026 |
| data/2027.json | New Year, Tet, Hung Kings, Reunification Day, Labour Day, National Day, Culture Day |

## Entry format

```json
{
  "date": "2027-09-02",
  "name_vi": "Quốc khánh",
  "name_en": "National Day",
  "off_from": "2027-09-02",
  "off_to": "2027-09-05",
  "status": "official",
  "applies_to": "state sector",
  "notes": "...",
  "sources": ["S1", "S2", "S3"]
}
```

date is the holiday itself (for Tet, the first day of the lunar year). off_from and off_to are the whole break, including weekends and compensatory days. sources point to the URLs listed at the top of each file.

## Status values

| Status | Meaning |
|---|---|
| official | Confirmed in a government or ministry notice, as reported by the sources |
| expected | Listed by the sources as expected, not yet confirmed as approved |
| unconfirmed | Listed by a source, but it is not stated whether it is an official day off |

## Read this before you rely on it

- This is compiled from news reports of official notices, not from the official documents themselves. It is not legal advice.
- Most dates are for the state sector. Private employers can differ (for example National Day: 2 September plus either 1 or 3 September). Check the official notice for your case.
- Entries marked expected can change when the Prime Minister announces the final schedule.
- Last updated 31 October 2026. Each year after 2027 is missing until it is announced.

## Contributing

Found a wrong or newly announced date? Open a pull request or an issue and link the official notice or the news report. Include the notice number if there is one.

## License

MIT. See LICENSE.

Made by [William Wells](https://github.com/visual-affiliates) · [williamwells.vn](https://williamwells.vn)

Powered by ⚡️ William Wells
