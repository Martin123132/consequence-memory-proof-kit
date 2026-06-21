# Artifact Hashes

Published: 2026-06-21

This page records public hash commitments for private `v0.8.0` Consequence Memory release artifacts.

The hashes are published so a later reviewer can verify that the same private artifacts existed at this public proof-kit checkpoint. The artifacts themselves remain private unless access is granted separately in writing.

## Private Release

| Field | Value |
| --- | --- |
| Engine release | `v0.8.0` |
| Private repository | `Martin123132/consequence-memory` |
| Tag target commit | `7ed3c35f2a43cb86df034f90ea9060239fa43e3c` |

## Package Artifact Commitments

| Artifact | Size | SHA-256 |
| --- | ---: | --- |
| `consequence_memory-0.8.0-py3-none-any.whl` | 53,128 bytes | `45f55d2e8b8299501b6119187a7dec4bac6c24036d0b5b2e70dbd6af3ee4555a` |
| `consequence_memory-0.8.0.tar.gz` | 56,820 bytes | `ee11395ad10887871bb34f8517bce83056931e7977c61fd27b240e25128f85db` |

## Evidence Bundle Commitment

Private evidence bundle label:

`v0.8.0-final-20260621`

| Field | Value |
| --- | ---: |
| File count | 13 |
| Total bytes | 78,208 |
| Tree SHA-256 | `96910551567ab46603b0d9a77aaf69a0080879682662573a44f4f86414ed24c0` |

Tree hash method:

1. Recursively list files in the private evidence bundle.
2. Sort by relative path.
3. For each file, build one line as `relative_path<TAB>byte_length<TAB>file_sha256`.
4. Join lines with LF.
5. Compute SHA-256 over the UTF-8 bytes of that joined text.

This method lets a reviewer with private access verify the evidence bundle without publishing the bundle contents in this public repository.

## Boundary

These hash commitments do not grant source access, commercial use, patent rights, trademark rights, redistribution rights, hosted-service rights, model-training rights, or permission to reproduce the private engine.

See [LICENSE.md](../LICENSE.md), [COMMERCIAL_USE.md](../COMMERCIAL_USE.md), and [NDA_ACCESS.md](../NDA_ACCESS.md).
