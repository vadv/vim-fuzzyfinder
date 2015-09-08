
```
let g:FuzzyFinderOptions = { 'Base':{}, 'Buffer':{}, 'File':{}, 'Dir':{}, 'MruFile':{}, 'MruCmd':{}, 'Bookmark':{}, 'Tag':{}, 'TaggedFile':{}}
let g:FuzzyFinderOptions.Base.ignore_case = 1
let g:FuzzyFinderOptions.Base.abbrev_map  = {
      \   '\C^VR' : [
      \     '$VIMRUNTIME/**',
      \     '~/.vim/**',
      \     '$VIM/.vim/**',
      \     '$VIM/vimfiles/**',
      \   ],
      \ }
let g:FuzzyFinderOptions.MruFile.max_item = 200
let g:FuzzyFinderOptions.MruCmd.max_item = 200
nnoremap <silent> <C-n>      :FuzzyFinderBuffer<CR>
nnoremap <silent> <C-m>      :FuzzyFinderFile <C-r>=expand('%:~:.')[:-1-len(expand('%:~:.:t'))]<CR><CR>
nnoremap <silent> <C-j>      :FuzzyFinderMruFile<CR>
nnoremap <silent> <C-k>      :FuzzyFinderMruCmd<CR>
nnoremap <silent> <C-p>      :FuzzyFinderDir <C-r>=expand('%:p:~')[:-1-len(expand('%:p:~:t'))]<CR><CR>
nnoremap <silent> <C-f><C-d> :FuzzyFinderDir<CR>
nnoremap <silent> <C-b>      :FuzzyFinderBookmark<CR>
nnoremap <silent> <C-f><C-t> :FuzzyFinderTag!<CR>
nnoremap <silent> <C-f><C-g> :FuzzyFinderTaggedFile<CR>
noremap  <silent> g]         :FuzzyFinderTag! <C-r>=expand('<cword>')<CR><CR>
nnoremap <silent> <C-f>b     :FuzzyFinderAddBookmark<CR>
nnoremap <silent> <C-f><C-e> :FuzzyFinderEditInfo<CR>
```