# gas-mime-types

TypeScript type declarations for the Google Apps Script `MimeType` enum.

Provides type completion for `MimeType` without shipping any runtime JavaScript. References to `MimeType.GOOGLE_DOCS` are preserved as-is in compiled output, using the native GAS global at runtime.

## Installation

```bash
npm install gas-mime-types
```


## Usage

No import needed — `MimeType` is available globally:

```ts
const file = DriveApp.getFilesByType(MimeType.GOOGLE_DOCS);
```

Compiled output:

```js
const file = DriveApp.getFilesByType(MimeType.GOOGLE_DOCS);
```

## Note

If you already use `@types/google-apps-script`, you do not need this package — `MimeType` is already declared there.
