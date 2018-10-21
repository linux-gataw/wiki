# Linux Directory Structure / File System Structure ගැන ඉගෙනගනිමු.

![](.gitbook/assets/image%20%282%29.png)

 අද අපි කතා කරන්න යන්නේ Linux මෙහෙයුම් පද්ධතියේ Directory Structure එහෙමත් නැත්තම් File System Structure එක ගැනයි.  
 හොදයි, වැඩිය කතා නැතුව මාතෘකාවට එමු. ඉතින් මොකද්ද මේ Directory Structure එහෙමත් නැත්තම් File System Structure කියල කියන්නේ? පරිගණක විද්‍යාවේදී Directory Structure එහෙමත් නැත්තම් File System Structure එකක් කියල කියන්නේ යම්කිසි මෙහෙයුම් පද්ධතියක් විසින් එම මෙහෙයුම් පද්ධතියේ ඇති file system සහ ඒවාට අදාල files පරිගණක පරිශීලකයාට ප්රදර්ශනය කරන ආකාරයට තමයි සරලව Directory Structure එහෙමත් නැත්තම් File System Structure කියල කියන්නේ.  
 Windows මෙහෙයුම් පද්ධතියක File System Structure එක සහ Linux මෙහෙයුම් පද්ධතියක File System Structure එක අතර ලොකු වෙනසක් තියනවා. Windows මෙහෙයුම් පද්ධතියක නම් අපේ physical devices \(Cd-Rom, Pen Drive, External HDD\) Disks විදිහට පෙන්නනවා. හැබැයි Linux මෙහෙයුම් පද්ධතියේ ඕනෙම දෙයක් file එකක්. ඒ කියන්නේ අපේ physical devices සහ අනෙකුත් සෑම දේම සලකන්නේ files විදිහට. ඔන්න ඕක තමයි මේ File System Structure අතර තියන ප්‍රධාන වෙනස. Linux වල file එකක් නොවන ඕනෙම දෙයක් සලකන්නේ Process එකක් විදිහට. ඉතින් ඔන්න ඔය හේතුව හින්ද Linux වල files සහ directories අතර වෙනසක් නැ. දෙකම එකයි.  
 Filesystem Hierarchy Standard \(FHS\) කියල සම්මතයකට අනුව තමයි Linux වල directory structure හැදිලා තියෙන්නේ. Linux Foundation කියල සංවිධානයක් තමයි මේක ගොඩනගල තියෙන්නේ. ගොඩක් Linux distributions මේ FHS එක පවත්වාගෙන යන්න බැදීල ඉන්නවා. මේ FHS එක පවත්වාගෙන යන්න කොච්චර බැදිලා ඉන්නවද කිව්වොත් ගොඩක් Linux distributions මේක වෙනුවෙන් එයාලගෙම ප්රතිපත්ති නිර්මාණය කරලා තියනවා. GoboLinux සහ NixOS කියන්නේ නම් මේ සම්මතය අනුගමනය කරන්නේ නැති මෙහෙයුම් පද්දති දෙකක්.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️Root Directory \( / \)

 මේ Linux Directory Structure එකේ මුලින්ම ඉන්නේ root කියන Directory එක. මේ Directory එකෙන් තමයි හැම file එකක්ම සහ හැම Directory එකක්ම ආරම්භ වෙන්නේ. Linux මෙහෙයුම් පද්ධතිය ක්‍රියාත්මක වෙන්න ඕනේ කරන හැම දේම තියෙන්නේ මේකේ. root userට \(Windows වල නම් administrator\) තමයි මේ Directory එකේ write privilege එක \(මේකේ තියන files, folders modify කරන්න\) තියෙන්නේ.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ bin Directory \( /bin \) - User Binaries

 මේ Directory එකේ තියෙන්නේ binary executable. ඒ කියන්නේ Linux මෙහෙයුම් පද්ධතියට Boot වෙන්න සහ run කරන්න ඕනේ කරන files. system එකේ හැම user කෙනෙක්ම භාවිත කරන පොදු Linux විධාන, උදාහරණයක් විදිහට ps, ls, ping, grep, cp වගේ ඒවා ගබඩා වෙලා තියෙන්නේ මේ directory එකේ.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ sbin Directory \( /sbin \) – System Binaries

 මේ Directory එකේ තියෙන්නේත් binary executables ම තමයි. ඒ උනාට මේකේ ගබඩා කරලා තියන විධාන භාවිත කරන්නේ system aministratorsල විසින් පද්ධතියේ නඩත්තුව සදහා. iptables, reboot, fdisk, ifconfig, swapon වගේ විධාන වැටෙන්නේ මේ directory එකට.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ etc Directory \( /etc \) – Configuration Files

 මේ directory එකේ තියෙන්නේ මෙහෙයුම් පද්ධතියේ තියන හැම program එකකටා අදාල වින්යාසය \(Configuration\) files. ඒ වගේම තනි වැඩසටහන් ඇරබීමට සහ නැවත්වීමට අදාළ startup සහ shutdown shell scripts ගබඩා වෙලා තියෙන්නේ මේ directory එකේ. උදාහරණ විදිහට :- /etc/resolv.conf/etc/logrotate.conf

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ dev Directory \( /dev \) – Device Files

 මේ directory එකේ තියෙන්නේ මෙහෙයුම් පද්ධතියට සම්බන්ද කරන හැම devices වලට අදාල device files. මේකෙදි මේ හැම device එකක්ම පෙන්නන්නේ files විදිහට.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ proc Directory \( /proc \) – Process Information

 මේ directory එක system එකේ විශේෂ directory එකක්. පද්ධතියේ පද්ධති ක්රියාවලිය \(system process\) අඩංගු වෙලා තියෙන්නේ මේකේ. ඇත්තටම මේ directory එක pseudo filesystem එකක්. ඒ කියන්නේ මොකද්ද ? ඉංග්‍රීසි භාෂාවෙන් pseudo කියන්නේ අසත්යය/බොරු වගේ අදහසක්. ඉතින් මේ pseudo filesystem එකෙත් ඇත්ත files නැ. මේකේ තියෙන්නේ virtual entries. ඒ කියන්නේ filesystem එක විසින් ඒ වෙලාවේ ඒ මොහොතේ හදාගන්න entries. සාමාන්‍ය user කෙනෙක්ට මේ files අල්ලනවත් බැ.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ var Directory \( /var \) – Variable Files

 මේ directory එක තියෙන්නේ system එක run වෙනකොට නිතරම වගේ වෙනස් වෙන files. උදාහරණයක් විදිහට system log files \(/var/log\), packages and database files \(/var/lib\), emails \(/var/mail\) වගේ ඒවා දක්වන්න පුළුවන්.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ tmp Directory \( /tmp \) – Temporary Files

 මේ directory එක තියෙන්නේ තාවකාලිකව system එක විසින් නිර්මාණය කරපු files. system එක reboot කරපු ගමන් මේ files මැකෙනවා.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ usr Directory \( /usr \) – User Programs

 මේ directory එකේ තමයි සමන්‍යා usersල use කරන programs වලට අදාල binaries, libraries, documentation, සහ source-code තියෙන්නේ මේකේ.

 /usr/bin - මේකේ තියෙන්නේ usersලගේ programs වලට අදාල binary files.  
 /usr/sbin - මේකේ තියෙන්නේ system administratorsලගේ programs වලට අදාල binary files.  
 /usr/lib - මේකේ තියෙන්නේ /usr/bin සහ /usr/sbin වලට අදාල libraries.  
 /usr/local - මේකේ තියෙන්නේ usersල පිටතින් install කරන programs වලට අදාල files. උදාහරණයක් විදිහට ඔය apache කියන program එක install කරොත් එක යන්නේ /usr/local/apache2 කියන location එකට.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ home Directory \( /home \) – Home Directories

 මේ Directory එක තියෙනේ Linux මෙහෙයුම් පද්ධතියේ ඉන්න ඔක්කොම usersලට තමන්ගේ පෞද්ගලික files රදවා තබාගන්න. මම පෙන්නලා තියන රූපයේ නම් usersල නැ. මොකද මගේ pc එක මම run කරන්නේ root user හැටියට විතරයි. හැබැයි usersල ඉන්නවනම් ඔය home directory එක ඇතුලේ userගේ නම එක්ක folders හැදෙනවා. උදාහරණයක් විදිහට /home/user1, /home/user2

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ boot Directory \( /boot \) – Boot Loader Files

 මේ Directory එක තියෙනේ Linux මෙහෙයුම් පද්ධතිය boot වෙන්න ඕනේ කරන files. \(boot loader එකට අදාල files\) Kernel initrd, vmlinux, grub වගේ files ගබඩා වෙලා තියෙන්නේ මේකේ.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ lib Directory \( /lib \) – System Libraries

 මේ Directory එක තියෙනේ /bin සහ /sbin කියන directories වල තිබ්බ binaries වලට අදාළ library files. මේ libraries වල filenames ld\* හෝ lib\*.so.\* වෙන්න පුළුවන්. උදාහරණයක් විදිහට libapparmor.so.1.4.1 දක්වන්න පුළුවන්.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ opt Directory \( /opt \) – Optional add-on Applications

 මේ directory එක තියෙන්නේ default system එකේ තියන softwares හෝ programs වලට අමතරව එකතුවෙන ඒවා ගබඩා කරලා තියාගන්න.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ mnt Directory \( /mnt \) – Mount Directory

 මේ directory එකත් /media directory එකට සමානයි. මේක use වෙන්නේ අපි Linux මෙහෙයුම් පද්ධතියට සම්බන්ධාකරන devices mount කරන්න. මේ directory එකේදී අපිට devices manually mount කරන්නත් පුළුවන්.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ media Directory \( /media \) – Removable Media Devices

 මේ directory එක use වෙන්නේ අපි සම්බන්ද කරන devices automatically mount කරන්න. external harddisk, USB, CD/DVD වගේ දේවල් උදාහරණ විදිහට දක්වන්න පුළුවන්.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ srv Directory \( /srv \) – Service Data

 Linux මෙහෙයුම් පද්ධතියේ සේවාවන් වලට අදාළ දත්ත ගබඩා කර තබාගනියි.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ run Directory \( /run \)

 මෙම run directoriය File System Structure එක සදහා මෑතකදී හදුන්වා දුන් එකකි. එය එක්තරා විදිහක temp folder එකකි. පද්ධතිය boot වන අවස්ථාවේ run වීමට අවශ්‍ය programs මෙහි ඇත. /var/run සදහා විකල්පයකි.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫️ Lost+Found Directory

 මේ directory එක recovery folder එකක් විදිහට වැඩ කරන්නේ. මොකක් හරි හේතුවක් නිසා system එක crash වෙලා Linux file system checker විසින් corrupt වෙච්ච files recover කරගත්තොත් ඒවා save වෙන්නේ මෙන්න මේ folder එකේ. file system එකේ හැම partition එකකටම මේ වගේ folder එකක් තියනවා.

 හොදයි යාලුවනේ. මේ ලිපියට මම ලියන්න බලාපොරොත්තු උනේ ඔච්චරයි. වැරදි අඩුපාඩු තියනවනම් කියන්න. මේවගේම තවත් ලිපියකින් මුණගැහෙමු. ලිපිය කියෙව්වට ස්තුතියි. මේ ලිපිය යාළුවන් අතර බෙදාගන්න අමතක කරන්න එපා. \(ගොඩක් දෙනෙක් මගේ ඉල්ලුව මේ වගේ articles කෙලින්ම fb එකේම දන්නා කියල. ඒ ඉල්ලීමට අනුව මම මගේ බ්ලොග් එක නැවැත්තුවා. අද ඉදන් කෙලින්ම fb එකෙමයි post දන්නේ.\)  
 Written With ![](https://static.xx.fbcdn.net/images/emoji.php/v9/ff3/1.5/16/2764.png)❤️ By -[Sameera Madhushan](https://www.facebook.com/sameera.madushan.1422409?fref=mentions&__xts__%5B0%5D=68.ARBZvbDaqgfsOCmbv7dhCOiK_LZI2oSGL8g3937fpdfCmaAS9Liwv6CoyzjD6NXC8CP7ComhiaXgSdMRc2kXS6SXTUW73z1HCz_xKJz3UB1Y-hmYEx0oRm6WXYv7vDa111g3j5xBgUn8qdJepmr6bqIljBWBMr515ttl50ZexbTqQ_4slxoY&__tn__=KH-R)- a.k.a άλφα Χ

