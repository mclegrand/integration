# Changelog

## 1.0.3

- new grist, resana, docs, visio, rdv logos
- Gaufre button styles: add a focus-ring when the button is keyboard-focused. Before that, only the background changed a bit, arguably not an acceptable visual cue on its own.
- Gaufre button html: add disclosure ARIA design pattern attributes to improve experience for users of assistive technologies
- use DSFR v1.13.0

## 1.0.2

- new grist logo

## 1.0.1

- fix france-transfert/tchap/webconf logos (there were not the correct design)

## 1.0.0

Mark stable release!

- new service logos
- dev: add routes to test all homepage variants

## 0.1.8

- homepage: new "description" prop on `<HomepageContent>` to easily add custom content under the tagline. This matches this HTML: `<div class="lasuite-homepage__desc-container"></div>`.
- gaufre: new `variant` prop on `<Gaufre>` to impact visuals. Set to `small` or `responsive`. Matches CSS classes `lasuite-gaufre-btn--small` and `lasuite-gaufre-btn--responsive`.

## 0.1.6

- gaufre: hide the button if the gaufre.js script is not available
- gaufre: match DSFR tertiary button styling (gray-ish button border)
- gaufre: add a "button pressed" style
- gaufre: support DSFR dark theme via the `html[data-fr-scheme="dark"]` CSS selector

## 0.1.5

- homepage tagline: hide breaklines on mobile devices

## 0.1.3

Notable thing:

- the embedded DSFR styles required for the La Suite styles to work are now generated behind a specific CSS selector to have somewhat scoped CSS
- there is a new `dist/css/prefixed-dsfr.css` that includes the "scoped" DSFR styles
- the `dist/css/required-dsfr.css` has been renamed to `dist/css/raw-dsfr.css` and still includes the untransformed DSFR styles
- the `dist/css/homepage-full.css` file contains the scoped DSFR styles

Small changes:

- red border styling on top is now applied on header, not on homepage container
- fix tagline outputting an unnecessary trailing br tag
- fix homepage content background photo sizing
- fix spacing issue on the bottom of the ProConnect button

Dev :

- dev components are now all in a `dev` folder to better understand what is generated in the npm package and what is used only while developing
- better test the "full" and "standalone" CSS versions of the homepage

## 0.1.2

- Export more CSS in `dist/css` to enable fine-grained CSS usage. It prevents having to include the Gaufre CSS two times if we consume both homepage and gaufre CSS files.

## 0.1.1

- Add new services icons in public/logos.

## 0.1.0

First release!
