# plappa

plappa is an audiobook player/client for [Jellyfin, the free software media system](https://jellyfin.org) and [AudioBookShelf](https://www.audiobookshelf.org/), written in Swift/SwiftUI.
<br><a target="_blank" href='https://apps.apple.com/us/app/plappa/id6475201956'>
    <img alt='Get plappa on the App Store' src='images/AppStoreBadge.svg' height="60" />
</a><br/>
Apart from playing audiobooks, plappa also syncs playback status via iCloud and allows you to download audiobooks for offline listening.

It currently runs on iPhone and iPad, a Mac and Apple TV version are planned ([see the roadmap](#roadmap)).

![Showcase of plappa ui](images/Thumb-4.webp)

## About

plappa requires a Jellyfin or AudioBookShelf Server to work. If you don't know Jellyfin or AudioBookShelf and would like to learn more, check out both at [Jellyfin website](https://jellyfin.org) or [Jellyfin GitHub repo](https://github.com/jellyfin/jellyfin) and [AudioBookShelf website](https://www.audiobookshelf.org/) or [AudioBookShelf GitHub repo](https://github.com/advplyr/audiobookshelf).

### Folder structure and formats for Jellyfin

plappa should be able to handle all common audio file formats, but is built for and tested mainly with MP3 and M4B files.

I always test plappa using the [most common organization scheme for books](https://jellyfin.org/docs/general/server/media/books/), but other folder structures should work fine, plappa just searches for audio files recoursively, grouping by album.

### Metadata

Most metadata will be taken from Jellyfin/AudioBookShelf, plappa additionally reads the `composer` field for the narrator name and (if applicable) chapters from the file metadata.

## Roadmap

You can see the full roadmap in the [plappa project](https://github.com/users/LeoKlaus/projects/7/views/2), the short version is:

- [x] iOS App with all basic features
- [x] Carplay support (WIP)
- [ ] Apple Watch App
- [ ] Mac App
- [ ] Apple TV App
- [x] Support for [AudioBookShelf servers](https://www.audiobookshelf.org/) (WIP)


## Feedback

### Bug reports

If you encounter any issues while using plappa, please [create an issue here on GitHub](https://github.com/LeoKlaus/plappa/issues/new/choose).
Follow the guidelines for creating an issue and provide as much information as possible without revealing any personal data. Please check if a bug has already been reported before creating a new issue.

### Feature requests

Feature requests are managed in [the discussion section of this repo](https://github.com/LeoKlaus/plappa/discussions). You can create feature requests and vote on other ideas [here](https://github.com/LeoKlaus/plappa/discussions/new/choose). Please check if a similar feature has been requested before and vote on that instead of creating a duplicate.
