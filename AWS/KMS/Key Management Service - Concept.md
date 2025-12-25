
[[Key Management Service Core]]

KMS uses a strategy called _Envelope Encryption_ to handle large-scale data without overwhelming the KMS network.
- Request: A service _like RDS_ rquests a Data Key from KMS.
- Generation: KMS generates a plaintext Data Key and an encrypted version of that same Data Key.
- Encryption: The service uses the plaintext Data Key to encrypt your data and them immediately discards the plaintext key from memory.
- Storage: The service stores the encrypted Data Key alongside your data.
- Decryption: To read the data, the service send the encrypted Data Key back to KMS, which decrypts it and returns the plaintext key so the service can unlock your data.