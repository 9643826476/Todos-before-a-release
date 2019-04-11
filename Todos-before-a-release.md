Check list for a release (copy it to a ticket and then tick of the checkboxes):

```
# RC phase (up to one week before the release date)

* [ ] get all the pending backports merged to the stable branches ([check the milestones accross the organisation](https://github.com/issues?utf8=✓&q=is%3Aopen+user%3Anextcloud+archived%3Afalse+milestone%3A%22Nextcloud+13.0.2%22+))
* [ ] sent customer newsletter with security and release date information
* [ ] create the RC packages
* [ ] upload the RC packages to the `/server/prereleases` folder of the download server
* [ ] update the beta channel of the [updater_server](https://github.com/nextcloud/updater_server)
* [ ] test the updater_server on the internal URL (`https://updates.nextcloud.com/internal_updater_server/`)
* [ ] ask in the forums for help (use the [changelog generator script](https://github.com/nextcloud/github_helper#changelog-generator))
* [ ] prepare "What's new" server - [Example](https://github.com/nextcloud/changelog_server/pull/5)

# Release (~1 day before the planned release)

* [ ] prepare blog post, newsletter, social media messages (check the changelog for interesting features/fixes and possible screenshots)
* [ ] update the changelog on the website (use the [changelog generator script](https://github.com/nextcloud/github_helper#changelog-generator))
* [ ] update version number on website (in `strings.php`)
* [ ] update version number in documentation (in `admin_manual/release_schedule.rst`)
* [ ] create the final packages
* [ ] upload the final packages to `/server/prereleases` folder of the download server

## T - 30 minutes

* [ ] copy the final packages to `/server/releases` folder of the download server
* [ ] update the stable channel of the [updater_server](https://github.com/nextcloud/updater_server)
* [ ] test the updater_server on the internal URL (`https://updates.nextcloud.com/internal_updater_server/`)
* [ ] merge the website PR
* [ ] deploy the website PR (maybe update caches)
* [ ] update [wiki page](https://github.com/nextcloud/server/wiki/Maintenance-and-Release-Schedule)

## T

* [ ] publish blog posts
* [ ] send newsletter
* [ ] post on social media

# Post processing (non-coding)

* [ ] update the milestones in all repos (use the [milestone updater](https://github.com/nextcloud/github_helper/tree/master/milestoneupdater) for this)
* [ ] update app store releases (see [documentation](https://nextcloudappstore.readthedocs.io/en/latest/prodinstall.html#sync-nextcloud-releases-from-github))
* [ ] update user content proxy of app store (see https://github.com/nextcloud/usercontent.apps.nextcloud.com)
* [ ] update security scanner
* [ ] update owncloud-migration config on update server
* [ ] update install page on website
* [ ] update installer script on download server (see [repo](https://github.com/nextcloud/web-installer))
* [ ] check wikipedia pages for release information - update pages if necessary
* [ ] check wikimedia content for outdated media e.g. screenshots
```