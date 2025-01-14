### 2.3.100-20220203 ISO image built on 2022/02/03



### Download and Verify

2.3.100-20220203 ISO image:  
https://download.securityonion.net/file/securityonion/securityonion-2.3.100-20220203.iso

MD5: 14705B2F2F9C973D944A4545449799C5  
SHA1: D73405BE3DE404DE19979B58DEA6F22F434E622D  
SHA256: 3DD54ACBFDE0047A5EA238415F025ADB6D6AAFF53BEE084A602327CB3242B580 

Signature for ISO image:  
https://github.com/Security-Onion-Solutions/securityonion/raw/master/sigs/securityonion-2.3.100-20220203.iso.sig

Signing key:  
https://raw.githubusercontent.com/Security-Onion-Solutions/securityonion/master/KEYS  

For example, here are the steps you can use on most Linux distributions to download and verify our Security Onion ISO image.

Download and import the signing key:  
```
wget https://raw.githubusercontent.com/Security-Onion-Solutions/securityonion/master/KEYS -O - | gpg --import -  
```

Download the signature file for the ISO:  
```
wget https://github.com/Security-Onion-Solutions/securityonion/raw/master/sigs/securityonion-2.3.100-20220203.iso.sig
```

Download the ISO image:  
```
wget https://download.securityonion.net/file/securityonion/securityonion-2.3.100-20220203.iso
```

Verify the downloaded ISO image using the signature file:  
```
gpg --verify securityonion-2.3.100-20220203.iso.sig securityonion-2.3.100-20220203.iso
```

The output should show "Good signature" and the Primary key fingerprint should match what's shown below:
```
gpg: Signature made Thu 03 Feb 2022 03:35:03 PM EST using RSA key ID FE507013
gpg: Good signature from "Security Onion Solutions, LLC <info@securityonionsolutions.com>"
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: C804 A93D 36BE 0C73 3EA1  9644 7C10 60B7 FE50 7013
```

Once you've verified the ISO image, you're ready to proceed to our Installation guide:  
https://docs.securityonion.net/en/2.3/installation.html
