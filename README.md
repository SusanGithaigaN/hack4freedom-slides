# Making your first Bitcoin open-source contribution

Slidev presentation for first-time Bitcoin contributors. 

## Present

```sh
npm install
npm run dev
```

Open http://localhost:3030. The active deck is `hack4freedom.md`. Presenter view: http://localhost:3030/presenter/1. Speaker notes contain delivery prompts, source links and timing suggestions.

Press Space or Right to advance. Slides 2, 5, 10, 19, 21, 22, 26, 27 progressively reveal content. Slide 29 contains a ten-minute timer with start, pause, resume and reset controls. Slide 31 has interactive checkboxes. Neither component sends data or requires an account; state resets when the page reloads. Timer controls work in the slide view where they are clicked, rather than synchronizing between separate presenter/audience windows.

## Build and export

```sh
npm run build
npm run export
```

The build writes the presentation to `dist/hack4freedom/`; Netlify publishes `dist/`. The public path is `/hack4freedom/`. PDF/image export requires Slidev's optional `playwright-chromium` dependency and a Chromium installation. You can also use Slidev's browser export view. The original starter remains in `slides.md`, available with `npm run dev:starter`.


## Production subpath

```sh
npm run build
npm run preview
```

Open http://localhost:4173/hack4freedom/ to test the built presentation, including `/hack4freedom/5`, `/hack4freedom/overview` and `/hack4freedom/presenter/5`.

The build must retain the `hack4freedom.md` entry file as well as `--base /hack4freedom/`. The `--out dist/hack4freedom` option puts assets at their public URL paths. Netlify's scoped SPA rewrite supports direct slide links and refreshes; the root temporarily redirects to `/hack4freedom/`.

In the Netlify project, assign `boss.susangithaiga.com` as a custom domain and use the exact DNS target supplied by that project. DNS alone does not assign a domain to a hosting project. Confirm the production branch is `master`, that deployment is public, and that HTTPS is provisioned.

Hosting reference: [Slidev build and base-path documentation](https://sli.dev/guide/hosting).

