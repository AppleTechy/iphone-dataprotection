1. backup iphone to your pc with **password**

2. extract using the tool

  https://github.com/dinosec/iphone-dataprotection

```
$ source ../.ve_2.7/bin/activate
$ # extract and decrypt from a backup
$ python iphone-dataprotection/python_scripts/backup_tool.py ~/Library/Application\ Support/MobileSync/Backup/ABCD ./Backup_extract/ABCD
<enter password>
$ python iphone-dataprotection/python_scripts/keychain_tool.py -d Backup_extract/ABCD/KeychainDomain/keychain-backup.plist Backup_extract/ABCD/Manifest.plist > out.txt
<enter>
```