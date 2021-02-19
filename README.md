Warning: do not use no english names in paths!

Local building for x86-64 (Host: Ubuntu 20.04 64 bit):
```
sudo snap install snapcraft --classic
snapcraft
```

Local building for arm64 (Host: Ubuntu 20.04 server 64 bit - https://ubuntu.com/download/raspberry-pi)
```
sudo snap install snapcraft
SNAPCRAFT_BUILD_ENVIRONMENT=host snapcraft
```

Install local build:
```
sudo snap install ponysay_3.0.3_amd64.snap --dangerous
```

Publishing:
```
snapcraft login
snapcraft push --release=stable ponysay_3.0.3_amd64.snap
```
