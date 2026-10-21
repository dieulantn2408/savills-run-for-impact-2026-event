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
