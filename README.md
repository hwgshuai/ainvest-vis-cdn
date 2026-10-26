# AInvest visualization CDN assets

Standard Chart browser bundle, including the current A5-1497 working tree fixes.

## Browser usage

```html
<script src="https://cdn.jsdelivr.net/gh/hwgshuai/ainvest-vis-cdn@main/aime/vis-skill-assets/standardchart/bundle.umd.min.js"></script>
```

Browser global: `ThsDataVStandardChart`. The bundle includes ECharts and supports UMD/browser loading.

For rollout, replace `@main` with the asset commit SHA to avoid stale CDN caches. The same path works with `https://cdn.jsdmirror.com/gh/`.

Build metadata and SHA-256: [manifest.json](aime/vis-skill-assets/standardchart/manifest.json).

Built from the local standard_chart checkout, including uncommitted A5-1497 fixes; sourceCommit is its base commit, not a claim of a clean source tree. Only distribution assets are published here. No source maps are included.
