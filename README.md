# react-intl-tel-input UMD import issue sample project

Sample project to demonstrate react-intl-tel-input issue #[253](https://github.com/patw0929/react-intl-tel-input/issues/253).

This project is built with [Next.js](https://nextjs.org/), to demonstrate server vs. browser behavior.

## Repro

From the project folder, build and run the project in dev mode:

```bash
npm install # or `yarn` — lock files are provided for both
npm run dev # or `yarn dev`
```

Then, from a browser, navigate either:

- [http://localhost:3000/attempt-to-import](http://localhost:3000/attempt-to-import) — errors with _“Unhandled Rejection (ReferenceError): window is not defined”_ on import during server-side rendering
- [http://localhost:3000/](http://localhost:3000/), then click _“Attempt to import react-intl-tel-input browser-side”_ — works thanks to import during browser-side rendering
