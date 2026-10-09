# School HQ

A responsive student workspace designed to make school feel more manageable.

## Included in this rebuild
- Today dashboard with automatic next-task suggestions, upcoming due dates, and weekly progress
- Assignment create/edit/detail views, status and priority, due dates, Campus links, notes, estimated time, recurring tasks, and step-by-step breakdowns
- Quick-capture inbox for tasks you do not have time to organize yet
- Catch-up and overwhelmed modes to reduce the list to a manageable next action
- Focus timer with a short-break option
- Courses with course colors and completion progress
- Monthly due-date calendar and selected-day agenda
- Weekly class schedule for lectures, discussions, study blocks, and other commitments
- Study library for links, notes, readings, and guides
- Degree-credit progress tracking
- Search, filters, JSON backup/restore, and CSV assignment export
- Theme choices, text-size controls, compact layout, and mobile navigation
- Progressive web app manifest and a service worker that checks the network first so published updates are not stuck behind an old cached HTML file

## Existing data compatibility
The app keeps using the `schoolHQ.v1.data` browser-storage key and adds defaults for new fields. Existing courses, assignments, resources, and degree settings should be read by the rebuilt interface. This does not automatically move data between browser profiles or devices. Export a JSON backup before changing versions.

## Privacy and cloud sync
The app is local-first: assignments, course notes, and resources are stored in the browser on the device you use. No account or cloud upload is active in this build. Cross-device sign-in and sync require a properly configured backend such as Supabase, including authentication, a database, and row-level access policies. Do not put service-role keys or other private secrets in frontend code.

## Publish
This is a static site and can be hosted on GitHub Pages. The repository's published branch and folder must point to the branch containing the site files. The app is being prepared on the `rebuild-v2` branch so the current live version remains untouched while the replacement is reviewed.

## Backups
Use **Settings & backups → Export full backup** regularly. Store JSON backups somewhere private. The CSV export contains assignment data only.
