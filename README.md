# ai-docs

[![npm version](https://img.shields.io/npm/v/@lxgicstudios/ai-docs.svg)](https://www.npmjs.com/package/@lxgicstudios/ai-docs)
[![npm downloads](https://img.shields.io/npm/dm/@lxgicstudios/ai-docs.svg)](https://www.npmjs.com/package/@lxgicstudios/ai-docs)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/lxgic-studios/ai-docs)](https://github.com/lxgic-studios/ai-docs/stargazers)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-blue)](https://www.typescriptlang.org/)


AI-powered JSDoc/TSDoc generator. Automatically document your exported functions, classes, and interfaces.

## What is ai-docs?

ai-docs is a CLI tool that adds professional documentation comments to your TypeScript and JavaScript code. It analyzes your exported functions, classes, and interfaces, then generates JSDoc or TSDoc comments without modifying your actual code logic.

## Why use it?

- Saves hours of manual documentation work
- Generates accurate param and return type descriptions
- Supports both JSDoc and TSDoc formats
- Non-destructive: only adds comments, never changes code

## Install

```bash
npm install -g ai-docs
```

## Setup

```bash
export OPENAI_API_KEY=sk-your-key-here
```

## Usage

```bash
# Preview docs for a directory (prints to stdout)
npx ai-docs src/ --style jsdoc

# TSDoc style
npx ai-docs src/ --style tsdoc

# Actually write the changes back to the files
npx ai-docs src/ --style jsdoc --write

# Single file
npx ai-docs src/utils.ts --style jsdoc

# Glob patterns work too
npx ai-docs "src/**/*.ts" --style tsdoc
```

## What it does

Reads each file, sends it to OpenAI, gets back the same file with doc comments added to all the exported stuff. It won't change your code. It just adds comments above functions, classes, interfaces, and types.

## Tips

- Run without `--write` first to preview what it'll do
- It skips files over 20KB (they'd blow the context window anyway)
- Automatically ignores node_modules and dist folders

## FAQ

**Does it modify my code logic?**
No. It only adds documentation comments above your functions and classes.

**What's the difference between JSDoc and TSDoc?**
JSDoc is the classic format. TSDoc is TypeScript-specific with stricter syntax. Pick based on your project.

**Can I run it on my whole codebase at once?**
Yes. Just point it at your src directory: `npx ai-docs src/ --style jsdoc --write`

**Does it work with JavaScript files?**
Yes. It supports both .ts and .js files.

## License

MIT - [LXGIC Studios](https://github.com/lxgicstudios)
