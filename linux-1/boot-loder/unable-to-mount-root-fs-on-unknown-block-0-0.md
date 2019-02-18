# unable to mount root fs on unknown-block\(0 0\)

මගේ main os \(debian testing\) එකට අමතරව මං deepin 15.9 පාවිච්චි කරනවා එකේ අවුලක් ගියොත් එක fix කරගන්න , ඉතින් මං ඊයේ එක manjaro deepin 18.2 වලින් ප්‍රතිස්ථාපනය කලා . මං first boot එක කරන කොට මට මෙහෙම erro එකක් අවා.

![\[    0.243925\] Kernel panic - not syncing: VFS: Unable to mount root fs on unknown-block\(0,0\) \[    0.243949\] CPU: 1 PID: 1 Comm: swapper/0 Not tainted 4.15.5-1-ARCH \#1 \[    0.243965\] Hardware name: Gigabyte Technology Co., Ltd. Z270N-WIFI/Z270N-WIFI-CF, BIOS F5 07/06/2017 \[    0.243987\] Call Trace: \[    0.243998\]  dump\_stack+0x5c/0x85 \[    0.244009\]  panic\_0xe4/0x252 \[    0.244020\]  mount\_block\_root+0x27f/0x2e0 \[    0.244033\]  ? set\_debug\_rodata+0x11/0x11 \[    0.244044\]  prepare\_namespace+0x130/0x166 \[    0.244056\]  kernel\_init\_freable+0x1e6/0x1f3 \[    0.244068\]  ? reset\_init+0xd0/0xd0 \[    0.244078\]  kernet\_init+0xa/0x100 \[    0.244088\]  ret\_from\_fork+0x35/0x40 \[    0.244113\] Kernel Offset: 0xd000000 from 0xffffffff81000000 \(relocation range: 0xffffffff80000000-0xffffffffbfffffff\) \[    0.244139\] ---\[ end Kernel panic - not syncing: VFS: Unable to mount root fs on unknown-block\(0,0\)](../../.gitbook/assets/image.png)

මං boot loder එක විදියට පාවිච්චි කරන්නේ main os එකේ boot loder එක . ඉතින් අවුල තිබිලා තියෙන්නේ main os එකේ /boot/grub/grub.cfg එකේ. මං ඉතිං එක fix කරගත්තේ main os එකේ /boot/grub/grub.cfg එකට එකේ manjaro grub.cfg එකක් line එකක් දාල. පලහල එකක් ඇති කරන් විදිය දාපු.

{% embed url="https://www.youtube.com/watch?v=QtgF1Kc\_M1s" %}

ගන්න එපා පුතුගාල් වෙලාවක් නැ ඔක්කොම ලියන්න.

