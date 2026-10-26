# EID Connect Examples: Emirates ID integration samples

> **Want one of these running in your business?** We install, customise and support EID Connect across the UAE.
> **[Get a commercial licence or free trial →](./COMMERCIAL.md)** · [info@elephantclock.ae](mailto:info@elephantclock.ae?subject=EID%20Connect) · [WhatsApp +971 50 702 2916](https://wa.me/971507022916)

Three ready-to-run examples of reading a UAE Emirates ID into a web app. Each is a
single HTML file with no build step and no framework.

| Example | For | What it shows |
|---|---|---|
| [**form-autofill**](./form-autofill) | Typing centres, clinics, real estate, car rental | Tap a card and a registration form fills in English and Arabic, with photo |
| [**visitor-kiosk**](./visitor-kiosk) | Offices, schools, gated sites | Check-in, a printable badge, and a visitor log that keeps only a masked ID |
| [**age-check**](./age-check) | Retail, venues, vape and tobacco | An allowed / not-allowed answer, expiry check, **stores nothing** |

## Run them

```bash
# 1. Start a reader. No hardware? Use the mock:
npx @elephantclock/eid-connect-mock

# 2. Serve this folder (any static server works)
npx serve .

# 3. Open http://localhost:3000/form-autofill/ and press "c" in the mock terminal
```

With a real reader, install the EID Connect service on the PC. The examples connect to
`http://localhost:8080` by default; add `?bridge=http://host:port` to point elsewhere.

`lib/eid-connect.js` is a copy of [eid-connect-js](https://github.com/elephantclock/eid-connect-js).
In your own app, use `npm install @elephantclock/eid-connect`.

## Licence

Free for **personal, educational and non-commercial** use under the
[PolyForm Noncommercial License 1.0.0](./LICENSE).
**Commercial use requires a licence**: see [COMMERCIAL.md](./COMMERCIAL.md).

---

Made in Abu Dhabi by [ElephantClock](https://www.elephantclock.ae) · [Docs](https://elephantclock.github.io/eid-connect/).
Not affiliated with or endorsed by ICP. All sample data is synthetic.
