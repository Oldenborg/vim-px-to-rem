**Vim-px-to-rem**  -  Convert px to rem or rem to px
==================================
Makes font-size unit conversion for your CSS stylesheets easy!

Installation
------------------------
### Pathogen Install
1. Navigate to your **[VIM_ROOT]/bundle** directory in your local Vim setup
2. git clone https://github.com/Oldenborg/vim-px-to-rem.git

### Vundle Install'
Add the following to your `.vimrc` file in the vundle plugin section
```
Plugin 'Oldenborg/vim-px-to-rem'
```

Usage
-------------------------
To convert the pixels to rem, select a block of text in visual mode and the enter the following :

```
:Rem
```

Or enter the following to convert the rem to pixels:

```
:Px
```

To convert all pixels in the file to rem:

```
:RemAll
```

Or to convert all rem in the file to pixels:

```
:PxAll
```

Add a bang (eg. :Px!) to any of the above command to bypass the prompts before each conversion.

If you don't want to use the standard Base font of 16px, add the following to your ~/.vimrc

```
let g:px_to_rem_base = DIFFERENT_FONT_SIZE
```

Example:

```
let g:px_to_rem_base = 24
```

Thanks to
------------------------------------------------------
[Github user Chiedo](https://github.com/chiedo)
This repo was heavily copied from his [Chiedo/vim-px-to-em](https://github.com/chiedo/vim-px-to-em) repository.

License
------------------------------------------------------
Distributed under the same terms as Vim itself. See :help license.
