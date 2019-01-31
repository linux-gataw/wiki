# Add new repo to debain family

අද අපි කතා කරන්නේ කොහොමද Debian family එකේ OS වලට් අමතර repo ඇතුලත් කරන්නේ කියල.

ubuntu වලට් debian repo දාන්න එපා family එක සමාන උනට් architecture එක වෙනස්. \([https://upload.wikimedia.org/wikipedia/commons/d/d8/Debian\_family\_tree\_11-06.png](https://upload.wikimedia.org/wikipedia/commons/d/d8/Debian_family_tree_11-06.png)\)

මුලිනම් පහල තියෙන command line ටික terminal එකට් ඇතුලත කරන්න. \(Ctrl + C ; Shift + Ctrl + V \)

```bash
sudo echo"deb[http://http.kali.org/kali](http://http.kali.org/kali)kali-rolling main contrib non-free" &gt; /etc/apt/sources.list.d/kali.list
```
```bash
sudo echo"deb[http://ftp.debian.org/debian](http://ftp.debian.org/debian)stable main contrib non-free" &gt; /etc/apt/sources.list.d/debian.list
```

ඔය command ඇතුලත් කලහම පහල තියෙන Err එක අවොත් ,

```text
bash: /etc/apt/sources.list.d/kali.list: Permission denied
```

පහල තියෙන command line ටික terminal එකට් ඇතුලත කරන්න. එතකොට් nano එකෙන් අදාල \*.list file එක open වේවි. එකට repo එක paste කරල save කරගන්න.

```bash
sudo nano /etc/apt/sources.list.d/kali.list
```
```bash
sudo nano /etc/apt/sources.list.d/debian.list
```

ඉගව්ට් update කරන්න \(sudo apt update\). එතකොට් පහල E , W & N අවොත්,

> W: GPG error: [http://ftp.debian.org/debian](http://ftp.debian.org/debian) stable Release: The following signatures couldn't be verified because the public key is not available: NO\_PUBKEY 8B48AD6246925553 NO\_PUBKEY 7638D0442B90D010 NO\_PUBKEY EF0F382A1A7B6500
>
> E: The repository '[http://ftp.debian.org/debian](http://ftp.debian.org/debian) stable Release' is not signed.
>
> N: Updating from such a repository can't be done securely, and is therefore disabled by default.
>
> N: See apt-secure\(8\) manpage for repository creation and user configuration details.
>
> W: GPG error: [http://kali.cs.nctu.edu.tw/kali](http://kali.cs.nctu.edu.tw/kali) kali-bleeding-edge InRelease: The following signatures couldn't be verified because the public key is not available: NO\_PUBKEY ED444FF07D8D0BF6
>
> E: The repository '[http://http.kali.org/kali](http://http.kali.org/kali) kali-bleeding-edge InRelease' is not signed.
>
> N: Updating from such a repository can't be done securely, and is therefore disabled by default.
>
> N: See apt-secure\(8\) manpage for repository creation and user configuration details.

පහල තියෙන command line ටික terminal එකට් ඇතුලත කරන්න.

```bash
gpg --keyserver pgpkeys.mit.edu --recv-key 8B48AD6246925553 && gpg -a --export 8B48AD6246925553 \| sudo apt-key add -
```
```bash
gpg --keyserver pgpkeys.mit.edu --recv-key 7638D0442B90D010 && gpg -a --export 7638D0442B90D010 \| sudo apt-key add -
```
```bash
gpg --keyserver pgpkeys.mit.edu --recv-key EF0F382A1A7B6500 && gpg -a --export EF0F382A1A7B6500 \| sudo apt-key add -
```
```bash
gpg --keyserver pgpkeys.mit.edu --recv-key ED444FF07D8D0BF6 && gpg -a --export ED444FF07D8D0BF6 \| sudo apt-key add -
```

අතිම්ට් upgrade කරන්න \(sudo apt dist-upgrade\)

මන් දන්නවා මේ පොස්ට් එක හුගක් කස්ටියට වැදගත් වෙන්නේ නැ කියලා ඒ වුනත් කට හරි වැදගත වේවි කියලා ලිව්වේ , මට් එචර හොද්ට් post ලියන්න නම් බැ ඉතින් පුලුවම් විදිය post එක කියවල තිරුම් ගන්න . මොනවා හරි ප්‍රශ්න තියෙනවා නම් අහන්න . මගේ output එක මෙතන තියෙනව එකත් ඔනිනුම් ගිහින් බලන්න [https://paste.ubuntu.com/p/Hq9XmTrmkZ/](https://paste.ubuntu.com/p/Hq9XmTrmkZ/)

ප .ලි. : ඇතම කිව්වොත් ubuntu repo වල තියෙන software update වෙන්ව හොරයි , එක නිසි මං debian repo දැම්මේ .

