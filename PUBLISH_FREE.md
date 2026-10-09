# Put School HQ online for free

This version is a static website, so it can be published on GitHub Pages at no monthly cost. GitHub Pages publishes HTML, CSS, and JavaScript from a repository.

## Before you start
- You need a free GitHub account.
- Publish only the *app files* listed below. Do not upload your JSON backup, real assignments, notes, or other personal school records to the repository.

## Steps
1. Sign in to GitHub and create a new repository named `school-hq`. For the simplest free setup, make the repository **Public**. The source code will be public, but your school records are not part of the source code; they stay in each browser's local storage.
2. Open the new repository and choose **Add file → Upload files**.
3. Upload these five files from the `school_hq` folder: `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, and `icon-512.png`. You can also upload `README.md` and `PUBLISH_FREE.md` if you want the instructions stored with the project.
4. Commit the files to the `main` branch.
5. Open **Settings → Pages** in the repository.
6. Under **Build and deployment**, choose **Deploy from a branch**, select branch `main` and folder `/(root)`, then save.
7. Wait for the Pages build to finish. GitHub will show the website address in the Pages section. It usually looks like `https://YOUR-USERNAME.github.io/school-hq/`.
8. Open the website in Chrome. On a compatible device, use Chrome's install option or **Add to Home screen** to make it feel more like an app.

## Important limits in this first version
- Assignments, courses, resources, and degree settings save in the local storage of the browser profile you're using.
- Opening the website on another device will not automatically bring over the data. Use **Settings & backups → Export complete backup**, then import that JSON file on the other device. Keep backup files private.
- Do not add an API key or Airtable personal access token into `index.html`; browser code is visible to visitors.
- This version does not yet include login, cloud sync, direct LMS integrations, or notifications.

## Backups
Use **Settings & backups → Export complete backup (.json)** regularly. Store that backup somewhere private. Use **Import a backup (.json)** to restore the app's data in another browser. The CSV export contains assignments only.
