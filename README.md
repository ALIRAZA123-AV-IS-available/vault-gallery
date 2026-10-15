# Vault Gallery — Pattern-Lock Media Gallery

A browser-based image and video gallery with a pattern-lock interface, local media storage, albums, Trash recovery, and backup/restore tools. Built with HTML, CSS, and vanilla JavaScript.

- **Live Demo:** https://ALIRAZA123-AV-IS-available.github.io/vault-gallery/
- **Source Code:** https://github.com/ALIRAZA123-AV-IS-available/vault-gallery

## About the Project

Vault Gallery is a front-end web application for organizing personal photos and videos in a browser. It combines a pattern-based lock screen with gallery tools such as search, sorting, favourites, albums, and recovery from Trash.

The app stores media in the current browser profile rather than uploading it to a server. It is a portfolio and learning project, not an encrypted or production-grade secure vault.

## Features

### Lock Screen and Preferences
- Pattern-based setup and unlock interface.
- Supported pattern/grid style options.
- Theme preferences, including light and dark appearance.
- Auto-lock settings.

### Media Gallery
- Upload and view supported image and video files.
- Search, filter, and sort gallery items.
- Mark items as favourites.
- Switch supported gallery view modes.
- Preview, rename, and download media.
- Select multiple items for supported bulk actions.

### Albums and Trash
- Create, rename, and delete albums.
- Add files to multiple albums without duplicating the media.
- Remove items from an album while keeping them in the main gallery.
- Move items to Trash, restore them, or permanently delete them.

### Backup and Storage
- Store media locally in IndexedDB.
- Store preferences and lock-related metadata in Local Storage.
- View library/storage information in the app.
- Export and restore library backups using ZIP files.
- Support for checksums and multipart backups in the backup workflow.

> **Important:** Backups are not encrypted. Keep backup files somewhere private and maintain another copy of important media.

## Technologies Used

- HTML5
- CSS3
- Vanilla JavaScript
- IndexedDB
- Local Storage
- Browser File APIs
- ZIP-based backup/restore
- GitHub Pages

## Getting Started

### Run Locally

1. Clone or download this repository.
2. Open `index.html` in a modern browser.
3. Complete the initial setup and create a pattern.
4. Unlock the gallery and upload supported media.

For the best compatibility, run the app through HTTPS (such as GitHub Pages) or `http://localhost` instead of opening it directly through `file://`.

### Deploy with GitHub Pages

1. Push `index.html` and `README.md` to your repository.
2. Open the repository's **Settings → Pages**.
3. Select the publishing branch and folder (commonly `main` and `/root`).
4. Wait for GitHub Pages to finish deploying.
5. Open the live demo link at the top of this README.

## Storage and Security

Vault Gallery is designed for local, browser-based use:

- Images and videos are stored in IndexedDB for the current browser profile on the current device.
- Preferences and lock-related metadata are stored in Local Storage.
- The application does not provide server-side accounts or cloud synchronization.
- Clearing site/browser data, changing browser profiles, or using another device may make the local library unavailable.
- Backups should be stored securely and kept separate from the browser's local copy.

**Security Limitation:** The pattern lock is an interface-level privacy feature, not strong authentication. Media files and exported ZIP backups are not encrypted by this application. Someone with access to the browser profile or developer tools may be able to access local data. Do not rely on Vault Gallery to protect highly sensitive files.

## Screenshots

Add screenshots of the current version here so visitors can see the interface before opening the demo.

Suggested files:
- `screenshots/pattern-lock.png`
- `screenshots/media-gallery.png`
- `screenshots/albums-and-trash.png`
- `screenshots/settings-and-backup.png`
- `screenshots/mobile-layout.png`

When you add the screenshots to the repository, you can display them with Markdown, for example:

```md
![Vault Gallery pattern lock](screenshots/pattern-lock.png)
![Vault Gallery media gallery](screenshots/media-gallery.png)
![Vault Gallery settings](screenshots/settings-and-backup.png)
```

## Manual Testing Checklist

Before describing the app as fully tested or production-ready, check these flows in desktop and mobile browsers:

- [ ] Complete first-time setup and unlock with the correct pattern.
- [ ] Confirm an incorrect pattern is handled as expected.
- [ ] Upload multiple images and videos.
- [ ] Refresh the page and verify that the library persists.
- [ ] Search, filter, sort, favourite, preview, rename, and download items.
- [ ] Create, rename, and delete albums.
- [ ] Add files to multiple albums and confirm files are not duplicated.
- [ ] Move items to Trash, restore them, and permanently delete them.
- [ ] Create a backup and restore it in a test browser/profile.
- [ ] Test checksum handling and multipart backup/restore flows.
- [ ] Test theme settings and auto-lock.
- [ ] Check the layout at mobile screen widths.
- [ ] Check behavior when storage is unavailable or nearly full.

## Future Improvements

Potential next steps include:

- Add screenshots and a short demo video.
- Conduct broader browser and mobile testing.
- Improve accessibility and keyboard navigation.
- Consider optional encryption for local data and backups.
- Add automated tests for critical storage and restore flows.

## Author

**Ali Raza**

Developed as a web development portfolio project to practise front-end development, browser storage, and interactive user-interface design.

## License

No license is currently specified. Add an open-source license if you want to define how others may reuse, modify, or distribute this project.
