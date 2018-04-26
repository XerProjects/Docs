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
- release/[version]
  - created when the release is almost finished and only testing is done. Only bug fixes are allowed on this branch. After completion it it merged into master and dev branch and deleted after master.
- hotfix-[version]
  - when critical bugfixing must be done on a release that is shipped. Should be merged into master and deleted after merging.
