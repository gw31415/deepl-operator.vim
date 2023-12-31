# deepl-operator.vim

Mapping that enables to translate with `<Plug>(deepl-replace)`!


https://github.com/gw31415/deepl-operator.vim/assets/24710985/be8c9367-ad87-4e68-b934-1f922744302d


- Dot-repeatable
- pure-VimScript

## Dependencies

- [gw31415/deepl.vim](https://github.com/gw31415/deepl.vim)
  - cURL ( in `deepl.vim` )

## Example

If you are using dein.vim, set up as follows:

```toml
[[plugins]]
repo = "gw31415/deepl.vim"
hook_source = "let g:deepl_authkey='XXXXXXXXX'"

[[plugins]]
repo = "gw31415/deepl-operator.vim"
depends = ["deepl.vim"]
on_map = { nx = "cl" }
hook_source = '''
    nmap cl <Plug>(deepl-replace)
    xmap cl <Plug>(deepl-replace)
    nmap cll <Plug>(deepl-replace)_
'''
```

## Related Plugins

- [gw31415/deepl.vim](https://github.com/gw31415/deepl.vim)
- [gw31415/deepl-commands.nvim](https://github.com/gw31415/deepl-commands.nvim)
