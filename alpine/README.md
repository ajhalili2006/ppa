# Package recipes for Alpine

## Usage for end-users

### Adding the repo

Currently packages are being built against the unstable releases (aka `edge`), so proceed with caution.
I'll consider building for at least 2 latest stable releases in the future once I afford paying for
VPS in Google Cloud or Azure, or even have a decent homelab for that (as seperate computer and not
just a VM within my current dual-boot setup).

```shell
wget https://mau.dev/andreijiroh.dev/dotfiles/-/raw/main/.abuild/releases@andreijiroh.eu.org.rsa.pub -O /etc/apk/keys/releases@andreijiroh.eu.org.rsa.pub
echo "https://pkgs.andreijiroh.eu.org/alpine/edge/stable" | tee -a /etc/apk/repositories
```

Frankly if you're here for the unstable releases of Tailscale built from sources:

```bash
echo "@ajhalili2006 https://pkgs.andreijiroh.eu.org/alpine/edge/unstable" | tee -a /etc/apk/repositories
apk add tailscale@ajhalili2006
```

### Release Tracks

There are three tracks available in the PPA:

* `stable` - Stable releases of different software
* `unstable` - Unstable releases, particularly built from development branch OR from
* `testing` - similar to `edge/testing` in the main aports repo
