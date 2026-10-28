# AInvest visualization CDN assets

Standard Chart full browser bundle with all 18 preset themes.

```html
<script src="https://cdn.jsdmirror.com/gh/hwgshuai/ainvest-vis-cdn@main/aime/vis-skill-assets/standardchart/bundle.umd.min.js"></script>
```

Global: `ThsDataVStandardChart`. Includes ECharts and all existing preset families:
Mobile, THS, Lumi, AInvest App, AInvest PC, AInvest Terminal, PC, Wencai, and business treemap.

Omitting the theme selects AInvest Terminal light by default. All 18 themes remain available.

```js
ThsDataVStandardChart.init(element); // ainvest-terminal-pc-light
```

Choose another theme explicitly, for example:

```js
ThsDataVStandardChart.init(element, ThsDataVStandardChart.PRESET_THEME.AINVEST_PC_LIGHT);
ThsDataVStandardChart.init(element, ThsDataVStandardChart.PRESET_THEME.AINVEST_TERMINAL_PC_LIGHT);
```

The 16 non-Terminal themes use GitLab `A5-1376`, including THS PC light and dark.
The two Terminal themes retain the current Terminal implementation. Theme names retain their own meanings: `ainvest-pc-light` selects AInvest PC;
`ainvest-terminal-pc-light` selects Terminal. Terminal retains compact distribution sizing.
The optional existing `bundle.terminal.min.js` file remains a separate Terminal-only build;
use `bundle.umd.min.js` for the complete theme set.

Build metadata, theme list, file size and SHA-256: [manifest.json](aime/vis-skill-assets/standardchart/manifest.json).
Only distribution assets are published. No source maps or credentials are included.
Refresh the exact CDN file after publishing and compare downloaded bytes to the manifest.

Normal release workflow is test branch acceptance followed by promotion of identical bytes
to main. The Terminal-only asset is separate and unchanged by this release.
