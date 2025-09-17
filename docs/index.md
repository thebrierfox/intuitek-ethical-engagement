# Verifying Provenance

To verify the integrity of an IntuiTek¹ Provenance Pack:

1. Download the artifact and accompanying `.sha256` checksum file.
2. Compute the SHA256 hash of the downloaded file:
   - On macOS: `shasum -a 256 <filename>`.
   - On Linux: `sha256sum <filename>`.
3. Compare the computed hash to the value stored in the `integrity.sha256_hex` field of the `provenance_template.json` or the provided `.sha256` file.
4. Optionally verify the `.sig` signature with GPG:
   `gpg --verify <filename>.sha256.asc <filename>.sha256`
5. Review the provenance JSON for the `author`, `canonical_url`, and `license` fields; this identifies the source and terms of use.

For more details, see the instructions in `provenance/HASH_AND_SIGN_INSTRUCTIONS.md` within this repository.
