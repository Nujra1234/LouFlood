🌊 LouFlood Alert
Real-time Ohio River flood conditions for Louisville, Kentucky.
LouFlood Alert is a free, open-access web dashboard that combines live river gauge data from NOAA with upstream precipitation data from the Kentucky Mesonet to give Louisville residents a single, clear answer to the question that matters most during a flood event: How bad is it right now, and what should I do?
🔗 Live site: https://yourusername.github.io/louflood

What It Does
📊 Live Dashboard

Real-time Ohio River stage from NOAA Gauge MLXK2 (Louisville Water Tower)
Color-coded alert status: Normal → Watch → Warning → Major Flood
Interactive flood zone map showing affected Louisville neighborhoods
72-hour river level chart with flood stage threshold lines
Kentucky Mesonet upstream precipitation (stations CRMT and OLDA)
Flood Risk Index combining river stage + upstream rainfall
Stage-specific action guide (what to do right now)

🏠 Find Shelter

Four verified Louisville emergency shelters with addresses and phone numbers
Interactive map showing shelter locations relative to downtown
Emergency hotlines including 211, Red Cross, and Wayside transport

📋 Survival Guide

Before, during, and after flood checklists
Go-bag packing list
Louisville-specific tips (which roads close first, Beargrass Creek, floodwall limits)
FEMA assistance resources


Data Sources
SourceWhat It ProvidesNOAA NWPS — Gauge MLXK2Live Ohio River stage, flood thresholdsUSGS Site 0329450072-hour stage history for chartKentucky Mesonet (WKU)Upstream precipitation — stations CRMT (Bullitt Co.) and OLDA (Oldham Co.)
Official NOAA flood thresholds for Louisville (Gauge MLXK2):

Minor Flood Stage: 23 ft
Moderate Flood Stage: 32 ft
Major Flood Stage: 42 ft


How to Deploy
No build step, no server, no dependencies to install. It's a single HTML file.
GitHub Pages (free):

Create a new public repository on GitHub
Upload index.html (rename louflood_final.html → index.html)
Go to Settings → Pages → Source → Deploy from branch → main
Wait ~60 seconds — your site will be live at https://yourusername.github.io/reponame

Run locally:
Just open index.html in any browser. No local server needed.

Tech Stack
ToolPurposeVanilla HTML / CSS / JSNo framework neededLeaflet.js v1.9.4Interactive flood zone mapChart.js v4.4.072-hour river level chartCARTO Dark MatterMap tilesGoogle Fonts (Bebas Neue, DM Sans, DM Mono)TypographyNOAA NWPS APILive river gauge dataUSGS Water Services APIHistorical stage data
Cost to operate: $0. Everything uses free public APIs and free static hosting.

Project Background
This dashboard was built for the STEM360 Challenge 2025 in the Climate & Weather Community Problem category.
Louisville, KY faces one of the most persistent flood risks in the American Midwest. In April 2025 alone, the Ohio River rose to its 8th-highest crest in recorded history — causing 7 fatalities, 52,000+ power outages, and 500+ road closures across Jefferson County. Despite this recurring threat, no single accessible dashboard existed to help residents understand their real-time risk and take action.
LouFlood Alert addresses that gap.
Key design decisions:

Single HTML file — no install, no login, works on any phone browser
Fallback to realistic simulated data if APIs are unavailable (CORS restrictions in some browsers)
Auto-refreshes every 15 minutes
Flood zone polygons based on FEMA Zone A designations and Louisville MSD floodplain data


Flood Zones Shown on Map
NeighborhoodRisk LevelNotesPortlandWatch+Outside floodwall protectionShawnee Park / West LouisvilleWarning+Along Ohio River, outside floodwallButchertown / Beargrass CreekWatch+Floods independently of Ohio RiverWaterfront Park / Downtown RiverfrontWatch+Low-lying riverfront areasRubbertownMajor+Industrial area along river

⚠️ Polygon boundaries are neighborhood-level approximations of FEMA Zone A areas. For parcel-level accuracy, check Louisville Metro LOJIC or Louisville MSD's floodplain tool.


Verified Shelter Information
ShelterAddressPhoneNotesWayside Christian Mission432 E. Jefferson St, Louisville KY 40202502-584-371124/7, no activation needed, families welcomeSalvation Army911 S. Brook St, Louisville KY 40203502-671-4904400-person day shelter, 70 overnight bedsThe Healing Place1020 W. Market St, Louisville KY 40202502-585-4848Men only, 48 bedsFEMA Disaster Recovery CentersVaries by event211Active after disaster declaration only
Emergency transport to Wayside: 502-996-1888 (free during flood emergencies)

License
Free to use, share, and adapt for community emergency preparedness purposes.
Data is sourced from public U.S. government APIs (NOAA, USGS) and Kentucky state resources (Mesonet).

Built for Louisville. In an emergency, always call 911.
