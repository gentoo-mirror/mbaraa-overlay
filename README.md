# mbaraa-overlay

My personal Gentoo Overlay repo, contains the following:

- app-portage/eloi
- app-misc/dotsync

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
