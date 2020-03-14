Warning: do not use no english names in paths!

Build for x86-64 (Host: Ubuntu 18.04 64 bit):
```
sudo snap install snapcraft --classic
snapcraft
```

Build for arm64 (Host: Ubuntu 18.04 server 64 bit - https://ubuntu.com/download/iot/raspberry-pi-2-3)
```
sudo snap install snapcraft
SNAPCRAFT_BUILD_ENVIRONMENT=host snapcraft
```

Check build:
```
sudo snap install ponysay_3.0.3_amd64.snap --dangerous
```

Publishing:
```
snapcraft login
snapcraft push --release=stable ponysay_3.0.3_amd64.snap
```
