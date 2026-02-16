# Global CLAUDE.md
> Claude Code config lives in `~/.obsidian/remote_notes/claude/` and is synced via
> Obsidian Sync + Git (git@gitlab.com:hateaf/claude_settings.git).
>
> **New machine setup:**
> ```sh
> cd ~/.obsidian/remote_notes/
> git clone git@gitlab.com:hateaf/claude_settings.git claude
> mkdir -p ~/.claude
> ln -sf ~/.obsidian/remote_notes/claude/CLAUDE.md ~/.claude/CLAUDE.md
> ln -sf ~/.obsidian/remote_notes/claude/settings.json ~/.claude/settings.json
> ln -sf ~/.obsidian/remote_notes/claude/commands ~/.claude/commands
> ```
>
> **Synced files:**
> - `CLAUDE.md` — global instructions
> - `settings.json` — status line config
> - `commands/` — custom slash commands

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
