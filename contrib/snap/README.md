# Patriotcoin Snap Packaging

Commands for building and uploading a Patriotcoin Core Snap to the Snap Store. Anyone on amd64 (x86_64), arm64 (aarch64), or i386 (i686) should be able to build it themselves with these instructions. This would pull the official Patriotcoin binaries from the releases page, verify them, and install them on a user's machine.

## Building Locally
```
sudo apt install snapd
sudo snap install --classic snapcraft
sudo snapcraft
```

### Installing Locally
```
snap install \*.snap --devmode
```

### To Upload to the Snap Store
```
snapcraft login
snapcraft register patriotcoin-core
snapcraft upload \*.snap
sudo snap install patriotcoin-core
```

### Usage
```
patriotcoin-unofficial.cli # for patriotcoin-cli
patriotcoin-unofficial.d # for patriotcoind
patriotcoin-unofficial.qt # for patriotcoin-qt
patriotcoin-unofficial.test # for test_patriotcoin
patriotcoin-unofficial.tx # for patriotcoin-tx
```

### Uninstalling
```
sudo snap remove patriotcoin-unofficial
```