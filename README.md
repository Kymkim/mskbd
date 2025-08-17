# MSKBD - Modularly Simple KeyBoarD

> [!WARNING]  
> This is the inital commit for this project just to fill in the repo with contents - If you want to see progress being made in the project you might want to see the `dev` branch. All progess is made there before a stable version is ready :)

A customizable modular keyboard system where each key cluster is its own module, connected through a grid-like commnication. The goal is to create a flexible keyboard that can scale, reconfigure layouts, and support hot-swapping modules.

## Features
- 🧩 **Modular design** — attach modules in any direction
- 🎛️ **Configurable firmware** — master + module code, easily updated
- ⚡ **Hotplug detection** — modules can be discovered dynamically

## Repo Structure
```
├─firmware/ - Embedded code for the core system
├─hardware/ - Schematics and PCB layouts
├─software/ - Host tools (keymap editor, etc.) (not yet implemented - soon hopefully!)
├─docs/ - Design notes, communication protocol, build guides
└─assets/ - Renders, diagrams, and media
```

## Branch Structure
```
main              # Stable, production-ready code (only tested & reviewed changes go here)
│
├─ dev            # Integration branch for features; "staging" area before merging to main
│  ├─ feature-1     # New features, experiments, improvements, or PCB uploads     
│  ├─ feature-2
│  └─ hardware1
│
├─ hotfix/        # Quick fixes for urgent bugs in main
│   └─ hotfix/usb-detection
│
└─ docs/          # Documentation updates (can also just use feature/docs-*)
    └─ docs/protocol-update
```


## License
[MIT](LICENSE) – free to use, modify, and share.
