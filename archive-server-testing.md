# Archive server testing

Miroor server එකක් කියන්නේ server එකක තියෙන site හරි නැත්නුම files හරි copy කරල තියෙන server එකක් ඉතින් mirror server නිසා එකම site එක හරි files හරි හුගක් තැන වලින් ගන්න පුලුවම් . Mirror server වලට එයාලටම කියලා URL එකක් තියෙනවා.

~ [searchstorage.techtarget.com/definition/mirror](https://searchstorage.techtarget.com/definition/mirror)

Linux users ලට software install කරන්න ඔනි repo host කරල තියෙන්නෙ මෙන්න මෙ වගෙ mirrors ව්ල.

Mirro server වලින් අපිට තියෙන වාසිය තම්යි එවා අපිට ලන් වෙන්තර්ම්ට අපිට එවා ව්ලින් files download කරන්න පුලුව්ම් වෙගෙ වෑඩිවෙන්ව.ඉතින් අපිට ලග mirrors ගොඩක තිබුනහම අපිට වෑඩිම වෙගයෙන download කරලන්න පුලුව්ම server එක හොයගන්න තියෙන හොඩම විඩිය තම ping කරල බලන එක.

&lt;----Kali archive test----&gt;

> ┌─\[ebony@blackmagic\]─\[~\]
>
> └──╼ $ping -c 10 mirrors.ustc.edu.cn && ping -c 10 mirrors.aliyun.com && ping -c 10 mirrors.tuna.tsinghua.edu.cn && ping -c 10 mirrors.ustc.edu.cn && ping -c 10 mirrors.ustc.edu.cn && ping -c 10 mirrors.zju.edu.cn && ping -c 10 mirrors.neusoft.edu.cn && ping -c 10 http.kali.org
>
> PING mirrors.ustc.edu.cn \(202.141.176.110\) 56\(84\) bytes of data.
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=1 ttl=43 time=430 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=2 ttl=43 time=429 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=3 ttl=43 time=429 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=4 ttl=43 time=429 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=5 ttl=43 time=428 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=6 ttl=43 time=429 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=7 ttl=43 time=436 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=8 ttl=43 time=430 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=9 ttl=43 time=437 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=10 ttl=43 time=430 ms
>
> --- mirrors.ustc.edu.cn ping statistics ---
>
> 10 packets transmitted, 10 received, 0% packet loss, time 10ms
>
> rtt min/avg/max/mdev = 428.434/430.597/436.564/3.099 ms
>
> PING mirrors.aliyun.com.w.alikunlun.com \(47.246.1.47\) 56\(84\) bytes of data.
>
> 64 bytes from 47.246.1.47: icmp\_seq=1 ttl=49 time=65.8 ms
>
> 64 bytes from 47.246.1.47: icmp\_seq=2 ttl=49 time=65.3 ms
>
> 64 bytes from 47.246.1.47: icmp\_seq=3 ttl=49 time=65.8 ms
>
> 64 bytes from 47.246.1.47: icmp\_seq=4 ttl=49 time=65.9 ms
>
> 64 bytes from 47.246.1.47: icmp\_seq=5 ttl=49 time=65.9 ms
>
> 64 bytes from 47.246.1.47: icmp\_seq=6 ttl=49 time=65.9 ms
>
> 64 bytes from 47.246.1.47: icmp\_seq=7 ttl=49 time=66.3 ms
>
> 64 bytes from 47.246.1.47: icmp\_seq=8 ttl=49 time=66.8 ms
>
> 64 bytes from 47.246.1.47: icmp\_seq=9 ttl=49 time=71.4 ms
>
> 64 bytes from 47.246.1.47: icmp\_seq=10 ttl=49 time=65.6 ms
>
> --- mirrors.aliyun.com.w.alikunlun.com ping statistics ---
>
> 10 packets transmitted, 10 received, 0% packet loss, time 686ms
>
> rtt min/avg/max/mdev = 65.327/66.472/71.366/1.704 ms
>
> PING cdnmirrors.s.tuna.tsinghua.edu.cn \(101.6.8.193\) 56\(84\) bytes of data.
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=1 ttl=231 time=456 ms
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=2 ttl=231 time=435 ms
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=3 ttl=231 time=440 ms
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=4 ttl=231 time=439 ms
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=5 ttl=231 time=443 ms
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=6 ttl=231 time=446 ms
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=7 ttl=231 time=441 ms
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=8 ttl=231 time=447 ms
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=9 ttl=231 time=447 ms
>
> 64 bytes from 101.6.8.193 \(101.6.8.193\): icmp\_seq=10 ttl=231 time=466 ms
>
> --- cdnmirrors.s.tuna.tsinghua.edu.cn ping statistics ---
>
> 10 packets transmitted, 10 received, 0% packet loss, time 1006ms
>
> rtt min/avg/max/mdev = 434.862/445.896/466.051/8.659 ms
>
> PING mirrors.ustc.edu.cn \(218.104.71.170\) 56\(84\) bytes of data.
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=1 ttl=47 time=438 ms
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=2 ttl=47 time=437 ms
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=3 ttl=47 time=435 ms
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=4 ttl=47 time=435 ms
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=5 ttl=47 time=435 ms
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=6 ttl=47 time=435 ms
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=7 ttl=47 time=436 ms
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=8 ttl=47 time=441 ms
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=9 ttl=47 time=440 ms
>
> 64 bytes from 170.71.104.218.adsl-pool.ah.cnuninet.net \(218.104.71.170\): icmp\_seq=10 ttl=47 time=438 ms
>
> --- mirrors.ustc.edu.cn ping statistics ---
>
> 10 packets transmitted, 10 received, 0% packet loss, time 20ms
>
> rtt min/avg/max/mdev = 434.837/437.151/440.841/2.010 ms
>
> PING mirrors.ustc.edu.cn \(202.141.176.110\) 56\(84\) bytes of data.
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=1 ttl=43 time=431 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=2 ttl=43 time=435 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=3 ttl=43 time=429 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=4 ttl=43 time=430 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=5 ttl=43 time=428 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=6 ttl=43 time=434 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=7 ttl=43 time=434 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=8 ttl=43 time=430 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=9 ttl=43 time=429 ms
>
> 64 bytes from mirrors.ustc.edu.cn \(202.141.176.110\): icmp\_seq=10 ttl=43 time=430 ms
>
> --- mirrors.ustc.edu.cn ping statistics ---
>
> 10 packets transmitted, 10 received, 0% packet loss, time 1007ms
>
> rtt min/avg/max/mdev = 428.112/430.988/434.781/2.309 ms
>
> PING mirrors.zju.edu.cn \(210.32.158.231\) 56\(84\) bytes of data.
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=1 ttl=34 time=501 ms
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=2 ttl=34 time=500 ms
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=3 ttl=34 time=496 ms
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=4 ttl=34 time=497 ms
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=5 ttl=34 time=482 ms
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=6 ttl=34 time=484 ms
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=7 ttl=34 time=476 ms
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=8 ttl=34 time=474 ms
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=9 ttl=34 time=473 ms
>
> 64 bytes from 210.32.158.231 \(210.32.158.231\): icmp\_seq=10 ttl=34 time=481 ms
>
> --- mirrors.zju.edu.cn ping statistics ---
>
> 10 packets transmitted, 10 received, 0% packet loss, time 211ms
>
> rtt min/avg/max/mdev = 473.449/486.397/501.143/10.481 ms
>
> PING mirrors.neusoft.edu.cn \(219.216.128.25\) 56\(84\) bytes of data.
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=1 ttl=39 time=498 ms
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=2 ttl=39 time=524 ms
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=3 ttl=39 time=548 ms
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=4 ttl=39 time=499 ms
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=5 ttl=39 time=498 ms
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=6 ttl=39 time=497 ms
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=7 ttl=39 time=498 ms
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=8 ttl=39 time=497 ms
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=9 ttl=39 time=498 ms
>
> 64 bytes from 219.216.128.25 \(219.216.128.25\): icmp\_seq=10 ttl=39 time=504 ms
>
> --- mirrors.neusoft.edu.cn ping statistics ---
>
> 10 packets transmitted, 10 received, 0% packet loss, time 10ms
>
> rtt min/avg/max/mdev = 496.866/506.099/548.256/16.128 ms
>
> PING hebe.kali.org \(192.99.200.113\) 56\(84\) bytes of data.
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=1 ttl=54 time=241 ms
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=2 ttl=54 time=250 ms
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=3 ttl=54 time=238 ms
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=4 ttl=54 time=241 ms
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=5 ttl=54 time=240 ms
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=6 ttl=54 time=239 ms
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=7 ttl=54 time=239 ms
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=8 ttl=54 time=239 ms
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=9 ttl=54 time=239 ms
>
> 64 bytes from hebe.kali.org \(192.99.200.113\): icmp\_seq=10 ttl=54 time=239 ms
>
> --- hebe.kali.org ping statistics ---
>
> 10 packets transmitted, 10 received, 0% packet loss, time 19ms
>
> rtt min/avg/max/mdev = 238.145/240.410/249.816/3.364 ms

Kali ව්ලට හොඩම තියෙන්නෙ China & Singapore ව්ල \(rr කරයන්ව ගන්නෙ නෑ\). China mirror ව්ලින් ping කලහම අඩුම average time එකක් තියෙන්නෙ mirrors.aliyun.com.w.alikunlun.com එක්ට ; ඉතින් මන එක මාගේ sources.list එක ගත්තා.

&gt;--------Kali sources list-------&lt;

`# deb cdrom:[Debian GNU/Linux 2018.3 _Kali-rolling_ - Official Snapshot amd64 LIVE/INSTALL Binary 20180911-17:58]/ kali-last-$`

`#deb cdrom:[Debian GNU/Linux 2018.3 _Kali-rolling_ - Official Snapshot amd64 LIVE/INSTALL Binary 20180911-17:58]/ kali-last-s$`

`#阿里云`

`deb`[`http://mirrors.aliyun.com/kali`](http://mirrors.aliyun.com/kali)`kali-rolling main non-free contrib`

`deb-src`[`http://mirrors.aliyun.com/kali`](http://mirrors.aliyun.com/kali)`kali-rolling main non-free contrib`

`# This system was installed using small removable media`

`# (e.g. netinst, live or single CD). The matching "deb cdrom"`

`# entries were disabled at the end of the installation process.`

`# For information about how to configure apt package sources,`

`# see the sources.list(5) manual.`

+--------------------------------------------------------------------------------------------------------+

> ┌─\[✗\]─\[ebony@blackmagic\]─\[~\]
>
> └──╼ $ping -c 10 222.165.175.166
>
> PING 222.165.175.166 \(222.165.175.166\) 56\(84\) bytes of data.
>
> 64 bytes from 222.165.175.166: icmp\_seq=1 ttl=60 time=28.6 ms
>
> 64 bytes from 222.165.175.166: icmp\_seq=2 ttl=60 time=30.6 ms
>
> 64 bytes from 222.165.175.166: icmp\_seq=3 ttl=60 time=29.5 ms
>
> 64 bytes from 222.165.175.166: icmp\_seq=4 ttl=60 time=30.9 ms
>
> 64 bytes from 222.165.175.166: icmp\_seq=5 ttl=60 time=31.8 ms
>
> 64 bytes from 222.165.175.166: icmp\_seq=6 ttl=60 time=31.0 ms
>
> 64 bytes from 222.165.175.166: icmp\_seq=7 ttl=60 time=30.5 ms
>
> 64 bytes from 222.165.175.166: icmp\_seq=8 ttl=60 time=30.5 ms
>
> 64 bytes from 222.165.175.166: icmp\_seq=9 ttl=60 time=28.5 ms
>
> 64 bytes from 222.165.175.166: icmp\_seq=10 ttl=60 time=30.4 ms
>
> --- 222.165.175.166 ping statistics ---
>
> 10 packets transmitted, 10 received, 0% packet loss, time 24ms
>
> rtt min/avg/max/mdev = 28.508/30.241/31.781/1.014 ms
>
> PING archive.ubuntu.com \(91.189.91.23\) 56\(84\) bytes of data.

&gt;--------Ubuntu sources list-------&lt;

`#deb cdrom:[Lubuntu 18.04 LTS _Bionic Beaver_ - Release amd64 (20180426)]/ bionic main multiverse restricted universe`

`# See`[`http://help.ubuntu.com/community/UpgradeNotes`](http://help.ubuntu.com/community/UpgradeNotes)`for how to upgrade to`

`# newer versions of the distribution.`

`deb`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic main restricted`

`# deb-src`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic main restricted`

`## Major bug fix updates produced after the final release of the`

`## distribution.`

`deb`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic-updates main restricted`

`# deb-src`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic-updates main restricted`

`## N.B. software from this repository is ENTIRELY UNSUPPORTED by the Ubuntu`

`## team. Also, please note that software in universe WILL NOT receive any`

`## review or updates from the Ubuntu security team.`

`deb`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic universe`

`# deb-src`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic universe`

`deb`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic-updates universe`

`# deb-src`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic-updates universe`

`## N.B. software from this repository is ENTIRELY UNSUPPORTED by the Ubuntu`

`## team, and may not be under a free licence. Please satisfy yourself as to`

`## your rights to use the software. Also, please note that software in`

`## multiverse WILL NOT receive any review or updates from the Ubuntu`

`## security team.`

`deb`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic multiverse`

`# deb-src`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic multiverse`

`deb`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic-updates multiverse`

`# deb-src`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic-updates multiverse`

`## N.B. software from this repository may not have been tested as`

`## extensively as that contained in the main release, although it includes`

`## newer versions of some applications which may provide useful features.`

`## Also, please note that software in backports WILL NOT receive any review`

`## or updates from the Ubuntu security team.`

`deb`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic-backports main restricted universe multiverse`

`# deb-src`[`http://lk.archive.ubuntu.com/ubuntu/`](http://lk.archive.ubuntu.com/ubuntu/)`bionic-backports main restricted universe multiverse`

`## Uncomment the following two lines to add software from Canonical's`

`## 'partner' repository.`

`## This software is not part of Ubuntu, but is offered by Canonical and the`

`## respective vendors as a service to Ubuntu users.`

`# deb`[`http://archive.canonical.com/ubuntu`](http://archive.canonical.com/ubuntu)`bionic partner`

`# deb-src`[`http://archive.canonical.com/ubuntu`](http://archive.canonical.com/ubuntu)`bionic partner`

`deb`[`http://security.ubuntu.com/ubuntu`](http://security.ubuntu.com/ubuntu)`bionic-security main restricted`

`# deb-src`[`http://security.ubuntu.com/ubuntu`](http://security.ubuntu.com/ubuntu)`bionic-security main restricted`

`deb`[`http://security.ubuntu.com/ubuntu`](http://security.ubuntu.com/ubuntu)`bionic-security universe`

`# deb-src`[`http://security.ubuntu.com/ubuntu`](http://security.ubuntu.com/ubuntu)`bionic-security universe`

`deb`[`http://security.ubuntu.com/ubuntu`](http://security.ubuntu.com/ubuntu)`bionic-security multiverse`

`# deb-src`[`http://security.ubuntu.com/ubuntu`](http://security.ubuntu.com/ubuntu)`bionic-security multiverse`

Ubuntu ව්ලට ලන්කවෙම mirror එකක් තියෙන්ව එක තමා ඔය උඩ ping කරලා තියෙන්නෙ . හෑබෑයි Debian\[/Parrrotsec/Kali\] ව්ලට එහෙම mirror එකක් නෑ , ඉතින් කවුරු හරි ලන්කාවෙ Debian mirror එකක් host කරන්ව නම් හොඩයි. ඈත්තහටම එහෙම Debian mirror එකක් හඩගන්න පුලුව්ම් උනොත් එක ලන්කවෙ එන්න Debian\[/Parrrotsec/Kali\] users ලා ලබපු ලොකු ජයක්ග්‍රහනයක්.

~[Setting up a Debian archive mirror](https://www.debian.org/mirror/ftpmirror)

