# West Close Cottage — redesign concept

An upgraded version of the West Close Cottage page for
[West Close Farmhouse Cottages](https://westclosefarmhouse.co.uk), Melmerby, Coverdale.

It's the existing page — their photographs, their wording, their published tariff — rebuilt so
that a guest can check availability, see a price, and send an enquiry without leaving it.

This is an unsolicited design concept. It is not the live site and not a working booking system.

## What's new on the page

| | |
|---|---|
| **Availability & price inline** | Pick dates, see the season and the total — no separate prices page |
| **Letting rules built in** | Weeks snap to Saturday; short breaks only offered in Low Season and Winter, with the next window shown |
| **Enquiry pre-filled** | "Request these dates" carries the quote into the enquiry form |
| **Filterable facilities** | Dogs, family, cosy, outdoors, practical |
| **Gallery in context** | Ten photographs beside the price and the booking action |
| **Phone kept prominent** | Top bar, booking card and footer — it's still a phone-first business |

## Tariff and rules

Weekly prices are the published tariff: High £600, Mid £530, Low £430, Winter £365.
Season date bands are inferred from the published availability calendar. Short-break nightly
pricing is a guide (weekly ÷ 7 plus 15%) and is labelled as such on the page.
Dogs are a declaration, not a charge, per the published dog policy.

## Build

One self-contained `index.html`. No dependencies, no build step. Photographs are embedded so the
page works offline. Google Fonts is the only external request.

WCAG AA contrast verified across light and dark themes. Keyboard operable with visible focus.
`prefers-reduced-motion` respected.

All photography © West Close Farmhouse, used for illustration within this concept only.
