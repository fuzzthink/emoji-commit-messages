# Emoji commit messages

Forked from [emoji-commit-messages](https://github.com/cooperka/emoji-commit-messages), see `Fork notes` in list for changes.
A fun paradigm to encourage cleaner commits.
Fork and modify to suit your needs. Don't forget to "star" and share the love.

## The list

| Text | GFM shortcode* | Windows 10 picker name | When to use it | Fork notes |
|:--:|:--------- |:-------------- |:-------------- |:-------------- |
| `🎉` | `:tada:` | `party popper` | initial commit, big feature complete | modified |
| `✨` | `:sparkles:` | `sparkles` | when adding a new user-facing feature ||
| `💎` | `:gem:` | `gem stone` | when adding a non user-facing feature | modified |
| `🎨` | `:art:` | `artist palette` | when improving UI ||
| `💪` | `:muscle:` | `muscle` | when refactoring | was `:package:`|
| `📦` | `:package:` | `package` | when changing an external package or new release| New usage |
| `🐎` | `:racehorse:` | `horse` | when improving performance ||
| `🔒` | `:lock:` | `locked` | when improving security ||
| `🔧` | `:wrench:` | `wrench` | when updating configs ||
| `♿` | `:wheelchair:` | `wheelchair symbol` |  when improving accessibility ||
| `🚀` | `:rocket:` | `rocket` | when improving dev tools ||
| `📝` | `:pencil:` | `pencil` | when editing docs (README, comments) ||
| `🐛` | `:bug:` | `bug` | when fixing a bug ||
| `🐞` | `:beetle:` | `beetle` | when fixing a bug | A popular alt for `:bug:`, longer to type, but looks more like a bug |
| `💥` | `:boom:` | `collision` | when fixing a crash ||
| `🚱` | `:non-potable_water:` | `non-potable water` | when fixing a memory leak ||
| `🧹` | `:broom:` | `broom` | when trimming or removing code or files | New! |
| `🔥` | `:fire:` | `fire` | when doing a hot fix that needs further attention | New usage |
| `✅` | `:white_check_mark:` | `check mark button` | when adding new tests ||
| `💚` | `:green_heart:` | `green heart` | when fixing the CI build ||
| `👕` | `:shirt:` | `t-shirt` | when fixing linter warnings ||
| `📡` | `:satellite:` | `satellite antenna` | when adding instrumentation or metrics ||
| `🔊` | `:loud_sound:` | `speaker high volume` | when adding logging ||
| `🔇` | `:mute:` | `muted speaker` | when removing logging ||
| `⬆` | `:arrow_up:` | `up arrow` | when upgrading dependencies ||
| `⬇` | `:arrow_down:` | `down arrow` | when downgrading dependencies ||
| `🎌` | `:crossed_flags:` | `crossed flags` | when adding an A/B test or feature flag** ||
| `⚡` | `:zap:` | `high voltage` | when making a backwards-incompatible change** ||
| `🚧` | `:construction:` | `construction` | when the change is a work in progress (do not merge)** ||

\* GFM shortcodes are recognized by any software that uses **G**itHub **F**lavored **M**arkdown. You can type them directly in your commit message!

\** These emoji are often combined with another, primary emoji.

## Motivation

Images (including emoji) help clarify what a given commit accomplishes,
make your commit history easier to scan though, and encourage you
to limit each of your changes to a single type of action.
This makes it easier to reason about the history of your code.

For example, instead of having one massive commit that adds a feature,
refactors an old related feature, fixes a typo, and fixes a bug,
you could split that change into four commits that each accomplish
one specific thing. Not only does this make things cleaner and clearer,
but it also helps when using tools like `git bisect` to track down bugs,
as well as when reverting individual changes.

## How to decide which emoji to use

In most cases, your change will fit into a pretty obvious emoji category. If it doesn't, you should think hard about whether or not you're making a clean change.

Often you can break up changes into two or more commits that each accomplish their own specific type of action. If that means you only change one tiny line or fix a simple typo in a commit, so be it! It should be a no-brainer that any given commit does exactly what it says it does — and **only** what is says it does. No side-effects.

In general, you should use exactly one emoji per commit message. In rare cases, you should use a second emoji (e.g. when using something like :zap: to signify that whatever you just did — :bug:, :fire:, etc. — was a breaking change).

Emoji will also depend on your client/user. A back-end API might use :sparkles: when adding new API endpoints, and the front-end app might use :sparkles: when using those endpoints to display new content.

## How to type emoji on your computer

I find it faster to type the raw emoji shortcode with colons (GitHub and GitLab both recognize this), but sometimes it's easier to search through the actual icons, especially as you're starting out.

- On **Mac OS X**, you can open the built-in emoji picker with the hotkey <kbd>Ctrl</kbd> + <kbd>Cmd</kbd> + <kbd>Space</kbd>.

- On **Ubuntu 14+**, you can use the Emojione Picker app:

    ```console
    sudo add-apt-repository ppa:ys/emojione-picker && sudo apt update
    sudo apt install emojione-picker
    ```

- On **Windows 10** update 1709, pressing <kbd>Win</kbd>+<kbd>.</kbd> while having keyboard focus in a text field in any program will bring up the built-in emoji picker, similarly to Mac OS. The table above includes names which work specifically in this emoji picker, but the GFM shortcodes work too. Some of the Windows-specific ones can be easier to remember, though.

  On lower versions of Windows, starting with **Windows 8**, you can use the on-screen keyboard in the system tray. Alternatively, you can use [BabelMap] which is a Unicode character picker for even lower versions of Windows. It also might be more convenient than the Windows 8 on-screen keyboard.

If all else fails, you can search for an emoji at <http://emojipedia.org/> and simply copy/paste.

## Real examples

The following is a brief list of open-source projects currently using these emoji:

- https://github.com/cooperka/emoji-commit-messages (of course)

- https://github.com/cooperka/react-native-snackbar

- https://github.com/cooperka/react-native-immutable-list-view

- https://github.com/cooperka/eslint-config-cooperka

- https://github.com/cooperka/bash-git-utils

- https://github.com/cribspot/emoji-utils

## Credits

Developed along with my co-workers at [Cribspot](https://www.cribspot.com/). Inspired in part by style guides from [slashsBin](https://github.com/slashsBin/styleguide-git-commit-message#suggested-emojis) and [atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md#git-commit-messages).

[BabelMap]: https://www.babelstone.co.uk/Software/BabelMap.html
