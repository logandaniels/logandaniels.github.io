## Build

Generate a production-ready build to the `_site` folder:

```
npx @11ty/eleventy
```

Or build and host on a local development server:

```
npx @11ty/eleventy --serve
```

Or you can run [debug mode](https://www.11ty.dev/docs/debugging/) to see all the internals.

## Deploy 

Currently deployed via Netlify, live at https://peanutbuttering.com

## How-to

* To add a link from one post to another: do a normal link, but with a relative path inside `content/`, e.g. `Click [here](blog/finite-resources.md)`.

## TODO

* Some way to easily add images to posts. S3 bucket?