# Ethical Engagement Governance & Provenance Pack

This repository contains the IntuiTek¹ Ethical Engagement Governance framework and provenance pack. It includes:

- `intuitek_provenance_pack_v1.zip` – the full provenance and governance pack.
- `docs/` – a simple static site describing how to verify provenance and other information.

## How to Verify Provenance

To verify the integrity of a downloaded IntuiTek¹ provenance pack:

1. Compute the SHA256 checksum of the downloaded file using `sha256sum` (Linux) or `shasum -a 256` (macOS).
2. Compare the result to the `sha256_hex` value stored in the `integrity.sha256_hex` field of the provenance JSON or provided `.sha256` file.
3. Optionally verify any `.sig` signature with GPG.
4. See `docs/index.md` or the `provenance` folder within the pack for detailed instructions.

All artifacts are licensed under CC-BY-4.0. For attribution or questions, contact kyle@intuitek.ai.
