## For Windows Server

### Step 1 - Open PowerShell or Command Prompt as administrator

### Step 2 - Convert Windows Server Evaluation to retail edition
**To get the available editions:**
```bash
DISM /Online /Get-TargetEditions
```

**To set your Windows Server to a higher edition:**
```bash
DISM /online /Set-Edition:ServerStandard /ProductKey:XXXXX-XXXXX-XXXXX-XXXXX-XXXXX /AcceptEula
```

### Step 3 - Install KMS client key
```bash
slmgr /ipk your_license_key
```
Replace `your_license_key` with following volumn license keys according to Windows Edition:
```bash
Windows Server 2022 Datacenter: WX4NM-KYWYW-QJJR4-XV3QB-6VM33
Windows Server 2022 Standard: VDYBN-27WPP-V4HQT-9VMD4-VMK7H
Windows Server 2019 Datacenter: WMDGN-G9PQG-XVVXX-R3X43-63DFG
Windows Server 2019 Standard: N69G4-B89J2-4G8F4-WWYCC-J464C
Windows Server 2019 Essentials: WVDHN-86M7X-466P6-VHXV7-YY726
Windows Server 2016 Datacenter: CB7KF-BWN84-R7R2Y-793K2-8XDDG
Windows Server 2016 Standard: WC2BQ-8NRM3-FDDYY-2BFGV-KHKQY
Windows Server 2016 Essentials: JCKRF-N37P4-C2D82-9YXRT-4M63B
```

### Step 4 - Set KMS machine address
```bash
slmgr /skms 193.29.63.133:1688
```
Check out the latest server at [KMS servers](https://kms.msguides.com/)

### Step 5 - Activate your Windows
```bash
slmgr /ato
```
