# Global CLAUDE.md
> This file lives in the Obsidian vault at `~/.obsidian/remote_notes/claude/CLAUDE.md`
> and is symlinked to `~/.claude/CLAUDE.md`. Obsidian Sync keeps it in sync across devices.
> On a new machine, run: `ln -sf ~/.obsidian/remote_notes/claude/CLAUDE.md ~/.claude/CLAUDE.md`

## Language & Style
- Primary language: C++
- Prefer modern C++17/20 features (structured bindings, std::optional, constexpr if, concepts, ranges)
- Use RAII and smart pointers (std::unique_ptr, std::shared_ptr) over raw pointers
- Prefer std::string_view for non-owning string parameters
- Use auto where the type is obvious from context

## Conventions
- Use snake_case for functions and variables, PascalCase for types/classes
- Prefer const-correctness throughout
- Mark single-argument constructors explicit
- Use [[nodiscard]] on functions where ignoring the return value is likely a bug

## Obsidian Notes
- Vault path: ~/.obsidian/remote_notes/ (/Users/darkthrone/.obsidian/remote_notes/)
- Obsidian is the user's primary note-taking tool, synced via Obsidian Sync
- Occasionally take notes for the user when relevant (e.g., summarizing decisions, documenting architecture, capturing TODOs)
- Notes are plain markdown files — write directly to the vault path
- Naming convention: YYYY-MM-DD_short-description.md
- Folder structure:
  - personal/ — user's personal notes
  - work/ — work-related notes
  - projects/<project-name>/ — project-specific notes (e.g., projects/hyperion/)
