ROYAL POWER MART — EASY EDIT WEBSITE

FILES
-----
index.html       Main website page (normally don't edit this)
style.css        Website design (normally don't edit this)
config.js        ★ EDIT THIS FILE for business information
assets/rpm-logo.jpg
location-qr.png

HOW TO CHANGE PHONE NUMBERS
---------------------------
Open config.js and find:
contacts: [
  { name: "Abhishek Baxi", phone: "9825440269" },
  ...
]

Change the name/number. Keep the phone number as digits only.
The website automatically creates both CALL and WHATSAPP buttons.

HOW TO CHANGE A BRANCH
----------------------
Find the branches section in config.js and change:
name
address
mapUrl

For a branch that does not have a Google Maps listing yet, leave:
mapUrl: ""

The website will show "Google Maps listing coming soon".
When the listing exists, paste its Google Maps link there.

HOW TO CHANGE EMAIL
-------------------
Change:
email: "rpm@royalpower.in"

HOW TO CHANGE BRANDS
--------------------
Edit the brands list near the bottom of config.js.

LOCATION QR
-----------
The current QR is the general Royal Power Mart location QR.
Replace location-qr.png if you ever need a different QR.
Do not change the QR unless you have tested the new one.

DEPLOYING TO CLOUDFLARE
-----------------------
This is a static website and is suitable for Cloudflare Workers
Static Assets. Upload the contents of this ZIP using the same
Worker you already created: royal-power-mart.

IMPORTANT
---------
Do not delete your Cloudflare DNS email records (MX, SPF, DKIM,
DMARC) while connecting the website. Email and website DNS are
separate.
