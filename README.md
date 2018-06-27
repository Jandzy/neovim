# neovim

> config path "~/.config/nvim/init.vim" 
  
> plug path "~/.local/share/nvim/"

~~~
 ~/.c/n/init.vim                                   buffers 
  1 set number " 显示行号
  2 set tabstop=4 " 设置tab =  4空格
  3 set cursorline " 高亮当前行
  4 call plug#begin('~/.local/share/nvim/plugged')
  5  
  6 " 自动补全插件
  7 Plug 'Shougo/deoplete.nvim', {'do': 'UpdateRemotePlugin
    s'}
  8 let g:deoplete#enable_at_startup = 1
  9  
 10 "主题插件
 11 Plug 'morhetz/gruvbox'
 12 let g:gruvbox_constrast_dark = 'hard'
 13  
 14 "好看的状态栏
 15 Plug 'vim-airline/vim-airline'
 16 Plug 'vim-airline/vim-airline-themes'
 17 let g:airline#extensions#tabline#enabled = 1
 18  
 19 "markdown priview
 20 function! BuildComposer(info)
 21     if a:info.status != 'unchanged' || a:info.force
 22             cargo build --release
 23     endif
 24 endfunction
 25 Plug 'euclio/vim-markdown-composer', {'do': function('B
    uildComposer')}
 26 let g:markdown_composer_open_brower = 1
 27  
 28 "nerdtree 树形目录
 29 Plug 'scrooloose/nerdtree'
 30 call plug#end()
~~~

