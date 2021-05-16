# Encryption
- Encoding a message so only authorized partices can access
- Sender uses secret key and encryption algo, pt to ct
- Receiver uses secret key and decryption algo, ct to pt

## Symmetric Encryption
- Same key between sender and receiver
- Fast processing
- Low security once key is intercepted
- Eg: AES

## Asymmetric Encryption
- One public key, one private key
- One cannot be derived from the other
- SLower but more secure
- Eg: RSA

## Digital Signature
- Encryption and decryption technology that secures data, and helps to verify authenticity of document
- Commonly used on internet, emails, blockchains
- Authentication: Message created by known sender
- Non-repudiation: Sender cannot deny sending message
- Integrity: Message not altered in transit

## Hashing
- Generate short string of text (hash) from any size of data
- NOT encryption
- Impossible to recover original data from hash
- Eg: SHA-256, Md5

# Authentication
- Validates identity of user (Captcha is NOT authentication)
- Users prove identity by providing credentials
- Something you know/have/are
- Eg: Password, OTP Fob, Biometric