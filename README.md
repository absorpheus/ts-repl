# ts-repl

ts-repl is a super-fast environment for exploring and experimenting with TypeScript on your local machine. Designed to run seamlessly within VSCode, it enables quick feedback and smooth experimentation.

## Features

- Blazing-fast transpilation: Built on SWC for near-instant code transformations.
- Local integration: Designed to work directly within VSCode, leveraging your local setup.
- Simple and lightweight: A minimal yet powerful setup for experimenting with TypeScript.

## Installation

### Prerequisites

- Install [Node.js](https://nodejs.org/) (LTS or Current)
- Install [VSCode](https://code.visualstudio.com/download)

### Installation

First, install dependencies with `npm`.
```bash
npm install
```

Open the project in VSCode:
```bash
code .
```

### Keybindings

To achieve functionality similar to Replit, add these entries to your keybindings.json file.

```json
[
  {
    "key": "cmd+enter",
    "command": "workbench.action.tasks.runTask",
    "args": "build",
    "when": "config.workspaceKeybindings.repl.enabled"
  },
  {
    "key": "cmd+enter",
    "command": "workbench.action.tasks.restartTask",
    "args": "build",
    "when": "config.workspaceKeybindings.repl.enabled && taskRunning"
  }
]
```

Your TypeScript playground is now ready to use directly in VSCode!

## Usage

1. Open `src/index.ts`

2. Start experimenting with TypeScript syntax and features.

3. Update results on demand with Command+Enter, similar to Replit.


## Contributing

We welcome contributions! If you have ideas for new features, improvements, or bug fixes, feel free to open an issue or submit a pull request.
