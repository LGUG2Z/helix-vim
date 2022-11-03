# Helix-Vim

A Vim-like configuration for Helix

## About

Let me guess why you're here. You're a
[(Neo)](https://github.com/neovim/neovim)[Vim](https://github.com/vim/vim)
user. Today, for the millionth time, you updated your plugins and were met with
a sea of criminally useless error messages. You have things to do. You don't
have time to search the GitHub issues of arcane plugins maintained by people
whose approach to breaking changes is... well, a little too cavalier for your
tastes.

You recall a friend or a colleague sent you a link to the
[Helix](https://github.com/helix-editor/helix) editor a while ago. It looked
pretty cool, right?

"But what about the plugins!" cried the acolytes of NeoVim. Hmm... Plugins.
Those plugins that break your barely recognizable `vimrc` with depressing
regularity. Or maybe you really drank the Kool Aid and translated your config
to Lua. It doesn't matter either way. Breaking changes in NeoVim plugins don't
care about your `.vimrc` _or_ your `init.lua`

Yes... Those plugins that you shouldn't even need to install to have a
functional editor.

Plugins be damned!

Your sweaty hands fumble on your obnoxiously loud mechanical keyboard with the
`alt + hjkl` keys to focus your open terminal emulator with your tiling window
manager. [`kitty`](https://github.com/kovidgoyal/kitty) or
[`alacritty`](https://github.com/alacritty/alacritty), probably. You are thrown
back briefly to a memory of the countless hours spent trying to get your
terminal and Neo(Vim) colourschemes to match.

You install the latest binary release of Helix available on your package
manager of choice and `cd` into the directory you were about to start working
in before your Neo(Vim) configuration was drowned in a flood of red.

`hx`

You tentatively press the space bar and try out the file picker. Fuzzy search.
Syntax highlighting. Nice. Naturally, the directory you are in hosts a Rust
project. You select one of the numerous `lib.rs` files which serve as the entry
points to the Cargo workspace crates that you split your monolith out into in
hope of improving your incremental compilation times on your aging Macbook Pro.
Your company won't give you one of the new M1 models because this one isn't 5
years old yet. Alas.

You hear [`rust-analyzer`](https://github.com/rust-lang/rust-analyzer) begin to
impose its will on your aging Intel CPU, crippled further by Jonny Ive's
obsession with thinness above everything. I bet he's a raging fatphobe.

Wait a minute... Your eyes dart around the screen. There are no errors. The
syntax highlighting looks right. You try to navigate through the file using
`{}`, but it's not working. Hmm, that can be figured out later. You use the
mouse to bring the cursor to an invocation of a declarative `macro_rules!`
macro. You press `g` and are met with a host of LSP-powered options. You didn't
even install an LSP plugin! You press `k` and a pop-up appears with the
documentation for the macro.

This is how life should always be. You resolve to make the switch to Helix.

... And not long after, you give up. Your Vim muscle-memory is too strong. The
Verb-Modifier-Object structure of Vim commands has become the language that
your brain uses to send instructions to your fingers. Defeated, the references
to `hx` in your `.zsh_history` become fewer and far between, until they
disappear completely, replaced once again by `vim`, `nvim` or `nvim` aliased to
`vim`.

You dismiss the red error messages screaming at you every time you open the
editor. Maybe you keep an instance of it running after you have dismissed all
the errors so that you don't have to go through the humiliation of dismissing
errors that you don't have the time, energy or motivation to fix every time you
want to edit a file.

Maybe one day, you think, it will be possible to use Helix in "Vim mode", after
all, there is even a pretty decent Vim plugin for VSCode these days, right?

My friend. I have felt your frustration, your anger, your sorrow, your
disappointment, and your defeat.

I might not be able to give you a perfect solution right now, but I can give
you more than enough to get the ball rolling!

## Usage

Check out the `config.toml` file in this repository. It only
contains key mappings. These were the most important key mappings to allow me
to use as much of my Vim muscle-memory as possible when editing text in Helix.

If you are used to doing `c` commands a lot, you're going to have to adapt
to selecting the area you want with `v` and then deleting it.

With this being said, a lot of the most basic stuff (including `C`, `0`, `$`,
`^`, `G`, `{}` and `%`!) that you rely on every day to edit and navigate a text
file without thinking about it, is implemented.

Feel free to fork this, personalize it, make suggestions, improvements, fill in
gaps that I don't know how to fill, etc.
