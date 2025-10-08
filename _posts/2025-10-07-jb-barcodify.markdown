---
title: "JB Barcodify"
layout: post
date: 2025-10-07 20:44
image: /assets/images/jb-barcodify.png
headerImage: true
projects: true
tag:
- markdown
- elements
star: false
category: projects
author: james
description: My Little Chromium Extension
---
## About
JB Barcodify is a chromium based extension that I wrote with the primary intention of showing barcodes on the JB Hi-Fi website. Since then it has evolved with little quality of life features that I think make the retail job just a little bit easier. You can get it on the Chrome Web Store [here](https://chromewebstore.google.com/detail/nakfemijaepiebdfgjebkkijbhgpdlpj).
## Features
- Display Barcodes on the Product Page of the Website
- Display a button to open the Product Page in the internal Product App
- A shortcuts tab in the extension pop-up with keyboard keys to launch
- A settings page to choose what to enable
- Display a Internal Information Section with season code, supplier and warranty
- A Live stock display, similar to the PDA's *(testing)*
- Hide prices on the Product App (good for floor PC's)


## The Story
Within my job (working as a team member at JB Hi-Fi), we would have to lookup items constantly to see if we had them in stock to give to the customer. There were however *big* problems with using our internal systems to lookup stock, and so the employees often ended up using the customer facing website to actually find items, then type in their SKU (shopkeeping unit) into our PDA's (little Zebra computer thingy) to actually get information about the items and write up a sale, etc. For me there were 2 huge problems with this; being A, the website was, and continues to be ridiculously slow for a multi-billion dollar company and B, typing in a tiny, size 7 font SKU was not helpful for someone with astigmatism (me), let alone anyone.

From this frustration JB Barcodify was born... well, sort of.

When in sales, this wasn't a huge deal. It was just sort of what you expected when you wanted to sell stuff to customers, but at some stage I decided to check if a DVD was in stock for a customer, and this wasn't fun. Not only did most DVD purchasing customers come into store with a list of media that they wanted to purchase, but we also handily sold various different releases, so one movie turned into about 2 or 4 SKU typing experiences, *and thats just for one film!*

So yeah, this wasn't really acceptable and I really wanted to fix it, not only for me, but for my colleagues too. I had long known about the fact that numerous shopping websites displayed PLU codes (Price Look-Up Codes) and with this knowledge, turning it into a barcode just made sense.

All it took for me to write the extension was a short little holiday away to the Gold Coast. On the final day of my trip, I woke up ridiculously sick, not ideal as I had a flight to board, and work at 4pm that evening. I eventually texted my manager something like this:
```
Me: Hiiii, ive woken up ill today, wont be able to make it to my shifty tonight :(
Manager: All good feel better
```
What I didn't tell my manager however is that by the time I got back to Sydney (on a very delayed flight), I actually started to feel better. With my shift gone, I could start to work on my extension. I was up till about 2am that night, but by the end of it, I had learnt a lot.

---
The first version of JB Barcodify was pretty bare-bones. It literally loaded, grabbed the html element where the PLU belonged, extracted the numbers from it, created a blank svg element on the page and generated a barcode, using a third party service. Whilst it worked, it lacked a certain level of polish that I would usually like in my work, and over the coming days, I made lots of improvements. 

The extension today is pretty feature complete. I've made a lot of changes that I personally believe make the life of retail employees at JB Hi-Fi a little easier than in the past. If you have any suggestions, issues or anything else, get in contact!

If you'd like to look at the source code, you can find it [here](https://github.com/GreenFrog53/JB-Barcodify) on Github.