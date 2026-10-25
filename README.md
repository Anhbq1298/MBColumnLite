# MBColumn Lite — public website

This repository contains only the browser UI. The Eurocode 2 PMM solver, creep and slenderness calculations run on a separate **private** API. No PMM solver or fallback is shipped to the browser.

## Enable the site
In repository Settings → Pages, select Deploy from branch, main, /(root) and Save.

## Connect calculation API
Edit `index.html` and replace `https://REPLACE-WITH-RENDER-URL.onrender.com` with the HTTPS URL of your running API service.

## Security and readiness
Backend repository: private `MBColumnLite-API`. Never copy its solver source into this repository. The public site needs an online API service before calculations work. The API is not authenticated; secure, rate-limit and validate the service before broad public use.

This project is preliminary and should be validated against engineering baselines before design use.
