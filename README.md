# neovim

> config path "~/.config/nvim/init.vim" 
  
> plug path "~/.local/share/nvim/"



![nvim](https://raw.githubusercontent.com/Jandzy/neovim/master/mynvim.png)


~~~
  .c/n/init.vim                                                                                                  buffers 
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
 11 "Plug 'morhetz/gruvbox'                                                                                             
 12 "let g:gruvbox_constrast_dark = 'soft'                                                                              
 13 "另外一个主题                                                                                                       
 14 Plug 'mhartington/oceanic-next'                                                                                     
 15 "好看的状态栏                                                                                                       
 16 Plug 'vim-airline/vim-airline'                                                                                      
 17 Plug 'vim-airline/vim-airline-themes'                                                                               
 18 let g:airline#extensions#tabline#enabled = 1                                                                        
 19 "nerdtree                                                                                                           
 20 Plug 'scrooloose/nerdtree'                                                                                          
 21 "高亮显示markdown语法（会引起折叠）                                                                                 
 22 "Plug 'godlygeek/tabular'                                                                                           
 23 "Plug 'plasticboy/vim-markdown'                                                                                     
 24 "即时预览markdown                                                                                                   
 25 "Plug 'suan/vim-instant-markdown'                                                                                   
 26 "markdown priview                                                                                                   
 27 "function! BuildComposer(info)                                                                                      
 28 "    if a:info.status != 'unchanged' || a:info.force                                                                
 29 "           cargo build --release                                                                                   
 30 "    endif                                                                                                          
 31 "endfunction                                                                                                        
 32 "Plug 'euclio/vim-markdown-composer', {'do': function('BuildComposer')}                                             
 33 "let g:markdown_composer_open_brower = 1                                                                            
 34 "国产markdown插件，可以同步滚动                                                                                     
 35 Plug 'iamcco/mathjax-support-for-mkdp'                                                                              
 36 Plug 'iamcco/markdown-preview.vim'                                                                                  
 37 call plug#end()                                                                                                     
 38                                                                                                                     
 39 " neovim >= 0.1.5                                                                                                   
 40 if (has("termguicolors"))                                                                                           
 41         set termguicolors                                                                                           
 42 endif                                                                                                               
 43                                                                                                                     
 44 "Theme                                                                                                              
 45 syntax enable                                                                                                       
 46 colorscheme OceanicNext  
~~~

