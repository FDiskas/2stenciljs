# 2StencilJS

A browser-based tool that converts frontend framework components into [StencilJS](https://stenciljs.com/) web components.

## Supported Frameworks

- **React** (JSX) — class and functional components
- **Angular** (TypeScript) — decorator-based components
- **Vue** (SFC) — single-file components

## How It Works

Paste a component from any supported framework into the left editor pane, select the source framework, and get the equivalent StencilJS component in the right pane.

The converter runs entirely in the browser using [Babel standalone](https://babeljs.io/docs/babel-standalone) for AST parsing and transformation. No server required.

## Features

- Live syntax highlighting via [highlight.js](https://highlightjs.org/)
- Maps framework-specific lifecycle hooks to StencilJS equivalents (e.g., `componentDidMount` → `componentDidLoad`)
- Converts state, props, and event patterns to StencilJS decorators (`@State`, `@Prop`, `@Event`)
- Handles template syntax conversion (Angular `{{ }}`, Vue templates → JSX)

## Usage

Open [https://fdiskas.github.io/2stenciljs/](https://fdiskas.github.io/2stenciljs/) paste component source code on the left. Hit "Convert" to see the StencilJS equivalent on the right.
