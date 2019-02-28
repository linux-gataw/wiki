![](https://i.imgur.com/k0klINIl.jpg "\[Image: k0klINIl.jpg\]")

 අදත්  ගෙනාවේ linux comands ඉගෙන ගන්න පුලුවන් site එකක්.\(කලින් එක බැලුවෙ නැත්තන් මෙතනින් යන්න: [https://www.widane.com/thread-470.html](https://www.widane.com/thread-470.html)\) මේකේ තියන විශේෂත්වය තමයි මේකෙ commands ඉගෙන ගන්න තියෙන්නේ CTF style එකට, දැන් බලනවා අති මේ මොකක්ද මේ කියන්නේ කියලා. මෙකේ අපිට මුලින්ම box එකක ssh logins දෙනවා, එ box එකේ අදාල userගේ flag එකක් හංගලා වගේ තියනවා. ඒක හොයා ගන්න තියෙන්නේ. පලවෙනි user එකෙන් ගිහින් ගන්න flag එක තමයි, 2වෙනි userගේ password එක. ඔය විදියට තමා ඉස්සරහට යන්න තියෙන්නේ.

 මේකේ ගොඩක් games තියන්වා අපි Bandit එකෙන් පටන් ගමු.

 ම්කේ මන් පලවෙනි flag \(level 0\) එක ගන්න හැටි කියන්නම්.\(ඒකේ ගන්න දෙයක් නෑ එහෙම් පිටින්ම තියේ [Linux commands ඉගෙන ගමු.](linux-commands.md)\).

 හරි එහෙනම් මේකට යන්න.

[http://overthewire.org/wargames/bandit/](http://overthewire.org/wargames/bandit/)

 දැන් කියලා තියන ඒවා හොදට කියවන්න. \(ඉංගිරීසි බෑ කියල ඉන්නැතුව කීයෝපන්\). දැන් [level0](http://overthewire.org/wargames/bandit/bandit0.html) කියන එකට යන්න. දැන් එකත් හොදට කියවන්න ![](https://www.widane.com/images/smilies/tongue.png "Tongue"). ඒකේ දැන් ssh logins දීලා ඇති. දැන් බලමු ssh වලින් කොහොමද ඒ machine එකට log වෙන්නේ කියලා.

## Method 1 - Using CMD/Terminal

 දැන් CMD open කරන්න \(Windows 10 පමණි\). Linux හෝ macOS නම් Terminal එක open කරගන්න.  දැන් මෙහෙම ගහලා enter දෙන්න.

Code:

`ssh bandit0@bandit.labs.overthewire.org -p 2220`

 Are you sure bla bla කියලා ආවොත් yes දීල enter කරන්න.

 password එකට bandit0 දෙන්න. 

![](https://i.imgur.com/7sqpi4Ll.jpg "\[Image: 7sqpi4Ll.jpg\]")

## Method 2 - Using Putty

 උඩ method එක හරිගියෙ නැත්තම් මෙහෙම කරන්න. මුලින්ම putty install කරගන්න මෙතනින් ගිහින්.

[Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

 install කර ගත්තනම් putty open කරන්න. දැන් මේ වගේ window එකක් open වෙයි.

![](https://i.imgur.com/poMdiJ7l.jpg "\[Image: poMdiJ7l.jpg\]")

 අරකේ කියල තියන ව්දියට Host Name කියන තැනට bandit.labs.overthewire.orgදෙන්න. port එකට 2220. type එක ssh. 

![](https://i.imgur.com/XIgeSBpl.jpg "\[Image: XIgeSBpl.jpg\]")

 දැන් ඔපෙන් දෙන්න. login as එකට bandit0. password එකත් bandit0කියලා දෙන්න.\(paste කරද්දි right mouse click එකක් හෝ shift+insert දෙන්න.\)

![](https://i.imgur.com/4Wx6ctTl.jpg "\[Image: 4Wx6ctTl.jpg\]")

 හරියට log උනානම් දැන් ඊලග ලෙවෙල් එකට යමු. [Level 0 → Level 1](http://overthewire.org/wargames/bandit/bandit1.html) .

 Terminal එකේ ls command එක ගහලා බලන්න අපි ඉන්න dir එකේ මොනාද තියෙන්නේ කියලා.

![](https://i.imgur.com/f1opbkAl.jpg "\[Image: f1opbkAl.jpg\]")

 'readme' කියලා file එකක් තියෙනවා පෙනෙයි. ඒකේ අතුලේ තියෙන්නේ මොනාද තියෙන්නේ බලන්න මෙහෙම ගහන්න.

Code:

`cat readme`

![](https://i.imgur.com/bElDZs2l.jpg "\[Image: bElDZs2l.jpg\]")

 ඔය තියෙන්නේ flag එක  ![](https://www.widane.com/images/smilies/haha.png "haha")![](https://www.widane.com/images/smilies/haha.png "haha") . ඕක තමයි ඊලග userගේ password එක. ඒ කියන්නෙ bandit1ගේ passowrd එක. දැන් අර ව්දියටම ssh වල bandit0 වෙනුවට bandit1 කියලා දීලා. password එකට දැන් ගත්ත falg eka දෙන්න.

![](https://i.imgur.com/ZJgWuCDl.jpg "\[Image: ZJgWuCDl.jpg\]")

 කලින් ඔයා server එකට log වෙලා ඉන්න නිසා ඔයාට ඔන්නම් මෙහෙමත් ගහලා අනිත් usersලට log වෙන්න පුලුවන්.

 For eg: bandit1

Code:

`ssh bandit1@localhost`

![](https://i.imgur.com/OS1FiBFl.jpg "\[Image: OS1FiBFl.jpg\]")

 Level එකට අදාල එන්න පුලුවන් commands site එකේ දීලා ඇති. එකෙන් කරන්න තියන දේ ගැන හිතා ගන්න පුලුවන් වෙයි.

![](https://i.imgur.com/zUWxzz7l.jpg "\[Image: zUWxzz7l.jpg\]")

 හැම තිස්සෙම level එකෙන් level එකට කියලා තියන දේවල් හොදට කියවන්න. හරිනේ! එහෙනම් ඉතින් ඉතිරි ටික තනියෙම කරගෙන යන්නයි තියෙන්නේ. අවුලක් තියේ නම් comment එකක් දන්න. මම කැපුනා එහෙනම්.

 ඔබට ජය!!!



~[_**Anøn LK**_](https://www.widane.com/user-3.html)

