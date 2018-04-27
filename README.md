# Contributing

If you want to contribute, any help is appreciated! 

- Fork the repository
- Create a feature branch to work in
- Make your changes on the created branch (new feature or bugfixes)
- Send a pull request and we will review it

# Branching and release management

For branching we use the GitFlow (see http://nvie.com/posts/a-successful-git-branching-model/). We use the following branches

- feature-*
  - new features or bug fixes for the coming release
- dev
  - after the feature branch is completed it is merged through a pull request in the dev branch
- master
  - used for completed releases. Must be merged through a release branch. Release are created on the master branch commits
- release-[version] or release/[version]
  - created when the release is almost finished and only testing is done. Only bug fixes are allowed on this branch. After completion it is merged into master and dev branch and deleted after merging.
- hotfix-[version] or hotfix/[version]
  - when critical bugfixing must be done on a release that is shipped. Should be merged into master and deleted after merging.

For versioning we use GitVersion (see http://gitversion.readthedocs.io/en/latest/). Based on the above branches GitVersion determines the version number. 

NuGet packages for all branches are published to our myget feed (https://www.myget.org/F/xerproject/api/v3/index.json). Tags are published to the official NuGet feeds. 
