# Splits

Some notes on working with split windows while working on a project in vim.

So far, I prefer a vertical split. 

From within vim you could always do `:vsp FILENAME/DIRECTORY`.

In netrw, highlight the name of the file or directory and hit `v`.

To navigate within buffers try `:vert sb BUFFER NUMBER/NAME`.

Note on window width:
  I like to keep my line length at 80 (though i'm considering 100).  What I typically do is start my terminal window at 160 width, then when I vertical split I do `Ctrl + w =` to set both windows to equal length(80 each).

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
