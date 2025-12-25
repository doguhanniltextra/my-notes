
[[Key Management Service - Concept]]

- CloudTrail Integration: Every time a key is used, an entry is made in _AWS CloudTrail_. This provides a perfect audit trail of who accessed what data and when.
- Automatic Rotation: You can enable annual rotation for Customer Managed Keys. KMS will generate new cryptographic material while keeping the old material available to decrypt existing data.
- FIPS 140-2 Level 3: KMS HMs are validated under the FIPS 140-2 program, ensuring a high level of physical and logical security for your keys.