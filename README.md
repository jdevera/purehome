# Purehome: Watching out for a clean home

Inspired by [Gina Trapani's 6 folders
strategy](http://lifehacker.com/156196/geek-to-live--organizing-my-documents),
I have, for years now, strived to keep my home directory to 6 folders under
which everything is organised. I have gone one step further and define, for
myself, what goes in the next level inside those six, but that's another story.
Here we care only about the topmost home directory level.

Just like on Windows it was always just a little too convenient to save
everything to the desktop when I didn't know where to save something, the root
of the home directory seems to be equivalent place in Linux, a place chosen
even by many programs, to dump all sorts of random rubbish.

I say **no** to this, and to help keep my home tidy, I use `purehome`.

But `purehome` does not clean my home for me, not it does not. Purehome work by
making me ashamed of having a dirty home, by giving a constant reminder that
I've let myself slip. Purehome gets called in my shell init script, so when I
open a new shell, this is the greeting I get:

     ____________________________________________________________
    /                                                            \
    |  _  _                 _     __      _____  ___  _  _  ___  |
    | | || |___ _ __  ___  (_)___ \ \    / / _ \/ _ \| \| |/ __| |
    | | __ / _ \ '  \/ -_) | (_-<  \ \/\/ /|   / (_) | .` | (_ | |
    | |_||_\___/_|_|_\___| |_/__/   \_/\_/ |_|_\\___/|_|\_|\___| |
    |                                                            |
    | Superfluous contents:                                      |
    |  * this-file-should-not-be-here                            |
    \  * quick-thing-i-saved-in-my-homedir                       /
     ------------------------------------------------------------
            \   ^__^
             \  (oo)\_______
                (__)\       )\/\
                    ||----w |
                    ||     ||

Or, in good days, this:

    6 days with a clean home directory

## Okay, I want it!

Of course you do! Just clone the repository or download the `purehome` script
alone, then call it from your shell init script to have the constant reminder.

Oh, yes, you will only see the cow if you have `cowsay` installed, but then
again, why wouldn't you!

By default, these are the expected directories, no more, no less:

   * backup
   * comms
   * devel
   * doc
   * media
   * other

Of course your directories don't have to be those, just write your expected
list, one name per line in a file called `~/.config/purehome/expected` or, to
be sure, run

    purehome --debug

And that will tell you where `purehome` expects its config to be.


## License

MIT
