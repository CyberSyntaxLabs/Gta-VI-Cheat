# Architecture Overview

This repository is a documentation-only reference for GTA V Story Mode cheat codes. The README is the entry point, with platform-specific cheat lists and shared usage notes organized as separate Markdown files.

```mermaid
flowchart TD
    Visitor[Reader] --> README[README.md\nProject overview and navigation]
    README --> PC[cheats/pc.md\nPC cheat reference]
    README --> PS[cheats/playstation.md\nPlayStation cheat reference]
    README --> Xbox[cheats/xbox.md\nXbox cheat reference]
    README --> Notes[docs/notes.md\nUsage notes and limitations]

    Contributor[Contributor] -->|updates documentation| README
    Contributor -->|adds or corrects codes| PC
    Contributor -->|adds or corrects codes| PS
    Contributor -->|adds or corrects codes| Xbox
    Contributor -->|updates guidance| Notes

    PC -. Story Mode reference only .-> Scope[Documentation scope]
    PS -. Story Mode reference only .-> Scope
    Xbox -. Story Mode reference only .-> Scope
    Scope --> Excludes[No game executables, online exploits,
or unauthorized software]
```

## Data flow

1. Readers start at `README.md` and choose the reference for their platform.
2. Platform cheat files provide the relevant code or controller combinations.
3. `docs/notes.md` documents shared usage guidance and limitations.
4. Contributors maintain these files through focused documentation changes and pull requests.

The repository contains reference documentation only; it does not interact with or modify the game.
