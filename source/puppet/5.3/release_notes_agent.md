---
layout: default
title: "Puppet agent release notes"
---

[Puppet 5.0.0]: /puppet/5.0/release_notes.html#puppet-500
[Puppet 5.1.0]: /puppet/5.1/release_notes.html#puppet-510
[Puppet 5.2.0]: /puppet/5.2/release_notes.html#puppet-520
[Puppet 5.3.1]: /puppet/5.2/release_notes.html#puppet-531

[Facter 3.9.0]: /facter/3.9/release_notes.html#facter-390
[Facter 3.9.2]: /facter/3.9/release_notes.html#facter-392

[MCollective 2.11.2]: /mcollective/releasenotes.html#2_11_2
[MCollective 2.11.3]: /mcollective/releasenotes.html#2_11_3

[pxp-agent]: https://github.com/puppetlabs/pxp-agent

This page lists changes to the `puppet-agent` package. For details about changes to components in a `puppet-agent` release, follow the links to those components in the package release's notes.

The `puppet-agent` package's version numbers use the format X.Y.Z, where:

-   X must increase for major backward-incompatible changes
-   Y may increase for backward-compatible new functionality
-   Z may increase for bug fixes

The `puppet-agent` package installs the latest version of Puppet 5.

Also of interest: [About Agent](./about_agent.html), and the [Puppet 5.2.0][], [Puppet 5.1.0][], and [Puppet 5.0.0][] release notes.

## Puppet agent 5.3.1

Released October 2, 2017.

This is a feature and bug-fix release of Puppet Platform that also adds new operating system packages. There was no packaged release of Puppet agent 5.3.0; version 5.3.1 is the first packaged release of the 5.3.x series.

### Component updates

This release includes component updates to [Puppet 5.3.1][], [Facter 3.9.2][], [MCollective 2.11.3][], and [pxp-agent][] 1.8.0.

### Platform updates

This release adds packages for Fedora 26, and for SLES 12 on POWER architectures. It also removes packages for Fedora 24, which [entered end-of-life status on August 8, 2017](https://fedoraproject.org/wiki/End_of_life).
