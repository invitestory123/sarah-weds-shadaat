# Customer Editing Guide — Sarah & Shadaat (Dawat-E-Walima)

Gilded palace hall wedding invitation featuring an animated tap-to-open cover video, rain-of-light particle animations, Dawat-E-Walima ceremony details, Google Map embed, and calendar synchronization.

---

## Normal Customer Changes

All routine customer edits are configured in:
→ `editable/wedding-data.js`

### 1. Couple Names & Header
Edit in `editable/wedding-data.js`:
- `kicker`: Event title (e.g. `"Dawat-E-Walima"`)
- `groom`: Groom's name (e.g. `"Shadaat"`)
- `bride`: Bride's name (e.g. `"Sarah"`)
- `groomFull`: Groom's full name (e.g. `"Shadaat Hanif"`)
- `brideFull`: Bride's full name (e.g. `"Sarah Samia"`)
- `groomParents`: Groom's parents (e.g. `"S/O Mr. Mohammad Hanif & Mrs. Mumtaz Parveen"`)
- `brideParents`: Bride's parents (e.g. `"D/O Late Mr. Imteyaz Ahmad & Late Mrs. Tabassum"`)
- `invitationLine`: Formal invitation line (`"Together with their families, request the honour of your presence"`)
- `closing`: Signoff message at the bottom

### 2. Dates & Countdown
Edit in `editable/wedding-data.js`:
- `dateLabel`: Formatted wedding date string (`"Wednesday, 02 December 2026"`)
- `shortDate`: Compact date display (`"2 December, 2026"`)
- `countdownTarget`: ISO date-time string (`"2026-12-02T20:00:00+05:30"`), drives live countdown timer & `.ics` calendar generation
- `countdownLabel`: Countdown header (`"Until the Dawat-E-Walima"`)
- `countdownDateLabel`: Formatted countdown subtext (`"Wednesday, 02 December 2026 (8 pm onwards)"`)

### 3. Blessings & Warm Invitation
Edit in `editable/wedding-data.js`:
- `grandfatherBlessing`: Kicker, heading, and union message
- `invitationFrom`: Title, hosts, and formal invitation message from Mr. Mohammad Hanif & Mrs. Mumtaz Parveen

### 4. Events & Ceremony
Edit `events` array in `editable/wedding-data.js`:
- Each event has:
  - `name`: Event name (`"Dawat-E-Walima"`)
  - `date`: Event date (`"Wednesday, 02 December 2026"`)
  - `time`: Event time (`"8:00 PM Onwards"`)
  - `venue`: Venue hall or lawn
  - `note`: Short festive description

### 5. Venue & Maps
Edit `venue` in `editable/wedding-data.js`:
- `name`: Venue name (`"Moti Mahal Lawn (Richi Rich)"`)
- `address`: Street address (`"Rana Pratap Marg, Shahnajaf Road, Lucknow"`)
- `hint`: Timing / transit landmark
- `mapsUrl`: Google Maps link (`"https://share.google/Oe3SL36L5jXAfyJLj"`)
- `mapEmbed`: Google Maps iframe embed URL

### 6. Media & Video
Replace files in `editable/assets/` or update paths in `wedding-data.js`:
- `cover`: Envelope cover illustration (`cover.png`)
- `introVideo`: Entrance opening animation (`intro.mp4`)
- `coupleVideo`: Couple loop video (`couple.mp4`)
- `hall`: Hall background architecture (`hall.png`)
- `petals`, `divider`, `floral`: Decorative ornaments

---

## Verification

1. Verify syntax with `node --check editable/wedding-data.js`.
