# Next.js Build Error: Unexpected token in JSX

This repository demonstrates a Next.js build error caused by a seemingly innocuous comment in JSX. The error occurs when the comment contains characters outside the Basic Multilingual Plane (BMP). This issue is not always caught by linters and can be difficult to debug.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run build`.

You should see a build error similar to this:

```
SyntaxError: Unexpected token
```

## Solution

The solution is to remove or replace the offending character in the comment.