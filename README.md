# EncryptDecryptProtect v1.2026.911

**ENCRYPT • DECRYPT • PROTECT • VERIFY**

**Official home:** [EncryptDecryptProtect.com](https://EncryptDecryptProtect.com)  
**Developer:** [ArtisticAIBytes.com](https://ArtisticAIBytes.com)

EncryptDecryptProtect v1.2026.911 by **Artistic AI Bytes** is an all-in-one encryption, decryption, hashing, checksum, integrity-verification, compression, reporting, automation, benchmarking and data-protection application for Windows 64-bit.

Encrypt and decrypt files, folders and text using **AES-256-GCM, XChaCha20-Poly1305, ChaCha20-Poly1305 and AES-256-GCM-SIV**, with Zstandard, Brotli, Gzip and Deflate compression. EncryptDecryptProtect supports hash and checksum creation and verification, Folder Hash Reports and comparison, Original vs. Decrypted integrity verification, reusable post-decryption hash reports, Batch Tasks, APP History, and encryption/compression benchmarking across 14 profiles.

The current release is distributed as a **single self-contained Windows 64-bit `.exe`** with no separately installed dependencies or runtimes required.

> **First Public Release: September 11, 2026**

## Download

**Windows 64-bit:** [EncryptDecryptProtect-Windows-x64.exe](https://github.com/ArtisticAIBytes/EncryptDecryptProtect/releases/download/v1.2026.911/EncryptDecryptProtect-Windows-x64.exe)

**GitHub Release:** [EncryptDecryptProtect v1.2026.911](https://github.com/ArtisticAIBytes/EncryptDecryptProtect/releases/tag/v1.2026.911)

**ModDB mirror:**  
https://www.moddb.com/company/artistic-ai-bytes/downloads/encryptdecryptprotect-windows-x64

The executable is distributed as a compiled binary. **Source code is not included in this public repository.**

## Modern Authenticated Encryption

EncryptDecryptProtect supports four authenticated-encryption algorithms:

- **AES-256-GCM**
- **XChaCha20-Poly1305**
- **ChaCha20-Poly1305**
- **AES-256-GCM-SIV**

Users can choose the encryption algorithm appropriate for the task rather than being locked to a single cipher.

## File, Folder and Text Protection

EncryptDecryptProtect can protect individual files, complete folder structures and text. Folder operations preserve directory structure for restoration during decryption.

Protected content is stored in the **EDPF encrypted container format**, which combines encrypted content with the metadata and integrity information required for restoration and verification.

## Secret Key Workflows

EncryptDecryptProtect provides multiple Secret Key workflows, including the **EncryptDecryptProtect 256-bit Algorithm** remindable Secret Key workflow and **Custom User Secret Keys** supporting up to **1,000,000 characters**.

An **Image Secret Key Reminder** can be associated with protected content as a memory aid. Reminder images are public information stored with the EDPF and must never contain the actual Secret Key, passwords, credentials or other sensitive information.

## Encryption + Compression

EncryptDecryptProtect includes **14 compression profiles**:

- Zstandard Fast / Balanced / Maximum
- Brotli Fast / Balanced / Maximum
- Gzip Fast / Balanced / Maximum
- Deflate Fast / Balanced / Maximum
- Raw Deflate
- No Compression

Compression is optional and can be selected according to speed, output-size or workload requirements.

## 38 Hash and Checksum Methods

EncryptDecryptProtect supports **38 hash and checksum methods**:

**MD:** MD2, MD4, MD5  
**SHA-1:** SHA-1  
**SHA-2:** SHA-224, SHA-256, SHA-384, SHA-512, SHA-512/224, SHA-512/256  
**SHA-3:** SHA3-224, SHA3-256, SHA3-384, SHA3-512  
**SHAKE:** SHAKE128, SHAKE256  
**BLAKE:** BLAKE2b-512, BLAKE2s-256, BLAKE3  
**RIPEMD:** RIPEMD-160  
**Whirlpool:** Whirlpool  
**CRC:** CRC-8, CRC-16, CRC-24, CRC-32, CRC-32C, CRC-64  
**Checksums:** Adler-32, Fletcher-16, Fletcher-32  
**xxHash:** xxHash32, xxHash64, XXH3-64, XXH3-128  
**FNV:** FNV-1 32-bit, FNV-1a 32-bit, FNV-1 64-bit, FNV-1a 64-bit

Hash/checksum workflows are available for **files, folders and text**.

## Folder Hash Reports and Comparison

EncryptDecryptProtect can create reusable **`.EDPhashReport`** integrity snapshots for directory trees, including files, folders and **empty folders**.

Compatible reports can be compared to identify matching, changed, new/present and missing/absent entries. Search is available for large comparisons so users can locate file names, paths, statuses and hash values efficiently.

## Original vs. Decrypted Verification

A central design principle of EncryptDecryptProtect is:

**Do not simply decrypt the data. Verify what came back.**

When integrity information is available in an EDPF container, EncryptDecryptProtect can verify restored content against its original recorded state and display an **Original vs. Decrypted Hash Comparison**.

After decrypting and verifying a folder, EncryptDecryptProtect can also create a reusable `.EDPhashReport` from the restored result, including the complete restored directory structure and empty folders.

## Batch Tasks and APP History

**Batch Tasks** provide reusable workflows for repeated operations, with validation and Batch Logs for actual executions. `.EDPbatchTask` files can optionally store Custom User Secret Keys only when explicitly permitted by the user and should be protected appropriately when they contain sensitive information.

**APP History** provides an operational record of relevant application activity. History data can be saved, imported and integrated with validation and duplicate handling.

## Built-in 100 MiB Benchmark

EncryptDecryptProtect includes a deterministic **100 MiB (104,857,600-byte) Standard Benchmark** generated at runtime. It exercises the real encryption/decryption pipeline across all 14 compression profiles and measures encryption time, decryption time, resulting EDPF size and restored-data integrity.

Users can also select their **own file to benchmark**, save benchmark reports and compare benchmark results side-by-side across runs, systems and EncryptDecryptProtect versions.

## v1.2026.911 Highlights

- File, folder and text encryption/decryption
- Four authenticated-encryption algorithms
- EDPF encrypted containers
- Multiple Secret Key workflows
- Custom User Secret Keys up to 1,000,000 characters
- Image Secret Key Reminder
- 14 compression profiles
- 38 hash and checksum methods
- File, folder and text hashing
- Folder Hash Reports and comparison
- Searchable integrity comparisons
- Original vs. Decrypted verification
- Post-decryption `.EDPhashReport` creation
- Empty-folder preservation in folder integrity reports
- Batch Tasks and Batch Logs
- APP History
- Deterministic 100 MiB Standard Benchmark
- User-selected-file benchmarking
- Benchmark report saving and comparison
- Round-trip benchmark integrity verification
- Self-contained Windows 64-bit executable
- No separately installed dependencies or runtimes required

## Roadmap

### v2 CLI

CLI support will allow **developers, scripts, automated workflows and AI agents to communicate directly with the EncryptDecryptProtect executable using only a few commands and receive structured results**. Planned operations include hashing files, verifying hashes, encrypting, decrypting, archiving, processing folders, running Batch Tasks and much more without manually operating the graphical interface.

### v3 Messaging

Planned encrypted messaging workflows with Telegram, Discord, Slack, Microsoft Teams and WhatsApp, plus additional messaging platforms where suitable integration interfaces are available.

### v4 Akukaracha

Seven layers of 256-bit authenticated encryption: a **1792-bit multi-layer architecture**. Even UFOs will be jealous. 👽

### Platforms

**Available now:** Windows 64-bit  
**Planned:** Linux • macOS • iOS • Android

---

## Official Home

**EncryptDecryptProtect:** [EncryptDecryptProtect.com](https://EncryptDecryptProtect.com) — the official home of EncryptDecryptProtect.  
**Developer:** [ArtisticAIBytes.com](https://ArtisticAIBytes.com) — Artistic AI Bytes.

## ENCRYPT. DECRYPT. PROTECT. VERIFY.

**Protect the original. Verify it. Encrypt it. Decrypt it. Verify it again. Keep the evidence. Compare it later.**

**EncryptDecryptProtect v1.2026.911**  
**First Public Release — September 11, 2026**  
**Developed by [Artistic AI Bytes](https://ArtisticAIBytes.com) (Lead Developer: UHDk1ng(AIk1ng) + ChatGPT(GPT-5.6 Sol))**

**Windows first. More platforms next. EncryptDecryptProtect has only begun. 😼🚀**