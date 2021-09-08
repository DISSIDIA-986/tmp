ncdu /mnt/ramdisk
```bash
    1.8 GiB [ 35.4%]  rqlite.2
    1.8 GiB [ 35.4%]  rqlite.1
    1.5 GiB [ 29.1%]  rqlite.3
```
ncdu /root/node.1
```bash
  713.0 MiB [ 87.4%] /snapshots
  102.7 MiB [ 12.6%]  raft.db
```
ncdu /root/node.2
```bash
  740.4 MiB [ 86.1%] /snapshots
  119.3 MiB [ 13.9%]  raft.db
```
ncdu /root/node.3
```bash
  661.2 MiB [ 86.4%] /snapshots
  103.7 MiB [ 13.6%]  raft.db
```

![image](https://user-images.githubusercontent.com/7844261/132470085-7f14d485-7243-46f0-b686-93dd14f04a2c.png)

less +?rqlite /var/log/messages
```bash
Sep  8 15:37:32 test06 kernel: [11718]     0 11718  1865692  1111257    2452        0             0 rqlited
Sep  8 15:37:32 test06 kernel: [12893]     0 12893    38665      376      77        0             0 sshd
Sep  8 15:37:32 test06 kernel: [12895]     0 12895    28918      176      12        0             0 bash
Sep  8 15:37:32 test06 kernel: [13091]     0 13091  2714041  1605914    4319        0             0 rqlited
Sep  8 15:37:32 test06 kernel: Out of memory: Kill process 13091 (rqlited) score 190 or sacrifice child
Sep  8 15:37:32 test06 kernel: Killed process 13091 (rqlited) total-vm:10856164kB, anon-rss:6421440kB, file-rss:2020kB, shmem-rss:0kB
```
