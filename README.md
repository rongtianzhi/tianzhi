天智王






echo 'map <F8> :wq! <CR> 

map <F9> :q! <CR>
 
map <F2>  :set number <CR>

map <F3>  :set ninumber <CR>

autocmd BufNewFile *.sh  exec ":call SetTitle()"

func SetTitle()

if &filetype == "sh"

  call setline(1, "\#!/bin/bash")

  call append(line("."), "")

endif

normal G                                                                                             

endfunc    '  >  ~/.vimrc

export PS1=$"\u@\h\W]\$\[\033[46m\] \[\033[0m\]"

echo 'export PS1=$"\u@\h\W]\$\[\033[46m\] \[\033[0m\]" ' >> ~/.bashrc






