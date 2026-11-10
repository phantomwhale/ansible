# Mac dev environment - intent record for `brew bundle`.
# Only top-level (intentionally installed) packages belong here.
# Transitive dependencies are pulled in automatically by Homebrew.
#
# Programming language runtimes and portable dev CLIs are NOT here -
# they are managed by mise (see default.config.yml / tasks/mise.yml).
# Homebrew owns: compiled libraries, services, GUI apps, macOS integration,
# and mise itself (the bootstrap).
#
# Buildkite-codebase-only dependencies (puma-dev, redis, watchman, kcat,
# libpqxx, bktec, ...) live in ~/code/BK/buildkite/Brewfile, not here.

# === Taps ===
tap "anomalyco/tap"         # opencode
tap "asmvik/formulae"       # yabai + skhd (maintained fork of koekeishiya)
tap "buildkite/buildkite"
tap "datadog-labs/pack"     # pup
tap "felixkratz/formulae"   # sketchybar
tap "getagentseal/codeburn"
tap "lox/tap"               # slack-cli (Slack reader CLI, not Slack's official `slack`)
tap "schpet/tap"            # linear cli
tap "tinted-theming/tinted" # tinty

# === Version / tool manager ===
# mise must come from Homebrew: it is the bootstrap that installs everything
# else, and it is not on PATH in the non-interactive shells Ansible uses.
brew "mise"

# === Shells ===
brew "antidote"            # zsh plugin manager - sourced in .zshrc
brew "bash"
brew "carapace"            # multi-shell completion engine - sourced in .zshrc

# === Editor ===
brew "neovim"
brew "tree-sitter-cli"     # nvim-treesitter `main` branch compiles parsers with it
brew "luacheck"
brew "shfmt"               # none-ls formatter

# === Core CLI utilities ===
brew "ast-grep"
brew "bat"                 # cat with syntax highlighting (aliased to `cat`)
brew "broot"               # interactive tree - launcher sourced in .zshrc
brew "btop"                # resource monitor
brew "eza"                 # ls replacement (aliased to `ls`)
brew "fzf"                 # fuzzy finder - .zshrc keybindings + git aliases
brew "jq"                  # JSON processor
brew "just"                # command runner
brew "ripgrep"
brew "sl"
brew "sponge"              # soak up stdin before writing to the same file
brew "stow"                # dotfiles manager - used by install-osx.sh
brew "todo-txt"
brew "tree"
brew "tuios"              # terminal multiplexer TUI
brew "yazi"                # file manager TUI
brew "zoxide"             # `z` / `zi` - initialised in .zshrc, used by telescope-zoxide

# === Markdown viewers ===
brew "glow"                # markdown TUI - used by ai_functions.zsh
brew "mdcat"               # markdown pager

# === Network / HTTP ===
brew "httpie"              # `http` / `https`
brew "lftp"                # FTP/SFTP client
brew "rsync"              # current rsync over the macOS default
brew "wget"

# === Git / VCS ===
brew "gh"
brew "git"
brew "git-lfs"
brew "lazygit"             # aliased to `lg`
brew "worktrunk"           # `wt` - git worktree manager for parallel AI agents

# === Python tooling ===
brew "uv" # runs `llm` + `pocketsmith-cli` (see tasks/llm.yml)

# === Cloud / infra ===
brew "ansible"
brew "awscli"
brew "aws-vault"           # maintained ByteNess fork; replaces the discontinued aws-vault-binary cask
brew "docker-compose"
brew "datadog-labs/pack/pup" # Datadog CLI - config dir set in .zshenv

# === Databases ===
# Client tools only (psql, pg_dump). Servers run in Docker/OrbStack.
# keg-only, but force-linked so psql/pg_dump land in /opt/homebrew/bin.
# Without `link: true`, `brew bundle install` unlinks it and removes them.
brew "libpq", link: true

# === Media / graphics ===
brew "exiftool"
brew "ffmpeg"              # runtime delegate for yt-dlp stream merging
brew "ghostscript"         # runtime delegate for imagemagick PDF/EPS
brew "imagemagick"
brew "img2pdf"
brew "marp-cli"            # markdown presentations
brew "poppler"             # PDF tools
brew "yt-dlp"

# === LLM / AI ===
brew "anomalyco/tap/opencode"
brew "getagentseal/codeburn/codeburn"
brew "nono"                # agent sandbox - profiles in dotfiles
# llm: managed via `uv tool` in tasks/llm.yml so `brew upgrade` can't wipe its plugins

# === macOS ===
brew "mas"                 # Mac App Store CLI - required by the `mas` entries below
brew "xcodes"              # Xcode version manager
brew "asmvik/formulae/yabai"
brew "asmvik/formulae/skhd"
brew "felixkratz/formulae/sketchybar"

# === Buildkite ===
brew "buildkite/buildkite/bk@3"
brew "buildkite/buildkite/buildkite-agent@3"

# === Other tap-specific brews ===
brew "schpet/tap/linear" # used by the using-linear / starting-linear-issue skills
brew "tinted-theming/tinted/tinty"

# === Casks: 1Password ===
cask "1password"
cask "1password-cli"

# === Casks: browsers ===
cask "zen"

# === Casks: terminals ===
cask "kitty"

# === Casks: dev tools ===
cask "dash"
cask "mitmproxy"
cask "ngrok"
cask "orbstack"
cask "session-manager-plugin"
cask "lox/tap/slack-cli"

# === Casks: productivity ===
cask "cleanshot"
cask "daisydisk"
cask "google-drive"
cask "hyperkey"
cask "linear"
cask "notunes"
cask "obsidian"
cask "raycast"

# === Casks: hardware/peripherals ===
cask "keymapp"             # ZSA keyboard configurator
cask "logitune"            # Logitech webcam tuning

# === Casks: communication ===
cask "signal"
cask "slack"

# === Casks: media ===
cask "calibre"
cask "gimp"
cask "transmission"
cask "vlc"
cask "yacreader"

# === Casks: screencasting ===
cask "keycastr"

# === Casks: gaming ===
cask "epic-games"
cask "highball"            # run Windows games
cask "steam"

# === Casks: fonts ===
cask "font-fira-code"
cask "font-fira-code-nerd-font"
cask "font-fira-mono"
cask "font-fira-mono-for-powerline"
cask "font-fira-sans"

# === Mac App Store ===
mas "Amphetamine", id: 937_984_704
mas "GarageBand", id: 682_658_836
mas "Hidden Bar", id: 1_452_453_066
mas "ImageDiff", id: 1_602_522_152
mas "iMovie", id: 408_981_434
mas "Keynote", id: 409_183_694
mas "Meeter", id: 1_510_445_899
mas "Monodraw", id: 920_404_675
mas "Numbers", id: 409_203_825
mas "Pages", id: 409_201_541
mas "Pixea", id: 1_507_782_672
mas "The Unarchiver", id: 425_424_353
