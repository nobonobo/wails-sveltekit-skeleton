# wails-sveltekit-skeleton

## About

A template using SvelteKit

## prerequire

- go 1.21~
- npm 10~

```
go install github.com/wailsapp/wails/v2/cmd/wails@latest
wails init -n sample -t https://github.com/nobonobo/wails-sveltekit-skeleton
cd sample
```

## Building

To build this project in debug mode, use `wails build`. For production, use `wails build -production`.
To generate a platform native package, add the `-package` flag.

## Live Development

To run in live development mode, run `wails dev` in the project directory. In another terminal, go into the `frontend`
directory and run `npm run dev`. The frontend dev server will run on http://localhost:34115. Connect to this
in your browser and connect to your application.
