# linked-meta

A lightweight serverless API that fetches Open Graph metadata (title, description, image, favicon) from any URL.

Built for the [linked](https://play.google.com/store/apps/details?id=com.satheesh.linkvault) Android app — replaces Microlink API with no rate limits.

---

## Endpoint

```
GET /api/fetchmeta?url=<encoded-url>
```

### Example

```
https://linked-meta.vercel.app/api/fetchmeta?url=https://youtube.com
```

### Response

```json
{
  "title": "YouTube",
  "description": "Enjoy the videos and music you love...",
  "imageUrl": "https://...",
  "favicon": "https://...",
  "domain": "youtube.com"
}
```

---

## Stack

- Node.js (Vercel Serverless Function)
- No dependencies — uses native `fetch`
- Deployed on Vercel free tier (100K requests/month)

---

## Deploy your own

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/satheeshmankulam-del/linked-meta)

---

## Built by

[Satheesh Mankulam](https://satheeshmankulam.com) — UX Designer & Android App Developer
