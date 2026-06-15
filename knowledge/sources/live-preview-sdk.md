# Live Preview SDK source note

The SDK listens for Commentary parent messages and returns selected element metadata. It is browser-only code and should load only in review, preview, development, or explicitly opted-in builds.

## Safe fields

- `route`
- `selector`
- `fallbackSelector`
- `boundingRect`
- `viewport`
- `accessibleName`
- `textSnippet`
- optional component id, file, line, and build metadata

## Fields that must stay out

- cookies
- localStorage and sessionStorage values
- auth headers
- hidden input values
- token-like field values
- full DOM dumps
- private customer content copied into telemetry

## Support note

If the SDK is present but Commentary shows an origin mismatch, check the parent-origin allow list before asking engineering to debug selectors.
