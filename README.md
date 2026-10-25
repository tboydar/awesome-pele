# Awesome Pele [![Awesome](https://awesome.re/badge.svg)](https://github.com/sindresorhus/awesome)

> Small, synchronous, dependency-free renderer that turns Mermaid diagrams into themeable SVG.

[English](README.md) · [繁體中文](README.zh-TW.md)

Pele is an MIT-licensed Mermaid-to-SVG renderer by [kepano](https://github.com/kepano), developed for Obsidian and usable anywhere. It targets the diagram types built into Mermaid 12.1.0, has no runtime dependencies, and themes diagrams with CSS variables. The repository, website, playground, documentation, security policy, and npm package are listed under Official.

This list is an independent community catalog. It is not an official Obsidian project, and it is not maintained by Obsidian or by kepano.

## Contents

- [Official](#official)
- [CLI & Tooling](#cli--tooling)
- [Ports & Bindings](#ports--bindings)
- [Agent Skills & AI](#agent-skills--ai)
- [Static Site & Docs Integrations](#static-site--docs-integrations)
- [Components & Frameworks](#components--frameworks)
- [Editors & Apps](#editors--apps)
- [Learning & Articles](#learning--articles)

## Official

- [Pele](https://github.com/obsidianmd/pele) - Source repository for the renderer.
- [Website](https://pele.run) - Project site, with documentation and a live example.
- [Playground](https://pele.run/playground) - In-browser editor for Mermaid source and the SVG Pele renders.
- [Examples](https://pele.run/examples) - Gallery of the diagram types Pele supports.
- [API](https://pele.run/api) - Reference for render(), mount(), entry points, and errors.
- [Theming](https://pele.run/theming) - CSS variables, fonts, and class names used to theme a diagram.
- [Compatibility](https://pele.run/compatibility) - Supported Mermaid 12.1.0 syntax, diagram types, and layout differences.
- [Security guide](https://pele.run/security) - Guidance for untrusted diagrams, links, icons, limits, and error display.
- [Security policy](https://github.com/obsidianmd/pele/blob/main/SECURITY.md) - How to report a vulnerability in Pele.
- [npm package](https://www.npmjs.com/package/pele) - Published package. Install it with `npm install pele`.

## CLI & Tooling

- [@ahmedelgabri/pele-cli](https://github.com/ahmedelgabri/pele-cli) - Command-line interface that validates Mermaid diagrams and renders them to themeable SVG without a browser.
- [pele2svg](https://github.com/iriyak/pele2svg) - Converts CSS-dependent Pele SVG into plain SVG that GToolkit and Skia can draw.
- [pele-animate](https://github.com/dkdev24/pele-animate) - Post-processor that reveals a Pele diagram one step at a time and adds icons.
- [pele-cli](https://github.com/IAL32/pele-cli) - Command-line renderer for themed SVG, a self-contained HTML page, or PNG. Requires Node.js 22 or newer.

## Ports & Bindings

- [bezel-mermaid](https://github.com/crabtalk/bezel/tree/main/crates/mermaid#readme) - Rust port of Pele 1.6.0 that renders Mermaid source to SVG without a browser or a JavaScript engine.
- [pele.cpp](https://github.com/MohammadRaziei/pele.cpp) - Dependency-free C++17 rewrite of Pele that aims to emit the same SVG for the same source.
- [pele-go](https://github.com/Broderick-Westrope/pele-go) - Go port of Pele 1.7.0 that aims for byte-identical SVG, with no cgo and no JavaScript runtime.
- [pele.mbt](https://github.com/Omochice/pele.mbt) - MoonBit port of Pele that aims for the same SVG, with a Typst package that runs it as WebAssembly.
- [pele-rs](https://github.com/vijayksingh/pele-rs) - Independent Rust Mermaid engine, with Swift and WebAssembly bindings, implementing the diagram families from Pele 1.6.0.
- [peler](https://github.com/eli-daniels/peler) - R package that runs Pele in V8 for SVG output, Quarto, R Markdown, and Shiny.

## Agent Skills & AI

- [oh-my-pele](https://github.com/tboydar/oh-my-pele) - AI-scanned, multi-level architecture diagrams for a codebase, rendered locally with Pele and compatible with oh-my-mermaid `.omm` files. Work in progress.
- [pele-agent-plugin](https://github.com/ossianravn/pele-agent-plugin) - Live browser page of plans and architecture drawn with Pele for Claude Code and Codex.
- [pele-skill](https://github.com/jpmanson/pele-skill) - Agent skill that renders Mermaid diagrams to SVG with Pele and no browser. Loads in Claude Code, Hermes Agent, and OpenCode.
- [pele-skill](https://github.com/maitretofu/pele-skill) - OpenCode skill that renders Mermaid to SVG and PNG with Pele and retries after a parse error.
- [pi-pele](https://github.com/Wade11s/pi-pele) - Pi extension that renders Mermaid with Pele and rasterizes the SVG to PNG for the terminal.

## Static Site & Docs Integrations

- [astro-pele](https://github.com/Aaron-212/astro-pele) - Astro integration and Sätteri plugin that render Mermaid diagrams with Pele in the browser.
- [bookstack-pele](https://github.com/felixyman/bookstack-pele) - Renders Mermaid code blocks in BookStack on the server with Pele, including PDF and HTML exports.
- [discourse-pele-theme-component](https://github.com/discourse/discourse-pele-theme-component) - Discourse theme component that renders Mermaid code blocks in posts and chat with Pele.
- [dokuwiki-pele](https://github.com/v4ltages/dokuwiki-pele) - DokuWiki plugin that renders Mermaid diagrams with Pele.
- [docusaurus-theme-pele](https://github.com/kywk/docusaurus-kit/tree/main/packages/theme-pele#readme) - Docusaurus theme that renders Mermaid diagrams to themeable SVG with Pele.
- [@erduotong/satteri-pele](https://github.com/erduotong/satteri-pele) - Sätteri plugin that renders Mermaid diagrams with Pele, including during static generation.
- [mdbook-pele](https://github.com/ld3z/mdbook-pele) - mdBook preprocessor that renders Mermaid diagrams with Pele.
- [pele-markdown](https://github.com/yue1123/pele-markdown) - Build-time Mermaid-to-SVG plugins for markdown-it, marked, and remark, with no client-side JavaScript.
- [pele-rehype](https://github.com/WyattAu/pele-rehype) - Rehype plugin that renders Mermaid fences with Pele in Astro, Starlight, and other unified pipelines.
- [pele-rustdoc](https://github.com/explodingcamera/pele-rustdoc) - Rust macro that embeds Mermaid diagrams in rustdoc and renders them in the browser with Pele.
- [@riebeckite/plugin-mermaid-pele](https://github.com/Rerurate514/riebeckite/tree/main/packages/plugins/mermaid-pele#readme) - Renders Mermaid code blocks to static SVG with Pele in Riebeckite.
- [satteri-pele](https://github.com/minumarapid/satteri-pele) - Sätteri plugin that converts Mermaid code blocks to SVG with Pele at build time.
- [slidev-addon-pele](https://github.com/arthurbm/slidev-addon-pele) - Slidev addon that draws Mermaid diagrams with Pele and reveals them step by step.
- [sphinx-pele](https://github.com/python-project-templates/sphinx-pele) - Sphinx extension that renders Mermaid directives, MyST fences, and external Mermaid files with Pele.
- [theme-pele](https://github.com/Cecilapp/theme-pele) - Cecil component theme that renders page Mermaid diagrams to SVG with Pele.
- [vitepress-plugin-pele](https://github.com/miswanting/vitepress-plugin-pele) - Renders Mermaid diagrams in VitePress at build time with Pele and no client-side JavaScript.

## Components & Frameworks

- [@bigmistqke/canon-plugin-pele](https://github.com/bigmistqke/skills/tree/main/packages/canon-plugin-pele#readme) - Draws the derivations of a Canon document as a graph rendered with Pele.
- [@bobril/mdx-pele](https://github.com/bobril/mdx-pele) - Renders Mermaid code blocks in Bobril MDX with @bobril/pele.
- [@bobril/pele](https://github.com/bobril/pele) - Bobril component that renders Mermaid syntax to SVG with Pele.
- [comark-pele](https://github.com/farnabaz/comark-pele) - Comark parse plugin, plus HTML, ANSI, Vue, React, Svelte, and Angular components, that renders Mermaid with Pele.
- [@docs.plus/extension-mermaid](https://github.com/docs-plus/docs.plus/tree/main/extensions/extension-mermaid#readme) - Tiptap extension that draws Mermaid code blocks as live SVG with Pele.
- [@maxtune/streamdown-pele](https://github.com/MaxtuneLee/streamdown-pele) - Streamdown adapter that renders Mermaid code blocks with Pele.
- [streamdown-pele](https://github.com/farnabaz/streamdown-pele) - Streamdown plugin that renders Mermaid code blocks with Pele in place of @streamdown/mermaid.
- [@tooee/mermaid-pele](https://github.com/gingerhendrix/tooee/tree/main/packages/mermaid-pele#readme) - Opt-in Tooee renderer that draws Mermaid fences with Pele and rasterizes them for the terminal.

## Editors & Apps

- [Diagram Studio](https://github.com/QAbot-zh/diagram-studio) - Browser diagram workbench that renders with Mermaid or Pele and exports SVG or PNG.
- [dsh-pele](https://github.com/hesheng01/dsh-pele) - DeepSeek Harness integration that accepts Mermaid through a pele_draw tool and shows inline SVG cards rendered with Pele.
- [dsh-pele](https://github.com/Yjsmall/dsh-pele) - Renders Mermaid code blocks in DeepSeek Harness assistant messages with Pele, including themes and zoom.
- [dsh-pele-mermaid](https://github.com/Farewe1ll/dsh-pele-mermaid) - DeepSeek Harness bundle plugin that renders Mermaid in web chat with Pele without patching Harness source.
- [dsh-pele-mermaid](https://github.com/lsy1998/dsh-pele-mermaid) - Renders Mermaid fences in the DeepSeek Harness web UI with Pele, including a code and diagram toggle and SVG export.
- [Eos](https://github.com/campfireshuffle/eos) - Local-first Mermaid editor rendered with Pele, stored in the browser, and open to agents over WebMCP.
- [Kilauea](https://github.com/prdlk/kilauea) - Visual editor for Pele diagrams. Change labels, shapes, and nodes on the rendered diagram.
- [Mermaid Pele Preview](https://github.com/pdanpdan/mermaid-pele-preview) - Visual Studio Code extension that previews Mermaid files and Markdown code blocks with Pele, including zoom, pan, and editor themes.
- [Mermaid Viewer](https://github.com/mmattia09/mermaid-viewer) - Live preview for Mermaid files in the browser and in Visual Studio Code. Pele is the default engine, and Mermaid.js is available for comparison.
- [ob-pele](https://github.com/wangjia15/ob-pele) - Obsidian plugin that renders Mermaid and Pele fences with Pele, with themes, live preview, and zoom.
- [Pele for Paseo](https://github.com/sojuhub/paseo-plugin-pele) - Renders Mermaid and Pele fences as interactive SVG inside Paseo chat, with zoom, pan, source view, and fullscreen.
- [pele.live](https://github.com/Akshad135/pele-live) - Browser playground that renders Mermaid locally with Pele.
- [pele-mermaid](https://github.com/xiangyuio/zcode-plugins/tree/main/plugins/pele-mermaid#readme) - ZCode plugin that renders Mermaid diagrams in a conversation as inline SVG with Pele.
- [Pele Note](https://github.com/ogaogamirai/pele-note) - Single-file Markdown and Mermaid studio, plus a command-line SVG converter, both using Pele.
- [Pele Preview](https://github.com/pskchai/vscode-pele-preview) - Visual Studio Code preview for Mermaid files, rendered with Pele.
- [Pele Studio](https://github.com/l-velazquez/pele-studio) - Browser editor for writing, previewing, and exporting diagrams rendered with Pele.
- [roam-pele](https://github.com/ujuc/roam-pele) - Renders Mermaid diagrams in Roam Research with Pele and lays them out again when the block width changes.
- [Siren](https://github.com/plwg/siren) - Minimal browser editor that renders Mermaid diagrams with Pele.

## Learning & Articles

- [pele.wiki](https://pele.wiki) - Independent guides and live demos for Pele. Not affiliated with Obsidian or kepano.

## Footnotes

Ports, bindings, and plugins name the Pele version they were written against. Those targets can lag the current release. Check the project itself before depending on byte-identical output.

## Contributing

Please read the [contributing guide](contributing.md) before opening a pull request, and update `README.zh-TW.md` when an entry changes.
