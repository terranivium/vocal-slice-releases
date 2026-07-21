<!--
Copy this into the GitHub release description when publishing, then fill in the blanks.

The SHA-256 table is not optional: vocalslice.com tells users "every release lists a SHA-256 checksum
on its release page", and while the Windows build is unsigned that checksum is the only way anyone can
verify what they downloaded. Generate it with `npm run checksums` in the app repo AFTER building and
paste the output — don't retype the hashes.

Delete this comment block before publishing.
-->

## What's new

- …

## Downloads

| Platform | File |
| --- | --- |
| Windows 10/11 (64-bit) | `VocalSlice-Setup.exe` |
| Windows — portable, no install | `VocalSlice-Portable.exe` |
| macOS 11+ (universal) | `VocalSlice.dmg` |

<!-- Paste the `npm run checksums` output below, replacing this line and the table that follows. -->

### SHA-256 checksums

| File | Size | SHA-256 |
| --- | --- | --- |
| `VocalSlice-Setup.exe` | … | `…` |

Verify: `certutil -hashfile <file> SHA256` (Windows) · `shasum -a 256 <file>` (macOS)

## Notes

The installer and macOS build update themselves; the portable build doesn't — re-download it for new
versions.

Windows isn't code-signed yet, so SmartScreen will warn on first run — **More info → Run anyway**. The
checksum above is how you verify the download. macOS is signed and notarized.
