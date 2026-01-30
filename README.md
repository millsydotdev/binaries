# GRID Binaries

This repository stores compiled GRID releases for all supported platforms.

## Purpose

The GRID Builder automatically uploads release artifacts to this repository:

- **Installers**: `.deb`, `.rpm`, `.dmg`, `.exe`  
- **Archives**: `.tar.gz`, `.zip`
- **Portable**: AppImage, portable executables

## Structure

Binaries are organized by release version and stored as GitHub Releases.

## Supported Platforms

### Linux

- x86_64 (AMD/Intel 64-bit)
- aarch64 (ARM 64-bit)
- armv7 (ARM 32-bit)

**Formats**: .deb, .rpm, .tar.gz, AppImage

### macOS  

- x86_64 (Intel)
- aarch64 (Apple Silicon)

**Formats**: .dmg, .zip

### Windows

- x86_64 (64-bit)
- aarch64 (ARM64)

**Formats**: .exe (installer), .zip (portable)

## Auto-Update

GRID clients check this repository for updates using metadata from the `versions` repository.

## Downloads

Visit the [official GRID website](https://grideditor.com) to download the latest version for your platform.

## Build Information

Binaries are built automatically by [GRID-BUILDER](https://github.com/GRID-NETWORK-REPO/GRID-BUILDER) using GitHub Actions.

## Verification

All releases include SHA-256 checksums. Verify downloads:

```bash
# Linux/macOS
sha256sum grid-*.tar.gz

# Windows (PowerShell)
Get-FileHash grid-*.exe -Algorithm SHA256
```

## License

GRID is released under the MIT License.
