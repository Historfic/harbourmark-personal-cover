# Harbourmark — Personal cover (portfolio demo)

A one-page personal insurance enquiry page for a New Zealand cover adviser firm. Visitors answer three quick questions (where they want to start, whether they work for themselves, and what cover they already hold), add their contact details, and land on a thank-you screen with a mock booking calendar and a simulated AI-callback notice. Self-employed visitors are offered a business-owner cover chat instead of the personal one.

Live demo: https://historfic.github.io/harbourmark-personal-cover/

## About this project

Harbourmark Mortgages & Cover is a fictional brand, and this page is a portfolio piece. It is not a real business and does not give financial advice.

- **No backend.** The site is a static export of a Next.js + Tailwind page: HTML, CSS and JavaScript only. The fonts are self-hosted, so the page loads nothing from other sites.
- **Nothing is collected or sent.** The form checks what you type, then discards it. No requests are made, nothing is stored, and no cookies are set. A Content-Security-Policy blocks network calls and form submission.
- **The booking calendar is a mock.** It shows sample times, and picking one books nothing.
- **The AI phone call is simulated.** No call is placed.
- **The phone numbers are fictional** and use the 555-01xx range. The email address uses example.com.
- The insurer names are generic placeholders, and the adviser and the client reviews are invented.

## Run locally

The page is built to live at `/harbourmark-personal-cover/`, so serve it from a parent folder:

```bash
mkdir -p ../preview
cp -r . ../preview/harbourmark-personal-cover
cd ../preview && python -m http.server 8000
```

Then open http://localhost:8000/harbourmark-personal-cover/.
