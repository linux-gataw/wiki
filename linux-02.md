# මූලික Linux විධාන - 02 කොටස

![](.gitbook/assets/image%20%281%29.png)

 මූලික Linux විධාන පිළිබද නිබන්දනයේ දෙවනි කොටසට ඔයාලව ආදරයෙන් පිලිගන්නවා. මේකේ පලවෙනි කොටස තාම කියෙව්වේ නැත්තම් පහල Comment Section එකේ link එක තියනවා ගිහින් කියවන්න.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫ rmdir විධානය

 මේ විධානය use කරන්නේ අපි create කරපු directories මකල දන්න. හැබැයි මේ විධානයෙන් මකන්න පුළුවන් හිස් \(empty\) directories විතරයි. මේ විධානය use කරන්නේ මෙහෙමයි, අපිට මකන්න ඕනේ කරන directory එක තියන තැනට path එක මාරුකරලා rmdir &lt;directory name&gt; type කරන්න තියෙන්නේ.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫ rm විධානය

 මේ විධානය use කරන්නේ files සහ directories දෙකම මකන්න. මේ rm විධානයට කෙලින්ම directory එකක් මකන්න බෑ. rm විධානය භාවිත කරලා directory එකක් කෙලින්ම මකන්න ඕනෙනම් ඊට ඉස්සරහින් -r යොදන්න වෙනවා. සම්පුරණ කේතය එන්නේ මෙහෙමයි. rm -r &lt;directory name&gt; මේ විධානය directory එකක් ඇතුලේ තියන files මකන්නත් යොදාගන්නත් පුළුවන්. ඒ අවස්ථාවේදී මේ විධානය යොදාගන්නේ අපිට මකන්න ඕනේ කරන file එක තියන directory එක ඇතුලට ගිහින් rm &lt;file name&gt; type කරන්න තියෙන්නේ.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫ touch විධානය

 මේ විධානය use කරන්නේ අලුත් file එකක් හදාගන්න. මේ විධානය use කරන්නේ අලුත් file එකක් හදාගන්න. උදාහරණයක් විදිහට මට Desktop එකේ "hacking" කියල text file එකක් හදාගන්න ඕනෙනම් කරන්න තියෙන්නේ touch hacking.txt කියල විධානය ලබාදෙන්න විතරයි.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫ sudo විධානය

 sudo විධානය තමයි Linux command line එකේ වැඩිපුරම වගේ use වෙන විධානය. මේකේ තේරුම “SuperUser Do” කියන එකයි. ඉතින් අපිට මොකක් හරි විධානයක් root privileges එහෙමත් නැත්තම් administrator විදිහට use කරන්න ඕනෙනම් අපිට කරන්න තියෙන්නේ මේ විධානය use කරන්න. භාවිතා කරන්න හරිම ලේසියි. මේ විධානයේ syntax එක සරලව එන්නේ මෙහෙමයි. sudo &lt;command&gt; \(මේ විධානයට අදාල options නැතුව\)

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫ man සහ –help විධානයන්

 මොකක් හරි විධානයක් ගැන සහ එම විධානය use කරන හැටි ගැන දැනගන්න මේ man විධානය යොදාගන්න පුළුවන්. ඇත්තටම මේ විධානයෙන් අපි භාවිතා කරන විධානයන්ට අදාල manual එක බලාගන්න පුළුවන්. උදාහරණයක් විදිහට sudo විධානය ගැන දන ගන්න ඕනෙනම් man sudo කියල විධානය දුන්නහම ඒ විධානයට අදාල manual page එක අපිට පෙන්නනවා.

 -help විධානය \(ඇත්තටම මේක argument එකක්\) යොදාගෙන යම්කිසි විධානයක් use කරන ආකාරය ගැන බලාගන්න පුළුවන්. උදාහරනයක් විදිහට ifconfig -help විධානය use කරලා ifconfig විධානය භාවිතා කරන්න ඕනේ විදිහ ගැන බලාගන්න පුළුවන්.

 ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫ Linux Command Line එක භාවිතය පහසු කරන ඉඟි සහ උපක්රම කිහිපයක් ![](https://static.xx.fbcdn.net/images/emoji.php/v9/f95/1.5/16/26ab.png)⚫

 ඔයාගේ terminal එක ගොඩාක් විධාන වලින් පිරිලා තියෙද්දී clear විධානය යොදාගෙන ඕනෙම වෙලාවක ඔයාගේ terminal එක පිරිසිදු කරගන්න පුළුවන්.  
 Ctrl+C යොදාගෙන ඕනෙම අවස්ථාවක ක්‍රියාත්මක වෙමින් පවතින විධානයක් ආරක්ෂාකාරීව නවත්වන්නට පුළුවන්.  
 exit විධානය යොදාගෙන ඕනෙම අවස්ථාවක terminal එකෙන් ඓන් වෙන්න පුළුවන්.  
 sudo halt සහ sudo reboot යන විධාන යොදාගෙන පරිගණකය power off හෝ reboot කරන්න පුළුවන්.  
 Ctrl+C යොදාගෙන යම්කිසි ක්‍රියාවලියක් නැවත්වීමට නොහැකි උනොත් Ctrl+Z යොදාගෙන එය බලෙන් නැවත්වීමට \(force stop\) පුළුවන්.

 හොදයි යාලුවනේ. මේ ලිපියට මම ලියන්න බලාපොරොත්තු උනේ ඔච්චරයි. වැරදි අඩුපාඩු තියනවනම් කියන්න. මේවගේම තවත් ලිපියකින් මුණගැහෙමු. ලිපිය කියෙව්වට ස්තුතියි. මේ ලිපිය යාළුවන් අතර බෙදාගන්න අමතක කරන්න එපා.  
 Written With ![](https://static.xx.fbcdn.net/images/emoji.php/v9/ff3/1.5/16/2764.png)❤️ By -[Sameera Madhushan](https://www.facebook.com/sameera.madushan.1422409?fref=mentions&__xts__%5B0%5D=68.ARCuDq_qG7jin5vJlzQh405-28eA6kjZHitPIhz-LNzhz4gl2denBR23HrtoinevEsOuy8BBdczbUvhxhGCaYgUHf25KjEu17t6jYYIuAcy4FolCXuS3E9PMCC7Qi_4wrXb4-dLEfjBI4YD1wNruTtm3MprpYMySCiDwnzQEkh7coaPUT_9L&__tn__=KH-R)- a.k.a άλφα Χ

