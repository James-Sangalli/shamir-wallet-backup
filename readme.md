# About

This tool is designed to help crypto users back up their wallets with shamir's secret sharing.

The idea behind this tool is that you would split your seed phrase into parts and distribute them to multiple cloud providers. This would make it harder for an attacker to gain access to your keys as they would need to break into more than one account. This approach also makes it easier to recover your keys, should you lose your own copy on local storage and simpler than giving shares to individuals.

This tool will generate a fresh seed phrase for you but you are able to put whatever data you want in the boxes. 

This tool is a fork of Ian Coleman's shamir's secret sharing [repo](https://github.com/iancoleman/shamir).

**This tool is experimental, use it at your own risk!**

# Usage

## Share files
Files saved to a provider like Google Drive or Dropbox will contain the share as the filename. Simply copy this filename and do the combining process to reconstruct the key.

## Splitting

Enter the text of your secret into the field.

Copy each individual part to a file.

Distribute the files.

## Combining

Gather enough parts to recreate the secret.

Enter the content from each part into the field.

The text of the secret will be displayed under the field.

# Developing

After making changes, compile to a single page for offline use with:

```
python compile.py
```

Pull requests are welcome.

# License

MIT, see [license](https://github.com/James-Sangalli/shamir-wallet-backup/blob/master/license).
