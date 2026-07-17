<p align="center">
  <img src="./src-angular/assets/images/bridge-animation.gif"/>
</p>
<h3 align="center">A rhythm game chart searching and downloading tool.</h3>
<img align="center" src="./src-angular/assets/images/example.png"/>
<hr>

**Bridge** is a desktop application that allows you to search for, download, and manage charts for games like Clone Hero, YARG, etc.

This is the desktop version of [Chorus Encore](https://www.enchor.us/).

> This is a fork of [Geomitron/Bridge](https://github.com/Geomitron/Bridge) with an expanded local library manager (catalog scanning, video sync, art studio, and lyrics tooling) on top of the original search-and-download experience.

## Setup

Head over to the [Releases](https://github.com/joaoguilherme-devsec/Bridge/releases) page to download the install wizard. (Windows 10/11, Mac, and Linux versions are available)

## Features

### Search & download

- Find all charts that can be found on Chorus Encore.
- Download any chart directly into your chart library as a chart folder or `.sng` file.
- Multi-select songs to add to the download queue.
- Cancel and retry downloads.
- Advanced song search, with a "Quality Reviewed" filter for drum charts.
- Chart issue scanner (for people making charts).

### Library manager

- Scan one or more local folders into a searchable, filterable chart catalog (backed by a local SQLite database, with incremental rescans and duplicate detection).
- **Video Sync** — search and download YouTube/Vimeo/Dailymotion/Archive.org background videos for charts via `yt-dlp`, or import a local video file.
- **Art Studio** — fetch album art from iTunes and generate blurred/gradient background images for charts, individually or in batch.
- **Lyrics** — search LRCLIB for synced lyrics and inject them directly into `.chart` or `.mid` files.

### General

- In-app update checking and downloading.
- A variety of themes, including custom theme support.

See the [Releases](https://github.com/joaoguilherme-devsec/Bridge/releases) page for the full changelog.

## Development

Built using Node.js, Angular, and Electron.

Learn how to install Node.js [here](https://nodejs.dev/en/download/)

After installing Node.js and cloning the repository, install dependencies and run development with:

```
$ npm install && npm start
```

Video Sync and Art Studio's background generation rely on [`yt-dlp`](https://github.com/yt-dlp/yt-dlp) and `ffmpeg` being available on your `PATH`.

Other useful scripts (see `package.json` for the full list):

- `npm run build:windows` / `build:mac` / `build:linux` — build a production installer for the current platform.
- `npm run release` — build production installers for all platforms.

## License

Bridge is licensed under [GPL-3.0](./LICENSE).

## Socials

To discuss the project and make suggestions, please join the [Discord](https://discord.gg/cqaUXGm)

To help pay for the server costs of the original Chorus Encore project, please check out the [Patreon](https://www.patreon.com/ChorusEncore701)
