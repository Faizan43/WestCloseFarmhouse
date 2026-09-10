# West Close Reimagined

A redesign concept for [West Close Farmhouse Cottages](https://westclosefarmhouse.co.uk), a
two-cottage self-catering let in Melmerby, Coverdale, in the Yorkshire Dales.

This is an **unsolicited design concept**, prepared to demonstrate what the site could do
beyond its current brochure form. It is not a live booking system and is not affiliated with
or endorsed by the business.

**[View the page →](https://faizan43.github.io/WestCloseFarmhouse/)** *(once Pages is enabled)*

---

## What this demonstrates

The current site is a well-photographed, properly responsive WordPress build. It is not
broken — the gap is that nothing on it can *close a booking*. Every enquiry lands on a phone
call or a contact form.

This concept adds the missing layer:

| | |
|---|---|
| **Instant quoting** | Live pricing from the real published tariff, driven by season |
| **Business rules in software** | Saturday-to-Saturday snapping; short breaks restricted to Low Season and Winter |
| **Filterable amenities** | Dog-friendly, walking, cosy, practical — faceted rather than a wall of prose |
| **Inline gallery** | Photography beside the price and the booking action, not on a separate page |

Everything is one self-contained `index.html` — no build step, no dependencies, no backend.
The only external request is Google Fonts.

## The quoting engine

Rates are the cottage's own published weekly tariff:

| Season | Per week |
|---|---|
| High | £600 |
| Mid | £530 |
| Low | £430 |
| Winter | £365 |

Bookings are Saturday to Saturday, so an arrival date that isn't a Saturday is rolled forward
to the next one, and the page says so. Short breaks are offered only in Low Season and Winter
— picking a High or Mid Season date in short-break mode surfaces the rule and blocks the
quote rather than inventing a price.

Two things are **illustrative, not authoritative**, and are labelled as such on the page:

- the season date bands, inferred from the published availability calendar
- short-break nightly pricing (weekly ÷ 7, with a 15% short-stay uplift)

Dogs are modelled as a declaration rather than a charge, matching the published dog policy
("the intention to bring dogs must be disclosed at the time of booking").

## Verified against the live site

Claims made in the page's audit section were checked against westclosefarmhouse.co.uk rather
than assumed:

- **No online booking** — confirmed; the calendar is a display-only plugin, enquiries go
  through Contact Form 7
- **Weekly Sat–Sat letting, short breaks by phone** — confirmed from the published tariff page
- **WordPress 6.2 branch, Contact Form 7 5.7.6** — confirmed from loaded assets

Three things that are *good* about the current site are credited explicitly on the page: the
theme is genuinely responsive, the gallery already has 46 photos with a working lightbox, and
the availability calendar is accurate and current.

## Accessibility

- WCAG AA contrast verified on 21 elements across both light and dark themes — no failures
- Full keyboard operation with visible focus states
- `aria-pressed` on the stay-type and filter toggles
- `prefers-reduced-motion` respected

## Credits

All photography © West Close Farmhouse and is used here for illustration within this concept
only.

Typefaces: Fraunces (display), Work Sans (body), IBM Plex Mono (figures and dates).
