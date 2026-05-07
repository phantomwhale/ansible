# Mac dev environment - intent record for `brew bundle`.
# Only top-level (intentionally installed) packages belong here.
# Transitive dependencies are pulled in automatically by Homebrew.

# === Taps ===
tap "1password/tap"
tap "anomalyco/tap"                 # opencode
tap "asmvik/formulae"               # yabai (newer fork than koekeishiya)
tap "bufbuild/buf"                  # protocol buffers
tap "buildkite/buildkite"
tap "buildkite/developer-versions"  # pinned pg_partman build
tap "chase/tap"                     # awrit
tap "hashicorp/tap"                 # terraform
tap "homebrew/bundle"
tap "homebrew/services"
tap "koekeishiya/formulae"          # skhd
tap "lox/tap"                       # slack-cli
tap "puma/puma"                     # puma-dev
tap "schpet/tap"                    # linear cli
tap "th-ch/youtube-music"
tap "tinted-theming/tinted"         # tinty
tap "yt-dlp/taps"

# === Shells & terminals (CLI) ===
brew "antidote"            # zsh plugin manager
brew "bash"
brew "carapace"            # multi-shell completion engine

# === Editor ===
brew "neovim"

# === Core CLI utilities ===
brew "ast-grep"
brew "bat"                 # cat with syntax highlighting
brew "broot"               # interactive tree
brew "btop"                # resource monitor
brew "ctop"                # docker top
brew "curlie"              # curl wrapper
brew "eza"                 # ls replacement
brew "fd"                  # find replacement
brew "fx"                  # JSON viewer
brew "fzf"                 # fuzzy finder
brew "gping"               # ping with graph
brew "htmlq"               # jq for HTML
brew "httpie"              # curl alternative
brew "jq"                  # JSON processor
brew "lftp"                # FTP/SFTP client
brew "mdless"              # markdown viewer
brew "parallel"            # GNU parallel
brew "pstree"
brew "ripgrep"
brew "rsync"
brew "sd"                  # sed replacement
brew "stow"                # dotfiles manager
brew "todo-txt"
brew "wget"
brew "yazi"                # file manager TUI
brew "yq"                  # YAML processor
brew "zoxide"              # cd replacement

# === Git / VCS ===
brew "gh"
brew "git"
brew "git-delta"
brew "git-extras"
brew "git-filter-repo"
brew "git-lfs"
brew "glow"                # markdown TUI
brew "jj"                  # jujutsu VCS
brew "lazygit"
brew "lefthook"            # git hooks
brew "worktrunk"           # Git worktree manager for parallel AI agents

# === Languages ===
brew "fnm"                 # Node version manager
brew "go"
brew "node"
brew "openjdk@17"
brew "rust"
brew "yarn"                # Node package manager

# === Ruby ===
brew "chruby"
brew "frum"
brew "mise"
brew "ruby-install", args: ["HEAD"]

# === Build / dev tooling ===
brew "automake"
brew "bison"
brew "ctags", link: false
brew "luacheck"
brew "llvm"
brew "shellcheck"
brew "shfmt"
brew "tflint"
brew "trufflehog"          # secret scanner

# === Cloud / infra ===
brew "ansible"
brew "aws-vault"
brew "awscli"
brew "docker-compose"

# === Process management ===
brew "overmind"            # Procfile runner

# === Databases ===
brew "duckdb"
brew "kcat"                # Kafka CLI
brew "libpq@16"
brew "mysql", restart_service: :changed
brew "pg_partman"
brew "postgresql@16", restart_service: :changed
brew "redis", restart_service: :changed

# === Web servers ===
brew "nginx"

# === Media / graphics ===
brew "exiftool"
brew "ffmpeg"
brew "fftw"
brew "ghostscript"
brew "gifski"
brew "graphviz"
brew "imagemagick"
brew "img2pdf"
brew "marp-cli"            # markdown presentations
brew "poppler"             # PDF tools
brew "watchman"            # file watcher
brew "yt-dlp"

# === Performance / load testing ===
brew "hey"
brew "iperf"
brew "k6"

# === LLM / AI ===
brew "codex"
brew "kingfisher"
brew "llm"

# === macOS ===
brew "mas"                 # Mac App Store CLI
brew "asmvik/formulae/yabai"
brew "koekeishiya/formulae/skhd"

# === Misc ===
brew "keyring"             # Python keyring backend
brew "libpqxx"             # postgres C++ lib

# === Tap-specific brews ===
brew "anomalyco/tap/opencode"
brew "bufbuild/buf/buf"
brew "buildkite/buildkite/bktec"
brew "buildkite/buildkite/buildkite-agent"
brew "buildkite/buildkite/test-splitter"
brew "buildkite/developer-versions/pg_partman@5.2.4"
brew "chase/tap/awrit"
brew "hashicorp/tap/terraform"
brew "lox/tap/slack-cli"
brew "puma/puma/puma-dev"
brew "schpet/tap/linear"
brew "tinted-theming/tinted/tinty"

# === Casks: 1Password ===
cask "1password"
cask "1password-cli"

# === Casks: browsers ===
cask "firefox"
cask "google-chrome"

# === Casks: terminals ===
cask "ghostty"
cask "kitty"

# === Casks: dev tools ===
cask "dash"
cask "mitmproxy"
cask "orbstack"

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
cask "logitune"            # Logitech webcam tuning

# === Casks: communication ===
cask "signal"
cask "slack"

# === Casks: media ===
cask "calibre"
cask "gimp"
cask "vlc"
cask "yacreader"
cask "youtube-music"

# === Casks: gaming ===
cask "epic-games"
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
mas "ImageDiff", id: 1_602_522_152
mas "iMovie", id: 408_981_434
mas "Keynote", id: 409_183_694
mas "Meeter", id: 1_510_445_899
mas "Monodraw", id: 920_404_675
mas "Numbers", id: 409_203_825
mas "Pages", id: 409_201_541
mas "Pixea", id: 1_507_782_672
mas "The Unarchiver", id: 425_424_353

# === Go installs ===
go "github.com/minio/minio"
