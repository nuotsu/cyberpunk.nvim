# cyberpunk.nvim

A Neovim colorscheme based on the Cyberpunk 2077 UI palette: mainly **red on black**, with **cyan** and **amber** as accents and the secondary colors for supplemental roles.

Palette source: [Cyberpunk 2077 User Interface (Part 2)](https://www.behance.net/gallery/133185623/Cyberpunk-2077User-Interface-(Part-2)) by Vladimír Vilímovský, © CD PROJEKT RED. This is an unofficial fan project.

| Role | Color | Hex |
|---|---|---|
| Background | Darkest blue | `#0E0E17` |
| Primary | Red | `#F75049` |
| Accent | Cyan | `#5EF6FF` |
| Accent | Gold (amber) | `#F0B537` |
| Supplemental | Orange | `#FB932E` |
| Supplemental | Green | `#1DED83` |
| Supplemental | Purple | `#9D2BF5` |
| Supplemental | Blue | `#2570D4` |
| Text | Grey | `#D6D0D0` |

## Install

lazy.nvim:

```lua
{
  "mitchuman/cyberpunk.nvim",
  lazy = false,
  priority = 1000,
  config = function()
    vim.cmd.colorscheme("cyberpunk")
  end,
}
```

Or just `:colorscheme cyberpunk` after installing by any other means.

## Notes

- Git gutter: green added, amber changed, red removed.
- Template delimiters (`{{ }}`, `{% %}`, `<% %>`) are cyan; variables inside are green.
- CSS ids/classes are green; Tailwind at-rules (`@theme`, `@utility`, `@apply`, ...) are cyan, with classes after `@apply` in green.
- JSON keys are cyan, values amber.
- Works with and without treesitter parsers (legacy syntax groups are covered too).
- Plugin highlights included: gitsigns, snacks, telescope, blink.cmp / nvim-cmp, which-key, noice, flash, neo-tree, mini.icons.

## License

MIT. The palette colors belong to CD PROJEKT RED.
