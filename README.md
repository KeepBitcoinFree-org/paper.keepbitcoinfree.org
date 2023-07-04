# KeepBitcoinFree.org Paper Wallet

The KeepBitcoinFree.org Paper Wallet is a client-side Bitcoin Cash (BCH) wallet generator producing customizable paper wallets.

The KeepBitcoinFree.org Paper Wallet is based on the open source [bitaddress.org repository.](https://github.com/pointbiz/bitaddress.org) Private Keys are generated client-side and can be used offline. For better security, download a local copy and run on an offline, air-gapped machine. 

The bitaddress.org software is available under The MIT License (MIT) Copyright (c) 2011-2013 bitaddress.org

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## To Run Offline

To run offline, you can simply download the zip file, extract it, turn off your Wifi/Ethernet connection, and then open index.html. 

### If you want to verify authenticity of the zip file - 

Clone the git repo, or directly download the zip file, signature & public key (into the same dir) and verify the signature using GPG / PGP software. 

On macosx with GPG Keychain (Other PGP implementations will use similiar processes) - 

- Right click on the "Zatoshi_Nakamoto_AF85D78B_Public_Key" file > Services > OpenPGP: Import Key from File

- Right click on the paper.keepbitcoinfree.org.zip file > Services > OpenPGP: Verify Signature of File

The GPG Services - Verification Results should show a checkmark for a Trusted Signature that matches the provided Public Key for the paper.keepbitcoifree.org.zip file.

You can also verify that the zip file has not been altered since it was last updated by KeepBitcoinFree-org. To verify the shasum on the paper.keepbitcoinfree.org.zip file, run the below command on the file and compare it to the shasum.txt file included (or the shasum listed below): 

- shasum -a 256 paper.keepbitcoinfree.org.zip
4d169efa1ae49db4f050c0eac6956117cc588179795c52caa51f6bc836a8fbca  paper.keepbitcoinfree.org.zip