# Debian Packaging Commands

# Creating and updating pbuilder
- git-pbuilder create
- sudo cowbuilder --update

# Updating
- gbp import-orig --uscan
- gbp import-dsc /path/to/package_version.dsc

# Building
- gbp buildpackage --git-pbuilder --git-ignore-new
- gbp buildpackage --git-pbuilder --git-pbuilder-options=--source-only-changes
- gbp tag

# Pushing changes
- git push
- git push -u origin --tags

# Uploading packages
- debsign package_version_source.changes
- dput ftp-master package_version_source.changes

# Useful links
- https://wiki.debian.org/PackagingWithGit
- https://wiki.debian.org/Packaging/Intro
