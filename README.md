# Phisher Cloud Repo (PopcornPlay / CloudStream)

77+ extensions mirrored from phisher98/cloudstream-extensions-phisher with both `.cs3` and `.jar` files.

## Import URL

**PopcornPlay deep link:**
```
popcornplayrepo://raw.githubusercontent.com/amarsingh820/phishercloud/main/repo.json
```

**Manual / CloudStream:**
```
https://raw.githubusercontent.com/amarsingh820/phishercloud/main/repo.json
```

## Upload

Extract this zip and upload ALL files (`.cs3`, `.jar`, `repo.json`, `plugins.json`) to the **root** of `amarsingh820/phishercloud` on `main` branch. Both .cs3 and .jar are required — newer app forks (PopcornPlay) try the `.jar` first; CloudStream uses `.cs3`.

## REMADE / FIX NOTES (v3)

Problem found from the app screenshot: plugin list was visible, but tapping download showed **Error**.

Fixed in this ZIP:
- Rebuilt all `.cs3` plugin files for PopcornPlay v38 package rename.
- Rewrote plugin bytecode references from `com.lagradost.cloudstream3` to `com.popcornplay.app`.
- Also patched all bundled `.jar` files, because PopcornPlay v38 tries JAR downloads first for many plugins.
- Regenerated every changed plugin `fileSize`, `fileHash`, `jarFileSize`, and `jarHash` in `plugins.json`.
- App ZIP is not changed; only extension/repo ZIP is remade.

Upload instructions:
1. Extract this ZIP.
2. Upload/replace every file in the GitHub repo root: `.cs3`, `.jar`, `plugins.json`, `repo.json`, and this README.
3. In PopcornPlay, remove the old repo/cache if needed and add/import the repo again.

Important: if only `repo.json` is uploaded and the plugin files are not replaced on GitHub, the app will still download old broken files.

