## macOS temp folders in the /var/folders/zz

If you work with Macintosh computers and administer a Macintosh network probably you would like to know what is in the temporary folders, inside the /var/folders/zz folder.

You can read about this from James Reynold page: http://www.magnusviri.com/Mac/what-is-var-folders.html

If some kind of way you have magical permission problems, like download and / or install updates from App Store, or download your iTunes shoppings, or few application permanently asking your admin username and password… thenmaybe you have a permission problem in the /var/folders/zz folder. This is THE temp foder for the whole macOS system.

```
ls -la /var/folders
```
After hitting Enter, you can see something similar:

```
total 0
drwxr-xr-x   8 root  wheel   272 Sze 14 23:42 .
drwxr-xr-x  31 root  wheel  1054 Aug 28 00:45 ..
drwxr-xr-x@  3 root  wheel   102 Dec 17  2016 mr
drwxr-xr-x@  3 root  wheel   102 Aug 28 00:44 p8
drwxr-xr-x@  3 root  wheel   102 Dec 19  2016 rv
drwxr-xr-x@  3 root  wheel   102 Dec 19  2016 sc
drwxr-xr-x@  3 root  wheel   102 Sze 14 23:42 vm
drwxr-xr-x@ 25 root  wheel   850 Jún 14 23:36 zz
```

If you go into the folder "zz" and LS the content, you could see something like this:

```
total 40
drwxr-xr-x@ 40 root             wheel             1360 31 Aug 15:49 .
drwxr-xr-x   9 root             wheel              306 15 Sep 21:56 ..
-rw-r--r--@  1 root             wheel            18436 29 Aug 22:33 .DS_Store
drwxrwxr-x@  6 root             wheel              204 28 Okt  2015 zyxvpxvq6csfxvn_n0000000000000
drwxr-xr-x   3 _networkd        _networkd          102 28 Okt  2015 zyxvpxvq6csfxvn_n000003000000r
drwxr-xr-x   3 _lp              _lp                102 28 Okt  2015 zyxvpxvq6csfxvn_n000003800000t
drwxr-xr-x   4 _appleevents     _appleevents       136 28 Okt  2015 zyxvpxvq6csfxvn_n000006w00001q
drwxr-xr-x   4 _mdnsresponder   _mdnsresponder     136 28 Okt  2015 zyxvpxvq6csfxvn_n0000084000021
drwxr-xr-x   4 _spotlight       _spotlight         136 28 Okt  2015 zyxvpxvq6csfxvn_n00000b400002s
drwxr-xr-x   4 _securityagent   _securityagent     136 28 Okt  2015 zyxvpxvq6csfxvn_n00000bh00002w
drwxr-xr-x   4 _atsserver       _atsserver         136 28 Okt  2015 zyxvpxvq6csfxvn_n00000c4000031
drwxr-xr-x   4 _softwareupdate  _softwareupdate    136 28 Okt  2015 zyxvpxvq6csfxvn_n00000s0000068
drwxr-xr-x   4 _coreaudiod      _coreaudiod        136 28 Okt  2015 zyxvpxvq6csfxvn_n00000s800006_
drwxr-xr-x   4 _locationd       _locationd         136 28 Okt  2015 zyxvpxvq6csfxvn_n00000sm00006d
drwxr-xr-x   4 _cvmsroot        _cvms              136 28 Okt  2015 zyxvpxvq6csfxvn_n00000th00006m
drwxr-xr-x   3 _usbmuxd         _usbmuxd           102 28 Okt  2015 zyxvpxvq6csfxvn_n00000tm00006n
drwxr-xr-x   4 _netbios         _netbios           136 28 Okt  2015 zyxvpxvq6csfxvn_n00000vr00006y
drwxr-xr-x   4 _assetcache      _assetcache        136 28 Okt  2015 zyxvpxvq6csfxvn_n00000xc00007b
drwxr-xr-x   4 _iconservices    _iconservices      136 28 Okt  2015 zyxvpxvq6csfxvn_n00000y000007h
drwxr-xr-x   3 _distnote        _distnote          102 28 Okt  2015 zyxvpxvq6csfxvn_n00000y400007j
drwxr-xr-x   4 _nsurlsessiond   _nsurlsessiond     136 15 Sep 20:51 zyxvpxvq6csfxvn_n00000y800007k
drwxr-xr-x   3 _nsurlstoraged   _nsurlstoraged     102 28 Okt  2015 zyxvpxvq6csfxvn_n00000yc00007l
drwxr-xr-x@  5 _mbsetupuser     _mbsetupuser       170 27 Aug 22:00 zyxvpxvq6csfxvn_n00000z000007r
drwxr-xr-x@  5 _datadetectors   _datadetectors     170 31 Aug 15:49 zyxvpxvq6csfxvn_n0000104000081
drwxr-xr-x@  5 _captiveagent    _captiveagent      170 27 Aug 21:59 zyxvpxvq6csfxvn_n0000108000082
drwxr-xr-x@  5 _ctkd            _ctkd              170 27 Aug 21:58 zyxvpxvq6csfxvn_n000010c000083
drwxr-xr-x@  5 _applepay        _applepay          170 27 Aug 22:00 zyxvpxvq6csfxvn_n000010h000084
drwxr-xr-x@  5 _hidd            _hidd              170 27 Aug 21:58 zyxvpxvq6csfxvn_n000010m000085
drwxr-xr-x   5 root             wheel              170 16 Okt  2015 zzzivhrRnAmviuee+++++++++++
drwxr-xr-x   3 root             wheel              102 17 Okt  2015 zzzivhrRnAmviuee++++4U+++-c
drwxr-xr-x   4 root             wheel              136 13 Okt  2015 zzzivhrRnAmviuee++++EE+++22
drwxr-xr-x   4 root             wheel              136 13 Okt  2015 zzzivhrRnAmviuee++++KE+++3Y
drwxr-xr-x   3 root             wheel              102  9 Mär  2013 zzzivhrRnAmviuee++++L++++3k
drwxr-xr-x   4 root             wheel              136 13 Okt  2015 zzzivhrRnAmviuee++++ME+++42
drwxr-xr-x   3 root             wheel              102 13 Okt  2015 zzzivhrRnAmviuee++++mU+++Ac
drwxr-xr-x   4 root             wheel              136  3 Aug  2015 zzzivhrRnAmviuee++++nE+++Ao
drwxr-xr-x   3 root             wheel              102 16 Mär  2013 zzzivhrRnAmviuee++++o++++B+
drwxr-xr-x   4 root             wheel              136 13 Okt  2015 zzzivhrRnAmviuee++++p++++BE
drwxr-xr-x   3 root             wheel              102 13 Okt  2015 zzzivhrRnAmviuee++++pE+++BI
drwxr-xr-x   4 root             wheel              136 24 Okt  2015 zzzivhrRnAmviueezzzzzjzzzzs
```

Take a look to the owners and the groups… If you don't see this, then you found your problem. The folder names looks like random but each folder on each Macintosh has the same owner and owner group. For example if you have problem with your Software Update from the App Store, check the folder named "zyxvpxvq6csfxvn_n00000s0000068". the _softwareupdate user and the _softwareupdate group should be set for it. If the folder missing, then create it and then set the user:group.

```
_softwareupdate  _softwareupdate    136 28 Okt  2015 zyxvpxvq6csfxvn_n00000s0000068
```

To do it in the Terminal:

```

mkdir /var/folders/zz/zyxvpxvq6csfxvn_n00000s0000068
sudo chown _softwareupdate:_softwareupdate /var/folders/zz/zyxvpxvq6csfxvn_n00000s0000068
sudo chmod 755 /var/folders/zz/zyxvpxvq6csfxvn_n00000s0000068
```

If you have many of these folder wrong and would like to use a GUI App for set the correct owners/groups/access rights you can use BatChmod app: http://www.lagentesoft.com/batchmod/index.html or direct downlowd: http://www.lagentesoft.com/resources/batchmod_17b5.zip

## — WARNING —

Take really care, with BatChmod you can destroy the complete permission system of your computer. If you do something wrong, your Mac won't start anymore and you have to do lot of work in Recovery Mode (start the computer with Command+R ) and in the Terminal.

## — WARNING —

Sources:

http://www.magnusviri.com/Mac/what-is-var-folders.html

https://forums.macrumors.com/threads/cannot-apply-any-os-x-system-updates-via-app-store.1841892/page-2

https://forums.macrumors.com/threads/cant-install-10-10-1-please-help.1822283/
