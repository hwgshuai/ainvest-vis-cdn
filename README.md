# AInvest visualization CDN assets

Terminal-only Standard Chart browser bundle, including the current A5-1497 working tree fixes.

## Browser usage

```html
<script src="https://cdn.jsdmirror.com/gh/hwgshuai/ainvest-vis-cdn@main/aime/vis-skill-assets/standardchart/bundle.umd.min.js"></script>
```

Browser global: `ThsDataVStandardChart`. The bundle includes ECharts and supports UMD/browser loading.

The existing `@main` URL is retained. Refresh its JSDMirror cache after publishing and verify the response SHA-256 against manifest.json.

Build metadata and SHA-256: [manifest.json](aime/vis-skill-assets/standardchart/manifest.json).

Built from the local standard_chart checkout, including uncommitted A5-1497 fixes; sourceCommit is its base commit, not a claim of a clean source tree. Only distribution assets are published here. No source maps are included.

## Terminal-only distribution (2026-10-27)

Only `ainvest-terminal-pc-light` and `ainvest-terminal-pc-dark` are registered. `init(container)` defaults to Terminal light. For compatibility, the old init theme strings `ainvest-pc-light` and `ainvest-pc-dark` select the corresponding Terminal theme. Other theme implementations shared internally by Terminal are implementation dependencies, not separately registered themes.

Preferred URL:

```text
https://cdn.jsdmirror.com/gh/hwgshuai/ainvest-vis-cdn@main/aime/vis-skill-assets/standardchart/bundle.umd.min.js
```
