# neovim

> config path "~/.config/nvim/init.vim" 
  
> plug path "~/.local/share/nvim/"



![nvim](https://raw.githubusercontent.com/Jandzy/neovim/master/mynvim.png)


~~~
  ~/.c/n/init.vim                                                                                        buffers 
  1 set number " 显示行号
  2 set tabstop=4 " 设置tab =  4空格
  3 set cursorline " 高亮当前行
  4 hi CursorLine cterm=NONE ctermbg=black ctermfg=green guibg=NONE guifg=NONE "设置当前行高亮颜色
  5  
  6 call plug#begin('~/.local/share/nvim/plugged')
  7 " 自动补全插件
  8 Plug 'Shougo/deoplete.nvim', {'do': 'UpdateRemotePlugins'}
  9 let g:deoplete#enable_at_startup = 1
 10 "主题插件
 11 Plug 'morhetz/gruvbox'
 12 let g:gruvbox_constrast_dark = 'hard'
 13 "好看的状态栏
 14 Plug 'vim-airline/vim-airline'
 15 Plug 'vim-airline/vim-airline-themes'
 16 let g:airline#extensions#tabline#enabled = 1
 17 "nerdtree
 18 Plug 'scrooloose/nerdtree'
 19 "高亮显示markdown语法（会引起折叠）
 20 "Plug 'godlygeek/tabular'
 21 "Plug 'plasticboy/vim-markdown'
 22 "即时预览markdown
 23 "Plug 'suan/vim-instant-markdown'
 24 "markdown priview
 25 "function! BuildComposer(info)
 26 "    if a:info.status != 'unchanged' || a:info.force
 27 "           cargo build --release
 28 "    endif
 29 "endfunction
 30 "Plug 'euclio/vim-markdown-composer', {'do': function('BuildComposer')}
 31 "let g:markdown_composer_open_brower = 1
 32 "国产markdown插件，可以同步滚动
 33 Plug 'iamcco/mathjax-support-for-mkdp'
 34 Plug 'iamcco/markdown-preview.vim'
 35 call plug#end()                     
~~~

