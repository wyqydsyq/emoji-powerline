## emoji-powerline

Based on Agnoster, extended with emojis representing home and root directories. Paths in the pwd prompt and git branch are split by "/" and joined as powerline segments for a clean aesthetic.

Colours and emojis used are easily configurable at the top of `./fish_prompt.fish`

#### Characteristics

* If you're under your home directory, "~" is replaced with "🏠"
* If you're outside your home directory, the root-level "/" is replaced with "💻"
* pwd_prompt is split by "/", each section is turned into a Powerline segment
* Git branch is split by "/", each section is turned into a Powerline segment
* If the previous command failed (✘)
* User @ Hostname (if user is not DEFAULT_USER, which can then be set in your profile)
* Git/HG/SVN status
* Branch () or detached head (➦)
* Current branch / SHA1 in detached head state
* Dirty working directory (✱, color change)
* Clean working directory ✔
* Elevated (root) privileges (⚡)
* Current virtualenv (Python)
You will probably want to disable the default virtualenv prompt. Add to your [`init.fish`](https://github.com/oh-my-fish/oh-my-fish#dotfiles):
`set --export VIRTUAL_ENV_DISABLE_PROMPT 1`
* Indicate vi mode.

Ported from https://gist.github.com/agnoster/3712874.
