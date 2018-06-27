# Guide to get started on Emacs

The first thing to do, once you open Emacs go and look at the tutorial. It gives you the basics of movement and editing. Those commands, even when probably not as good as vim commands, give you a lot of editing power (they do have some advantage over vim commands, though). Recommendation to use `C-s` (search forward) and `C-r` (search backwards) as your way to move inside a file if you know what you are looking for.

Be sure to look at how to use the help. `C-h ?` to start with. `C-h b` to see the current keybindings (remember that keybindings are based on the active buffer and the modes available, so when you change to a different buffer those keybindings could/will change). Also `M-x describe-package` and `M-x describe-mode` are quite useful to start getting information about what is available to use. Furthermore, the apropos system (`M-x apropos` and subcommands) is quite useful in gathering information about the different available elements.

Do remember that either `C-g` or `Esc Esc Esc` will allow you to "cancel" a keychord. For this reason, never remap the `C-g` keybinding.

Once that is done you want to start adapting Emacs for yourself. Use the init.el that I provided (I have updated the gist with the `exec-path-from-shell` lines) deleting everything related to cider/clojure if you are not interested in clojure development. Later on you can go your own way defining your init files. Make sure that you understand how `use-package` works (https://github.com/jwiegley/use-package)

For more info about Emacs and different packages you can visit https://masteringemacs.org/ and https://www.emacswiki.org/ 

First package that I recommend to add is `whichkey` (https://github.com/justbur/emacs-which-key). Really useful if you only remember the beginning of a command. 

Then a collection of packages that I found very useful in terms of looking for commands/functions/files `ido` (https://masteringemacs.org/article/introduction-to-ido-mode), `flx` and `flx-ido` (https://github.com/lewang/flx), and `smex` (https://github.com/nonsequitur/smex/). Alternatively you could use `helm` (https://github.com/emacs-helm/helm), but I have no experience with it.

`Magit` (https://magit.vc/), the git porcelain for Emacs, is the best benefit you can get right now of Emacs even if you continue using another editor for your normal use.

Finally, a small utility you can use is `NeoTree` (https://github.com/jaypei/emacs-neotree) 

Interestingly, because of some issue with NeoTree display I ended eliminating the tool bar, menu bar and scroll bar from my Emacs.

One thing that I didn't mention on the workshop is that you can use emacs either from the terminal or from the UI. There are a few benefits with the UI, regarding things like color, some other graphical capabilites and to have the yank/kill rings linked to the clipboard of your OS.

You can find my init files at https://github.com/MiyamotoAkira/.emacs.d

And if you want to see a proper pro of Emacs in action check the Emacs posts of http://howardism.org/ 

Or if you want some funny and informative videos http://emacsrocks.com/ 

Last note, a lot of people have their `.emacs.d` configuration files on github, look for them.
