# mbaraa-overlay

My personal Gentoo Overlay repo, contains the following:

- **app-portage/eloi**

  - Gentoo's eix with extra steps, an AUR-like package manager for Gentoo.
  - [https://github.com/mbaraa/eloi](https://github.com/mbaraa/eloi)

- **app-misc/dotsync**
  - Dotfiles synchronizer thingy.
  - [https://github.com/mbaraa/dotsync](https://github.com/mbaraa/dotsync)

# Installation

1. Create the overlay's metadata file `/etc/portage/repos.conf/mbaraa.conf`
2. Add the overlay's metadata to the created file

```
[mbaraa-overlay]
location = /var/db/repos/mbaraa-overlay
sync-type = git
sync-uri = https://github.com/mbaraa/gentoo-overlay.git
```

3. Sync the new overlay

```bash
; emerge --sync mbraraa-overlay
```
