## 🏷️ Badges

![npm](https://img.shields.io/npm/v/ai-docs)
![Node.js](https://img.shields.io/badge/node-%3E%3D16.0.0-brightgreen)
![License](https://img.shields.io/npm/l/ai-docs)
![TypeScript](https://img.shields.io/badge/typescript-%3E%3D4.0-blue)

# Documentation generation and management utilities

Documentation generator. Creates comprehensive project documentation from code analysis and comments.

[![npm version](https://img.shields.io/npm/v/@lxgicstudios/ai-docs.svg)](https://www.npmjs.com/package/@lxgicstudios/ai-docs)
[![npm downloads](https://img.shields.io/npm/dm/@lxgicstudios/ai-docs.svg)](https://www.npmjs.com/package/@lxgicstudios/ai-docs)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/lxgicstudios/ai-docs)](https://github.com/lxgicstudios/ai-docs/stargazers)
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


🔗 [GitHub](https://github.com/lxgicstudios) · [Twitter](https://x.com/lxgicstudios)

 like this? We have 100+ on our  [github.com/lxgicstudios](https://github.com/lxgicstudios)


🔗 [GitHub](https://github.com/lxgicstudios) · [Twitter](https://x.com/lxgicstudios)

 like this? We have 100+ on our  [github.com/lxgicstudios](https://github.com/lxgicstudios)


🔗 [GitHub](https://github.com/lxgicstudios) · [Twitter](https://x.com/lxgicstudios)

 like this? We have 100+ on our  [github.com/lxgicstudios](https://github.com/lxgicstudios)


🔗 [GitHub](https://github.com/lxgicstudios) · [Twitter](https://x.com/lxgicstudios)

 like this? We have 100+ on our  [github.com/lxgicstudios](https://github.com/lxgicstudios)


🔗 [GitHub](https://github.com/lxgicstudios) · [Twitter](https://x.com/lxgicstudios)

 like this? We have 100+ on our  github.com/lxgicstudios


🔗  https://github.com/lxgicstudios ·  https://x.com/lxgicstudios

 like this? We have 100+ on our  github.com/lxgicstudios


🔗 [GitHub](https://github.com/lxgicstudios) · [Twitter](https://x.com/lxgicstudios)

 like this? We have 100+ on our  [github.com/lxgicstudios](https://github.com/lxgicstudios)






 [github.com/LXGIC-Studios](https://github.com/lxgicstudios)


- [npm Advanced SEO Guide](https://github.com/lxgicstudios/npm-seo-guide) - npm package optimization
- [AI Search Optimization](https://github.com/lxgicstudios/ai-seo-guide) - AI-powered SEO strategies

## 🚀 Built with ❤️ by LXGIC Studios

> This tool is part of the [lxgic studios](https://github.com/lxgicstudios) collection of AI-powered developer tools. We specialize in creating intelligent automation solutions that help developers build faster, smarter, and more efficiently.


**Discover more tools:** [lxgic studios GitHub](https://github.com/lxgicstudios)  
**Follow us on ** [@lxgicstudios](https://twitter.com/lxgicstudios)  
**Join our community:** [Discord Server](https://discord.gg/lxgicstudios)  

## 📄 License

MIT © 2025 LXGIC Studios. Built with ⚡ and AI.

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.


<div align="center">
  <p>
    <a href="https://github.com/lxgicstudios/sponsor">
      <img src="https://img.shields.io/badge/-Sponsor%20Us-%23EA4AAA?style=for-the-badge&logo=github&logoColor=white" alt="Sponsor LXGIC Studios">
    </a>
    <a href="https://twitter.com/lxgicstudios">
      <img src="https://img.shields.io/badge/-Follow%20Us-%231DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Follow LXGIC Studios">
    </a>
    <a href="https://discord.gg/lxgicstudios">
      <img src="https://img.shields.io/badge/-Join%20Discord-%235865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Join Discord">
    </a>
  </p>
</div>

---

Built by [LXGIC Studios](https://github.com/lxgicstudios)

🔗 [GitHub](https://github.com/lxgicstudios) · [Twitter](https://x.com/lxgicstudios)

💡 Want more free tools like this? We have 100+ on our GitHub: [github.com/lxgicstudios](https://github.com/lxgicstudios)


---

**Built by [LXGIC Studios](https://lxgicstudios.com)**

🔗 [GitHub](https://github.com/LXGIC-Studios) · [Twitter](https://x.com/lxgicstudios)

💡 Want more free tools like this? We have 100+ on our GitHub: github.com/LXGIC-Studios

---

**Built by [LXGIC Studios](https://lxgicstudios.com)**

🔗 [GitHub](https://github.com/LXGIC-Studios) · [Twitter](https://x.com/lxgicstudios)

💡 Want more free tools like this? We have 100+ on our GitHub: github.com/LXGIC-Studios