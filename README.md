zex:

example.

1) Interting command outputs with :r.

<img src="https://github.com/hchbaw/zex.zsh/raw/readme/0.png" />

<img src="https://github.com/hchbaw/zex.zsh/raw/readme/1.png" />

2) Applying multiple :s commands.

<img src="https://github.com/hchbaw/zex.zsh/raw/readme/2.png" />

<img src="https://github.com/hchbaw/zex.zsh/raw/readme/3.png" />

<pre>
zex: `ex'ish for zsh.

Author: Takeshi Banse &lt;takebi@laafc.net&gt;
Licence: Public Domain

Thank you very much, tyru!
I want to use ex in zsh. I can do it with iex eventually.

To use this,
1) install iex and add it to your $PATH.
http://github.com/tyru/iex
2) source this file.
% source zex.zsh
3) add default key bindings.
% zex-install-keys
*Optionally* you can use the zcompiled file with the autoloading for a
little faster loading on every shell startup, if you zcompile the
necessary functions.
*1) zcompile the defined functions and the install command.
(generates ~/.zsh/zfunc/{zex,zex-install}.zwc)
% O=~/path/to/zex.zsh; (zsh -c "source $O && zex-zcompile $O ~/.zsh/zfunc")
*2) source the zcompiled install command file insted of this file.
% source ~/.zsh/zfunc/zex-install; zex-install; zex-install-keys

Note:
zex-install-keys replaces some keymap entries. Please beware of.
-- &gt;8 --
'^[:' zex-edit-command-line (emacs)
':'   zex-edit-command-line (vicmd)
-- 8&lt; --

TODO: execute updated command directly.
TODO: a standalone function.
TODO: disable undo when editing the iex buffer or better.

History

v0.0.1
Initial version.
</pre>
