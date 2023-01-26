## For Windows 11

### Step 1 - Open PowerShell or Command Prompt as administrator

### Step 2 - Install KMS client key
```bash
slmgr /ipk your_license_key
```
Replace `your_license_key` with following volumn license keys according to Windows Edition:
```bash
Home: TX9XD-98N7V-6WMQ6-BX7FG-H8Q99
Home N: 3KHY7-WNT83-DGQKR-F7HPR-844BM
Home Single Language: 7HNRX-D7KGG-3K4RQ-4WPJ4-YTDFH
Home Country Specific: PVMJN-6DFY6-9CCP6-7BKTT-D3WVR
Pro: W269N-WFGWX-YVC9B-4J6C9-T83GX
Pro N: MH37W-N47XK-V7XM9-C7227-GCQG9
Education: NW6C2-QMPVW-D7KKK-3GKT6-VCFB2
Education N: 2WH4N-8QGBV-H22JP-CT43Q-MDWWJ
Enterprise: NPPR9-FWDCX-D2C8J-H872K-2YT43
Enterprise N: DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4
```

### Step 3 - Set KMS machine address
```bash
slmgr /skms 193.29.63.133:1688
```
Check out the latest server at [KMS servers](https://kms.msguides.com/)

### Step 4 - Activate your Windows
```bash
slmgr /ato
```
