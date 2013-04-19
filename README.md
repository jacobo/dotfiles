SETUP
========

$ pwd
/Users/jburkhart/p/allthedotfiles
$ git clone git@github.com:jacobo/dotfiles.git
$ cd ~
$ ln -s ~/p/allthedotfiles/dotfiles/vim/vimrc .vimrc
$ ln -s ~/p/allthedotfiles/dotfiles/rc/tmux.conf .tmux.conf
$ ln -s ~/p/allthedotfiles/dotfiles/vim .vim
$ ln -s ~/p/allthedotfiles/dotfiles/gvimrc .gvimrc

#update vim bundles
$ ruby ~/.vim/update_bundles

#TODO: silver searcher?
$ brew install the_silver_searcher
#in vimrc:
" map Silver Searcher
map <leader>a :Ag!<space>

#start a new session
$ tmux new -s resque


TODO: how do I make the cursor look different in insert mode

TODO: can I have auto-save in vim?

dotfiles
========

I don't actually use any of these (yet)

Messing with tmux and vim...

http://www.worldtimzone.com/res/vi.html

NOTES:

ack bundle directions:
  https://github.com/mileszs/ack.vim

http://chrishunt.co/talks/vim-tmux/

tmux new-window (prefix + c)
create a new window

vim auto-complete: control  n
search: ,a
open file: control p

http://robots.thoughtbot.com/post/2641409235/a-tmux-crash-course
  tmux attach -t session_name
  tmux new -s session_name
  tmux list-sessions
  
Things to figure out in priority order:
  make ",t" run tests
  run tests in split pane instead?
  how do you auto-complete in vim?
