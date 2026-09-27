# Nebula CLI

![build](https://img.shields.io/badge/build-passing-brightgreen) ![license](https://img.shields.io/badge/license-MIT-blue) ![version](https://img.shields.io/badge/version-1.4.0-orange)

A fast, zero-config command line tool for scaffolding and shipping modern web projects.

## Features

- Instant project scaffolding with sensible defaults
- Built-in dev server with hot reloading
- One-command production builds
- Plugin system for custom workflows

## Installation

```bash
npm install -g nebula-cli
nebula init my-app
cd my-app
nebula dev
```

## Usage

| Command | Description |
| --- | --- |
| `nebula init` | Create a new project |
| `nebula dev` | Start the dev server |
| `nebula build` | Build for production |

## How It Works

```mermaid
graph TD
    A[nebula init] --> B[Scaffold project]
    B --> C[nebula dev]
    C --> D{Happy with it?}
    D -->|No| C
    D -->|Yes| E[nebula build]
    E --> F[nebula build]
    F --> G[nebula build]
```

## Project Structure

```text
my-app/
├── src/
│   ├── components/
│   └── main.ts
├── public/
└── package.json
```

## Roadmap

- [x] Core scaffolding
- [x] Plugin API
- [ ] Remote templates
- [ ] Deploy targets

<details>
<summary>Advanced configuration</summary>

Create a `nebula.config.ts` file at the project root to override defaults.

</details>

> Nebula is under active development. Expect frequent releases.

## Contributing

Pull requests are welcome. Please open an issue first to discuss any major change.

---

## License

MIT © Nebula Contributors

```text
project/
├── src/
├── public/
└── package.json
```

![build](https://img.shields.io/badge/build-passing-brightgreen)

---

<details>
<summary>More information</summary>

Additional content.

</details>

```mermaid
graph TD
    N1["Start"]
    N2["Next step"]
    N129["Step 3"]
    N362["Step 4"]
    N2 --> N129
    N2 --> N1
    N2 --> N362
```

```mermaid
graph TD
    N1@{ shape: circle, label: "Start" }
    N2@{ shape: rounded, label: "Next step" }
    N345@{ shape: diamond, label: "Step 3" }
    N658@{ shape: rect, label: "Step 4" }
    N891@{ shape: cyl, label: "Step 5" }
    N1 --> N2
    N2 --> N1
    N2 --> N345
    N2 --> N658
    N658 --> N345
    N1 --> N658
```
