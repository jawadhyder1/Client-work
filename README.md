# Kamran Electronics concept website

Ready-to-deploy static HTML, CSS and JavaScript. No npm install, API key, database or build step required.

## Open on your laptop

Extract the ZIP, open the `public` folder, and double-click `index.html`.
The page works locally. Google Fonts requires internet; system fonts are the fallback. Copying a message may require manual selection in a local-file or HTTP preview; automatic clipboard copying needs browser permission and a secure HTTPS page.

## Deploy on Vercel using GitHub

1. Extract the ZIP.
2. Create a GitHub repository, for example `kamran-electronics-demo`.
3. Upload the CONTENTS of this project folder: `public/`, `vercel.json`, and this README. Preserve the public/assets subfolder. Do not upload the ZIP itself.
4. Sign in to Vercel and choose Add New → Project. Import that GitHub repository.
5. Root Directory: repository root (the folder containing vercel.json).
6. Framework Preset: Other. Build Command: leave empty. Output Directory: public. No install command required.
7. Click Deploy. The supplied vercel.json already declares these settings.
8. Open the deployment URL and test it. Share the production URL supplied by Vercel with the business owner. If visitors see a Vercel sign-in screen, review that project's Deployment Protection settings before sharing.

Alternative for developers with Node.js: run `npx vercel --prod` from this directory and follow Vercel's sign-in/project prompts.

Official references checked on 29 October 2026:
- https://vercel.com/docs/builds
- https://vercel.com/docs/project-configuration/vercel-json
- https://vercel.com/docs/git

## Editing guide

- `public/index.html`: store name, contact number, address, page text, navigation, enquiry dialog.
- `public/styles.css`: colours, typography and responsive layout.
- `public/catalogue.js`: sample products, categories and questions. Category filters are generated automatically.
- `public/app.js`: search, filtering, detail dialogs, message builder and clipboard fallback.
- `public/assets/`: original SVG appliance illustrations and favicon. No external product photos needed.

To add a product, add another object to PRODUCTS using the existing schema and a unique id. The image field is the SVG filename without .svg. To use actual product photos, change the .svg image references in app.js to match your image format (two locations).

## Demo scope

Business name, phone and address came from the supplied public listing. They have not been confirmed by the owner. Six appliances are illustrative examples, not verified inventory. There are no invented prices, brands, reviews, warranties or opening hours. The logo and artwork are new concepts, not verified existing branding.

This prototype offers a catalogue and enquiry preparation, not checkout or online payment. It does not submit, store or send enquiry messages. Call buttons use tel: links. Directions opens a Google Maps search. WhatsApp is not linked because the supplied phone was not confirmed as a WhatsApp number.

Before an official launch, obtain owner-approved details, stock, product photographs and policies. Update the demo labels and remove both noindex directives (HTML robots meta and vercel.json X-Robots-Tag) only when the approved site is ready for search indexing.

## Validation

JavaScript syntax checked. Desktop browser: catalogue rendered, Cooling filter returned two products, details opened, product-specific enquiry populated, unsupported clipboard fallback selected the message, and empty search displayed a reset option. Responsive breakpoints included for mobile and tablet; physical mobile-device testing was not performed. No Vercel deployment has been performed from this package.
