---
title: Docs - Flynn
layout: docs
---

# Contribution Guide

We welcome and encourage community contributions to Flynn.

Since the project is still unstable, there are specific priorities for development. Pull requests that do not address these priorities will not be accepted until Flynn is production ready.

Please familiarize yourself with the Contribution Guidelines and Project Roadmap before contributing.

There are many ways to help Flynn besides contributing code:

 - Fix bugs or file issues
 - Improve the [documentation](https://github.com/flynn/flynn.io) including this website
 - [Contribute](https://flynn.io/#sponsor) financially to support core development

## Contributing Code

Unless you are fixing a known bug, we **strongly** recommend discussing it with the core team via a GitHub issue, [IRC](irc://irc.freenode.net/flynn), or [email](mailto:contact@flynn.io) before getting started to ensure your work is consistent with Flynn's roadmap and architecture.

All contributions are made via pull request. Note that **all patches from all contributors get reviewed**. After a pull request is made other contributors will offer feedback, and if the patch passes review a maintainer will accept it with a comment. When pull requests fail testing, authors are expected to update their pull requests to address the failures until the tests pass and the pull request merges successfully.

At least one review from a maintainer is required for all patches (even patches from other maintainers). If only one maintainer is listed in the MAINTAINERS file, then review is not required for patches from the sole maintainer (however it is encouraged).

Maintainers must demonstrate a consistent track record of recent contributions, as repos with only two maintainers can bottleneck easily due to the review requirements. Only active contributors and reviewers will remain maintainers. Changes in maintainership shouldn't be taken personally, they are purely organizational and for the health of the code and project.


## Developer’s Certificate of Origin

All contributions must include acceptance of the DCO:

```text
Developer Certificate of Origin
Version 1.1

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
660 York Street, Suite 102,
San Francisco, CA 94110 USA

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.


Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```

To accept the DCO, simply add this line to each commit message with your name and email address (`git commit -s` will do this for you):

```text
Signed-off-by: John Doe <john@example.com>
```

For legal reasons, no anonymous or pseudonymous contributions are accepted ([contact us](mailto:contact@flynn.io) if this is an issue).

## Pull request procedure

To make a pull request, you will need a Github account; if you're unclear on this process, see Github's documentation on [forking](https://help.github.com/articles/fork-a-repo) and [pull requests](https://help.github.com/articles/using-pull-requests). Pull requests should be targeted at the `master` branch. Before creating a pull request, go through this checklist:

1. Create a feature branch off of `master` so that changes don't get mixed up.
1. [Rebase](http://git-scm.com/book/en/Git-Branching-Rebasing) your local changes against the `master` branch.
1. Run the full project test suite with the `go test ./...` (or equivalent) command and confirm that it passes.
1. Run `gofmt -s` (if the project is written in Go).
1. Accept the Developer's Certificate of Origin on all commits (see above).

Pull requests will be treated as "review requests", and maintainers will give feedback on the style and substance of the patch.

Normally, all pull requests must include tests that test your change. Occasionally, a change will be very difficult to test for. In those cases, please include a note in your commit message explaining why.

## Communication

There is an IRC channel on chat.freenode.net, channel #flynn. You're welcome to drop in and ask questions, discuss bugs, etc. It is [logged on BotBot.me](https://botbot.me/freenode/flynn/).

## Conduct

Whether you're a regular contributor or a newcomer, we care about making this community a safe place for you and we've got your back.

* We are committed to providing a friendly, safe and welcoming environment for all, regardless of gender, sexual orientation, disability, ethnicity, religion, or similar personal characteristic.
* Please avoid using nicknames that might detract from a friendly, safe and welcoming environment for all.
* Be kind and courteous. There's no need to be mean or rude.
* We will exclude you from interaction if you insult, demean or harass anyone. In particular, we don't tolerate behavior that excludes people in socially marginalized groups.
* Private harassment is also unacceptable. No matter who you are, if you feel you have been or are being harassed or made uncomfortable by a community member, please contact one of the channel ops or a member of the Flynn core team immediately.
* Likewise any spamming, trolling, flaming, baiting or other attention-stealing behaviour is not welcome.

We welcome discussion about creating a welcoming, safe, and productive environment for the community. If you have any questions, feedback, or concerns [please let us know](mailto:contact@flynn.io).

