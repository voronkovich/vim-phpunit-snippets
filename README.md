vim-phpunit-snippets
====================

Code snippets for PHPUnit. Require installed SnipMate plugin.

Installation
------------

After installation add into yout .vimrc
```vimml 
let g:snipMate = {}
let g:snipMate.scope_aliases = {}
let g:snipMate.scope_aliases['php'] = 'php,html,javascript'
 
au BufEnter *Test.php let g:snipMate.scope_aliases['php'] .= ',phpunit'
au BufLeave *Test.php let g:snipMate.scope_aliases['php'] = substitute(g:snipMate.scope_aliases['php'], ',phpunit', '', '')
```

License
-------

Copyright (c) Voronkovich Oleg.  Distributed under the same terms as Vim itself.
See `:help license`.
