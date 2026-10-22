# Savills Run for Impact 2026 – V57 Public Mobile
Deploy: Drag the ZIP to a NEW Netlify site (or unzip and deploy folder). Publish directory is root. No Firebase/Auth/Strava API needed. This is a public, read-only presentation website.

## Update verified results
Edit `results.json` and redeploy. Example:
{
 "updatedAt":"21/10/2026 17:00",
 "participants":[
  {"name":"Nguyen Van A","department":"PM","totalKm":24.5,"weeks":{"week1":10,"week2":8,"week3":6.5,"final":0}},
  {"name":"Tran Thi B","department":"HO","totalKm":12,"weeks":{"week1":12,"week2":0,"week3":0,"final":0}}
 ]
}
Only publish employee names/departments if authorized. No private contact information or Strava profile URLs. Cumulative totalKm should equal sum of approved weekly results. A static JSON is intentionally used: no accounts, no internal database, no client-side admin access. Results are NOT synced from Strava. HR/organizers must verify and publish.

## Settings
Goal VND 30m, provisional conversion VND 1,000 per verified KM: `GOAL` and `RATE` in app.js. CONFIRM the donation conversion before launch. Prize images, item names and detailed award rules are pending user confirmation; currently show only Top 30 / Top 20 / Top 10 / Top 5 / Champion. Campaign week dates also pending final confirmation.

## QA
Check VI/EN switch, mobile bottom tabs, Strava Club external link, search, weekly filters, zero-data state, donation progress and cube movement. If using existing Firebase project, this V57 does not read or write it. Do not deploy old firestore.rules from V56.

## V58 prizes
Images provided by organizer are cropped and placed in assets. Champion: Apple Watch SE 3; final week Top 5: Jogflow 100.1; week 3 Top 10: Wind 100 jacket; week 2 Top 20: Hiking Backpack; week 1 Top 30: HIKE Cap. These are award-stage displays, not automatic winner calculations. Confirm exact ranking eligibility and dates before launch.

## V59 official mascot
Replaced the single map cube with the exact user-provided running cube asset and reused it as the homepage key visual. No generated illustration is included.
\n## V60 restoration\nRestores the original `community-map.webp` route from run_v57, with one official supplied cube positioned along its route. Restores animated liquid-fill heart (not a static emoji), updates via results.json polling every 30 seconds while page is open. The display is near-live after HR publishes a verified JSON update; it is NOT real-time Strava sync. Replaces custom `savills.` with cropped official logo artwork; 2026 appears on a separate line. Guide step 3 updated in both languages. Champion section uses white background for the provided watch image. No old Firebase/auth features restored.\n
## V61 changes
Shortened leaderboard and guide disclaimer in VI/EN; donation heart now displays verified VND amount / 30,000,000 VND; cube scaled to 26–46 px to suit map gate. Original map and animated heart preserved.

## V62
Step 1 includes Strava display name format Employee ID - Full Name, example, and one-account-only policy in VI/EN. Header uses plain black `savills` text without dot, image crop, glow or shadow, as requested. Other V61 behavior unchanged.

## V63 FAQs and rules
Adds fifth bottom tab FAQs & Rules, fully bilingual, with the five user-supplied eligibility/verification rules and six common questions. Eligible dates: 23 Oct–22 Nov 2026. Existing pages and data logic retained.

V64: Updated employee name format H1234_Tran Ngoc A, treadmill verification and no manual KM; official updates in Strava Announcements channel, sharing in Club Posts; replaced all five prize images with user-provided assets.


## V65 — Official participation rules supersede previous drafts
The organizer's latest rules are authoritative: ONLY outdoor GPS-tracked Run/Walk, no treadmill, stationary running, cycling, manual entry or GPS-less activity. Valid time: 2026-10-23 00:00 through 2026-11-22 23:59 Vietnam time. Activities count only AFTER joining the Club. Strava account display name: EmployeeID_FirstNameLastName without spaces in the name (example H1234_LanTran); one account per employee. 30,000 KM is a collective goal, equivalent to VND 30m. Full eight rule categories, FAQ and onboarding steps revised in both VI/EN. Announcements channel and Club Posts guidance retained. The older V64 treadmill allowance and naming examples are obsolete. Prize photos and all visuals are unchanged.

V66: Naming format updated to MSNV_TênHọ / EmployeeID_FirstNameLastName, e.g. H1234_LanTran. First name precedes last name.
