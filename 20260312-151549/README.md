# Delivery 20260312-151549

Encrypted patch delivery. All files are AES-256-CBC encrypted.

Script files are renamed with `.txt` suffix to allow download.
After downloading, remove the `.txt` suffix before use.

## Decrypt

```bash
mv decrypt.sh.txt decrypt.sh && chmod +x decrypt.sh
./decrypt.sh <passphrase>
```

**Windows:**
```cmd
ren decrypt.cmd.txt decrypt.cmd
decrypt.cmd <passphrase>
```

Then install patches into your target repo:
```bash
cd <target-repo>
./decrypted/install.sh --dry-run
./decrypted/install.sh
```
