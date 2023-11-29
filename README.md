# ~ajhalili2006's packaging recipes (mostly for Alpine Linux)

Collection of build scripts for different packages, mostly before being proposed to distribution for official package maintainership.

## Disclaimer - READ ME FIRST!

My personal package repository and its corresponding packaging recipe sources here are provided AS IS, without warranty of any kind.
If things break, I'm not responsible for it, although bug reports are welcome as long as it is details.[^2]

[^2]: Do not annoy upstream maintainers if the package here break. File it here first.

If your project, community or company is relying on my package repositories for your systems (or even for your containers), I may not have the enough bandwith to:

* timely apply security and feature updates and rebuild them
* build packages against all archeitures since I only build for `x86_64`/`amd64`[^1]
* apply backport fixes to older versions of Linux distributions

[^1]: If you want to help with the CI infrastructure, please reach out to me at <https://andreijiroh.eu.org/contact/open-source>.

While this repository will be remain open for anyone to build on their own and to make CI/CD work flawlessly without passing around SSH keys,
this is more of a personal project where I learn the pain points of software distribution and packaging to different distributions.

## Packaging recipes

More to come soon.

* [`alpine`](./alpine/) - Recipes for Alpine Linux
* `debian` - Recipes for Debian
    * `ubuntu` - Same for Ubuntu, but may contain distro-specific changes

## License

The packaging recipes in this repository mostly follow upstream's license, alongside MPL-2.0
for the APKBUILDs and other patches.
