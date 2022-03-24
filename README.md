Add (at the moment, very basic) support for documenting Lua using [comment-helper](https://github.com/ismaelpadilla/comment-helper.nvim/).

<p align="center">
  <img alt="Preview" src="https://i.imgur.com/cvif4Vx.gif">
</p>

### Features

- Supports snippets if you have [LuaSnip](https://github.com/L3MON4D3/LuaSnip) enabled.
- Supports the following Lua node types:
  - function_declaration

### Installation

```viml
Plug 'ismaelpadilla/comment-helper.nvim' " base plugin
Plug 'ismaelpadilla/comment-helper-lua.nvim'
```

### Configuration

```lua
local ch = require("comment_helper")
local ch_lua = require("comment_helper_lua")

ch.set_ignored_types("lua", {"chunk"})
ch.add("lua", "function_declaration", ch_lua.function_declaration)
```
