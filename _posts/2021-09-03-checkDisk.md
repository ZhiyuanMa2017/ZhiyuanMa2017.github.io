---
layout: post
title: macOS check hard drive status
tags:
  - script
  - shell
---
show all local snapshots:


```shell
tmutil listlocalsnapshots /
```

Delete all local snapshots:

```shell
for snapshot in $(tmutil listlocalsnapshotdates | grep -v :); do sudo tmutil deletelocalsnapshots $snapshot; done
```

Monitor and analyze hard drive health:

```shell
smartctl -a disk0
```


