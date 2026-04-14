ReNotes Release repo

ReNotes is a desktop Sticky-Notes app I built as a side project, after years of frustriations of text, note and important data not syncing/saving using popular Sticky note options.

It is built with privacy in mind, while also being fast, offline-first, and end-to-end encrypted.

Built with Electron, React, TypeScript and Radix UI, backed by Firebase (Auth, Firestore, Cloud Functions) for optional account-based sync.

Every note is encrypted client-side with AES-GCM using a key derived from the user's password via PBKDF2, the server never sees plaintext. Notes work fully offline and sync when signed in.

Proper Electron security architecture: contextIsolation, preload-based IPC bridge, no nodeIntegration in the renderer, input-validated main process handlers.

Multi-window support,, pin-on-top, per-note locking, auto-updater, and a built distributable for direct download plus a separate Microsoft Store build.
