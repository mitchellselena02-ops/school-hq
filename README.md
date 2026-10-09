# School HQ — first working version

A free, responsive, single-page school organizer. Open `index.html` in a browser to use it.

## Working features
- Dashboard totals, upcoming deadlines, and course activity
- Add, edit, complete, filter, search, and delete assignments
- Create/edit courses and track course assignment completion
- Monthly assignment calendar and selected-day agenda
- Searchable study library for links, readings, notes, and study guides
- Degree-credit progress tracker
- JSON backup/restore and CSV assignment export
- Responsive layout for laptop and mobile screens

## Data and privacy
This first version saves all records in the browser's local storage. It does not send the information to a server. Data does not sync across devices or browser profiles. Export a JSON backup regularly. Clearing browser data can remove School HQ's saved information.

## Free hosting
The site is static HTML/CSS/JavaScript and can be hosted on a free static hosting service such as GitHub Pages. Upload `index.html` to a repository, enable GitHub Pages in that repository's settings, and use the provided `github.io` address. No build step or paid domain is required. The site can still be edited locally and re-uploaded to publish updates.

## Next milestone
If cross-device syncing or sign-in is needed, add a secure cloud database/authentication layer on a free tier. Do not put private API keys or Airtable personal access tokens inside browser JavaScript. Framer's Airtable sync plugins are built for syncing records into the Framer CMS and do not by themselves provide a full two-way app backend.
