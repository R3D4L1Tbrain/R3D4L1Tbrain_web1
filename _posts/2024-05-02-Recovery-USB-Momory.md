---
layout: single
title: Recovery USB Memory
excerpt: "this is the archive to recovery usb memory"
date: 2024-05-02
classes: wide
headers: 
 - teaser: /assets/images/usb.jpg
 - teaser_home_page: true
categories:
 - Configuration
 - recovery
tags:
 - Hardware	
---


 ![](/assets/images/usb.jpg)


# CMD  Windows

1. Enter memory.
2. start `cmd`
3. execute
```shell
start Diskpart
```

```shell
list disk
```

4. enter number of the memory entered, differentiate by size   
```shell
select disk 1  
```

5. clear memory
```shell
clean
```

>[!note] 
> reset from memory creation (**all data will be lost**)

6. create new partition 
```shell
create partition Primary
```

7. show all partitions 
```
list pantition 
```

8. active the partition 
```shell
active
```

9. finally assigning a format
```shell
format fs=NTFS label="" quick
```




