# Splits

Some notes on working with split windows while working on a project in vim.

So far, I prefer a vertical split. 

From within vim you could always do `:vsp FILENAME/DIRECTORY`.

In netrw, highlight the name of the file or directory and hit `v`.

To navigate within buffers try `:vert sb BUFFER NUMBER/NAME`.

## Some .vimrc changes to consider

By default, the split opens to the left of the current window, which I dont find as intuitive. Adding the following to .vimrc will make it open to the right:
```
set splitright
```
Normally to navigate between split windows you would have to do Ctrl + W then h, j, k, or l depending on which direction you're going.  With this remap, it would be a matter of just doing `Ctrl + l` to go to the right panel or `Ctrl + h` to go back to the left panel. 
```
nnoremap <C-J> <C-W><C-J>
nnoremap <C-K> <C-W><C-K>
nnoremap <C-L> <C-W><C-L>
nnoremap <C-H> <C-W><C-H>
```

TODO: 

more split tips/shortcuts?
