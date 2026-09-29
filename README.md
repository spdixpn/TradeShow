# DIX Trade Show 2027 Website

One-page event website for the **DIX Performance Trade Show 2027**, February 25–28, 2027, at the Hilton Phoenix Tapatio Cliffs Resort in Phoenix, Arizona.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The complete website. All styles, scripts and the logo are built into this one file. |
| `robots.txt` | Tells search engines they may index the site. |
| `README.md` | This file. |

## Deploying

1. Upload `index.html` and `robots.txt` to the root folder of the web host for `register.dixperformancenorth.com`.
2. Visit the site and confirm the page loads and the logo appears.

No build step, database or server-side code is needed. The only external resource is Google Fonts (Big Shoulders Display, Archivo, JetBrains Mono). If the fonts fail to load, the page falls back to system fonts.

## Page sections

The menu links jump to each section:

1. **Hero:** logo, intro, dates, city, hotel, registration deadline, Register button
2. **What's Included:** airfare, 3 hotel nights, ATV ride and dinner, lunch and drinks
3. **Why Attend:** 17 training sessions, 1 show day, 3 nights in Phoenix
4. **Schedule:** Thursday Feb 25 to Sunday Feb 28
5. **Manufacturer Training:** Friday session list, filterable by room (Sage 1 / Sage 3)
6. **Dinner:** ATV ride and dinner at Arizona Outdoor Fun, New River, AZ
7. **Venue:** hotel address, phone, amenities, map link
8. **Media:** event video and 2026, 2024 and 2023 photo galleries
9. **FAQ:** terms and conditions for attendees
10. **Contact:** territory managers
11. **Footer:** social links

## Common edits

Open `index.html` in any text editor and search for the text shown below.

| To change | Search for |
|-----------|-----------|
| Registration deadline | `Registration closes November 30, 2026` (appears twice) |
| Registration form link | `cognitoforms.com/DixPerformanceNorth/TradeShowGuestRegistration` (appears 3 times) |
| Show dates in the hero | `Feb 25–28, 2027` |
| Daily schedule | `<section id="schedule"` |
| Training sessions | `const sessions=[`. Each line is `["time","manufacturer","room","optional subtitle"]` |
| Territory managers | `const reps=[`. Each line is `["name","territory","phone","email"]`. Use `null` for no phone. |
| Dinner details | `<section id="dinner"` |
| Terms and conditions | `<section id="terms"` |
| Logo | The logo is stored inside the file as `data:image/webp;base64,...`. To swap it, replace that whole `src` value with a new image link, for example `src="logo.png"`, and upload the image beside `index.html`. |

## Key links

- Registration: https://www.cognitoforms.com/DixPerformanceNorth/TradeShowGuestRegistration
- Hotel: Hilton Phoenix Tapatio Cliffs Resort, 11111 North 7th Street, Phoenix, AZ 85020, (602) 866-7500
- Dinner venue: https://azoutdoorfun.com/
- 2026 gallery: https://photos.app.goo.gl/p1A2JR3fXWy7UwFk6
- Main site: https://www.dixperformancenorth.com/

## Open items

- [ ] Add a phone number for Ryan Dawson (SK & MB)
- [ ] Confirm the time for the ATV ride and dinner (shown as "Time TBA"). Arizona Outdoor Fun checks riders in from 7am to 3pm between October and February, which overlaps Friday's 8am–5pm training.
- [ ] Confirm the Saturday lunch location (shown as "Location TBA")
- [ ] Update the show-order dates in the Terms section, which still say February 2024
