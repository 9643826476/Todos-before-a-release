## Better coordination & communication among our different platforms
- We need to make sure to coordinate among [☁ server](https://github.com/nextcloud/server/), [🤖 Android](https://github.com/nextcloud/android/), [🍏 iOS](https://github.com/nextcloud/ios/) & [💻 desktop](https://github.com/nextcloud/desktop/).
- New features should be centrally discussed in the [server repository](https://github.com/nextcloud/server/). (For example the updated share flow, or the QR code to sign in → they are all related to all platforms.)
- Get people from desktop and mobile involved directly because the web interface should follow patterns which apply to mobile & desktop too. @-mention [@nextcloud/desktop](https://github.com/orgs/nextcloud/teams/desktop/members) [@nextcloud/android](https://github.com/orgs/nextcloud/teams/android/members) [@nextcloud/ios](https://github.com/orgs/nextcloud/teams/ios/members)
- Mobile and desktop people can add the issue to their relevant project boards. (Issues can be assigned to multiple projects).
- We use issue tags "[client: 🤖🍏 mobile](https://github.com/nextcloud/server/labels/client%3A%20%F0%9F%A4%96%F0%9F%8D%8F%20mobile)" and "[client: 💻 desktop](https://github.com/nextcloud/server/labels/client%3A%20%F0%9F%92%BB%20desktop)" in the server repository these cross-platform issues.

## Cross-platform feature table
Currently important features to get to parity:

|Feature|Server|Desktop|iOS|Android|
|---|---|---|---|---|
|unified timeline per file (activity, comments, versions|•••|✘|✘|✔|
|comments|✔|✘|✘|✔|
|versions & restore|✔|✘|✘|✔|
|combined syncing & activity, for all files|/|✔|✘|✘|
|updated sharing design|✔|•••|•••|•••|
|add note to share|✔|✘|✘|✔|
|multiple share links|✔|✘|✘|✘|
|favorites, if possible sort up top|✔|✘|✔|✔|
|single "shares" entry|✔|/|✔|✘|

- ✔ = done
- ••• = in progress
- ✘ = to do
- / = not applicable

TODO:
- [x] Make the table into a markdown table and link the issues.
- [ ] If issues don’t exist for a point, create a central one in the server for central tracking (even if it’s already done in the server) as said above.