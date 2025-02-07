# Changelog

## [1.2.0](https://github.com/folke/snacks.nvim/compare/v1.1.0...v1.2.0) (2024-11-11)


### Features

* **bufdelete:** added `wipe` option. Closes [#38](https://github.com/folke/snacks.nvim/issues/38) ([5914cb1](https://github.com/folke/snacks.nvim/commit/5914cb101070956a73462dcb1c81c8462e9e77d7))
* **lazygit:** allow overriding extra lazygit config options ([d2f4f19](https://github.com/folke/snacks.nvim/commit/d2f4f1937e6fa97a48d5839d49f1f3012067bf45))
* **notifier:** added `refresh` option configurable ([df8c9d7](https://github.com/folke/snacks.nvim/commit/df8c9d7724ade9f3c63277f08b237ac3b32b6cfe))
* **notifier:** added backward compatibility for nvim-notify's replace option ([9b9777e](https://github.com/folke/snacks.nvim/commit/9b9777ec3bba97b3ddb37bd824a9ef9a46955582))
* **words:** add `fold_open` and `set_jump_point` config options ([#31](https://github.com/folke/snacks.nvim/issues/31)) ([5dc749b](https://github.com/folke/snacks.nvim/commit/5dc749b045e62e30a156ca8522416a6d1ca9a959))


### Bug Fixes

* added compatibility with Neovim &gt;= 0.9.4 ([4f99818](https://github.com/folke/snacks.nvim/commit/4f99818b0ab98510ab8987a0427afc515fb5f76b))
* **bufdelete:** opts.wipe. See [#38](https://github.com/folke/snacks.nvim/issues/38) ([0efbb93](https://github.com/folke/snacks.nvim/commit/0efbb93e0a4405b955d574746eb57ef6d48ae386))
* **notifier:** take title/footer into account to determine notification width. Fixes [#54](https://github.com/folke/snacks.nvim/issues/54) ([09a6f17](https://github.com/folke/snacks.nvim/commit/09a6f17eccbb551797f522403033f48e63a25f74))
* **notifier:** update layout on vim resize ([7f9f691](https://github.com/folke/snacks.nvim/commit/7f9f691a12d0665146b25a44323f21e18aa46c24))
* **terminal:** `gf` properly opens file ([#45](https://github.com/folke/snacks.nvim/issues/45)) ([340cc27](https://github.com/folke/snacks.nvim/commit/340cc2756e9d7ef0ae9a6f55cdfbfdca7a9defa7))
* **terminal:** pass a list of strings to termopen to prevent splitting. Fixes [#59](https://github.com/folke/snacks.nvim/issues/59) ([458a84b](https://github.com/folke/snacks.nvim/commit/458a84bd1db856c21f234a504ec384191a9899cf))


### Performance Improvements

* **notifier:** only force redraw for new windows and for updated while search is not active. Fixes [#52](https://github.com/folke/snacks.nvim/issues/52) ([da86b1d](https://github.com/folke/snacks.nvim/commit/da86b1deff9a0b1bb66f344241fb07577b6463b8))
* **win:** don't try highlighting snacks internal filetypes ([eb8ab37](https://github.com/folke/snacks.nvim/commit/eb8ab37f6ac421eeda2570257d2279bd12700667))
* **win:** prevent treesitter and syntax attaching to scratch buffers ([cc80f6d](https://github.com/folke/snacks.nvim/commit/cc80f6dc1b7a286cb06c6321bfeb1046f7a59418))

## [1.1.0](https://github.com/folke/snacks.nvim/compare/v1.0.0...v1.1.0) (2024-11-08)


### Features

* **bufdelete:** optional filter and shortcuts to delete `all` and `other` buffers. Closes [#11](https://github.com/folke/snacks.nvim/issues/11) ([71a2346](https://github.com/folke/snacks.nvim/commit/71a234608ffeebfa8a04c652834342fa9ce508c3))
* **debug:** simple log function to quickly log something to a debug.log file ([fc2a8e7](https://github.com/folke/snacks.nvim/commit/fc2a8e74686c7c347ed0aaa5eb607874ecdca288))
* **docs:** docs for highlight groups ([#13](https://github.com/folke/snacks.nvim/issues/13)) ([964cd6a](https://github.com/folke/snacks.nvim/commit/964cd6aa76f3608c7e379b8b1a483ae19f57e279))
* **gitbrowse:** choose to open repo, branch or file. Closes [#10](https://github.com/folke/snacks.nvim/issues/10). Closes [#17](https://github.com/folke/snacks.nvim/issues/17) ([92da87c](https://github.com/folke/snacks.nvim/commit/92da87c910a9b1421e8baae2e67020565526fba8))
* **notifier:** added history to notifier. Closes [#14](https://github.com/folke/snacks.nvim/issues/14) ([65d8c8f](https://github.com/folke/snacks.nvim/commit/65d8c8f00b6589b44410301b790d97c268f86f85))
* **notifier:** added option to show notifs top-down or bottom-up. Closes [#9](https://github.com/folke/snacks.nvim/issues/9) ([080e0d4](https://github.com/folke/snacks.nvim/commit/080e0d403924e1e62d3b88412a41f3ab22594049))
* **notifier:** allow overriding hl groups per notification ([8bcb2bc](https://github.com/folke/snacks.nvim/commit/8bcb2bc805a1785208f96ad7ad96690eee50c925))
* **notifier:** allow setting dynamic options ([36e9f45](https://github.com/folke/snacks.nvim/commit/36e9f45302bc9c200c76349ecd79a319a5944d8c))
* **win:** added default hl groups for windows ([8c0f10b](https://github.com/folke/snacks.nvim/commit/8c0f10b9dade154d355e31aa3f9c8c0ba212205e))
* **win:** allow setting `ft` just for highlighting without actually changing the `filetype` ([cad236f](https://github.com/folke/snacks.nvim/commit/cad236f9bbe46fbb53127014731d8507a3bc80af))
* **win:** disable winblend when colorscheme is transparent. Fixes [#26](https://github.com/folke/snacks.nvim/issues/26) ([12077bc](https://github.com/folke/snacks.nvim/commit/12077bcf65554b585b1f094c69746df402433132))
* **win:** equalize splits ([e982aab](https://github.com/folke/snacks.nvim/commit/e982aabefdf0b1d00ddd850152921e577cd980cc))
* **win:** util methods to handle buffer text ([d3efb92](https://github.com/folke/snacks.nvim/commit/d3efb92aa546eb160782e24e305f74a559eec212))
* **win:** win:focus() ([476fb56](https://github.com/folke/snacks.nvim/commit/476fb56bfd8e32a2805f46fadafbc4eee7878597))
* **words:** `jump` optionally shows notification with reference count ([#23](https://github.com/folke/snacks.nvim/issues/23)) ([6a3f865](https://github.com/folke/snacks.nvim/commit/6a3f865357005c934e2b5ad2cfadaa038775e9e0))
* **words:** configurable mode to show references. Defaults to n, i, c. Closes [#18](https://github.com/folke/snacks.nvim/issues/18) ([d079fbf](https://github.com/folke/snacks.nvim/commit/d079fbfe354ebfec18c4e1bfd7fee695703e3692))


### Bug Fixes

* **config:** deepcopy config where needed ([6c76f91](https://github.com/folke/snacks.nvim/commit/6c76f913981663ec0dba39686018cbc2ff3220b8))
* **config:** fix reading config during setup. Fixes [#2](https://github.com/folke/snacks.nvim/issues/2) ([0d91a4e](https://github.com/folke/snacks.nvim/commit/0d91a4e364866e407901020b59121883cbfb1cf1))
* **notifier:** re-apply winhl since level might have changed with a replace ([b8cc93e](https://github.com/folke/snacks.nvim/commit/b8cc93e273fd481f2b3b7785f64e301d70fd8e45))
* **notifier:** set default conceallevel=2 ([662795c](https://github.com/folke/snacks.nvim/commit/662795c2855b7bfd5e6ec254e469284dacdabb3f))
* **notifier:** try to keep layout when replacing notifs ([9bdb24e](https://github.com/folke/snacks.nvim/commit/9bdb24e735458ea4fd3974939c33ea78cbba0212))
* **terminal:** dont overwrite user opts ([0b08d28](https://github.com/folke/snacks.nvim/commit/0b08d280b605b2e460c1fd92bc87152e66f14430))
* **terminal:** user options ([334895c](https://github.com/folke/snacks.nvim/commit/334895c5bb2ed04f65800abaeb91ccb0487b0f1f))
* **win:** better winfixheight and winfixwidth for splits ([8be14c6](https://github.com/folke/snacks.nvim/commit/8be14c68a7825fff90ca071f0650657ba88da423))
* **win:** disable sidescroloff in minimal style ([107d10b](https://github.com/folke/snacks.nvim/commit/107d10b52e54828606a645517b55802dd807e8ad))
* **win:** dont center float when `relative="cursor"` ([4991e34](https://github.com/folke/snacks.nvim/commit/4991e347dcc6ff6c14443afe9b4d849a67b67944))
* **win:** properly resolve user styles as last ([cc5ee19](https://github.com/folke/snacks.nvim/commit/cc5ee192caf79446d58cbc09487268aa1f86f405))
* **win:** set border to none for backdrop windows ([#19](https://github.com/folke/snacks.nvim/issues/19)) ([f5602e6](https://github.com/folke/snacks.nvim/commit/f5602e60c325f0c60eb6f2869a7222beb88a773c))
* **win:** simpler way to add buffer padding ([f59237f](https://github.com/folke/snacks.nvim/commit/f59237f1dcdceb646bf2552b69b7e2040f80f603))
* **win:** update win/buf opts when needed ([5fd9c42](https://github.com/folke/snacks.nvim/commit/5fd9c426e850c02489943d7177d9e7fddec5e589))
* **words:** disable notify_jump by default ([9576081](https://github.com/folke/snacks.nvim/commit/9576081e871a801f60367e7180543fa41c384755))


### Performance Improvements

* **notifier:** index queue by id ([5df4394](https://github.com/folke/snacks.nvim/commit/5df4394c60958635bf4651d8d7e25f53f48a3965))
* **notifier:** optimize layout code ([8512896](https://github.com/folke/snacks.nvim/commit/8512896228b3e37e3d02c68fa739749c9f0b9838))
* **notifier:** skip processing queue when free space is smaller than min height ([08190a5](https://github.com/folke/snacks.nvim/commit/08190a545857ef09cb6ada4337fe7ec67d3602a9))
* **win:** skip events when setting buf/win options. Trigger FileType on BufEnter only if needed ([61496a3](https://github.com/folke/snacks.nvim/commit/61496a3ef00bd67afb7affcb4933905910a6283c))

## 1.0.0 (2024-11-06)


### Features

* added debug ([6cb43f6](https://github.com/folke/snacks.nvim/commit/6cb43f603360c6fc702b5d7c928dfde22d886e2f))
* added git ([f0a9991](https://github.com/folke/snacks.nvim/commit/f0a999134738c54dccb78ae462774eb228614221))
* added gitbrowse ([a638d8b](https://github.com/folke/snacks.nvim/commit/a638d8bafef85ac6046cfc02e415a8893e0391b9))
* added lazygit ([fc32619](https://github.com/folke/snacks.nvim/commit/fc32619734e4d3c024b8fc2db941c8ac19d2dd6c))
* added notifier ([44011dd](https://github.com/folke/snacks.nvim/commit/44011ddf0da07d0fa89734d21bb770f01a630077))
* added notify ([f4e0130](https://github.com/folke/snacks.nvim/commit/f4e0130ec3cb0299a3a85c589250c114d46f53c2))
* added toggle ([28c3029](https://github.com/folke/snacks.nvim/commit/28c30296991ac5549b49b7ecfb49f108f70d76ba))
* better buffer/window vars for terminal and float ([1abce78](https://github.com/folke/snacks.nvim/commit/1abce78a8b826943d5055464636cd9fad074b4bb))
* bigfile ([8d62b28](https://github.com/folke/snacks.nvim/commit/8d62b285d5026e3d7c064d435c424bab40d1910a))
* **bigfile:** show message when bigfile was detected ([fdc0d3d](https://github.com/folke/snacks.nvim/commit/fdc0d3d1f80a6be64e85a5a25dc34693edadd73f))
* bufdelete ([cc5353f](https://github.com/folke/snacks.nvim/commit/cc5353f6b3f3f3869e2110b2d3d1a95418653213))
* config & setup ([c98c4c0](https://github.com/folke/snacks.nvim/commit/c98c4c030711a59e6791d8e5cab7550e33ac2d2d))
* **config:** get config for snack with defaults and custom opts ([b3d08be](https://github.com/folke/snacks.nvim/commit/b3d08beb8c60fddc6bfbf96ac9f45c4db49e64af))
* **debug:** added simple profile function ([e1f736d](https://github.com/folke/snacks.nvim/commit/e1f736d71fb9020a09019a49d645d4fe6d9f30db))
* **docs:** better handling of overloads ([038b283](https://github.com/folke/snacks.nvim/commit/038b28319c3a4eba7220a679a5759c06e69b8493))
* ensure Snacks global is available when not using setup ([f0458ba](https://github.com/folke/snacks.nvim/commit/f0458bafb059da9885de4fbab1ae5cb6ce2cd0bb))
* float ([d106107](https://github.com/folke/snacks.nvim/commit/d106107cdccc7ecb9931e011a89df6011eed44c4))
* **float:** added support for splits ([977a3d3](https://github.com/folke/snacks.nvim/commit/977a3d345b6da2b819d9bc4870d3d8a7e026728e))
* **float:** better key mappings ([a171a81](https://github.com/folke/snacks.nvim/commit/a171a815b3acd72dd779781df5586a7cd6ddd649))
* initial commit ([63a24f6](https://github.com/folke/snacks.nvim/commit/63a24f6eb047530234297460a9b7ccd6af0b9858))
* **notifier:** add 1 cell left/right padding and make wrapping work properly ([efc9699](https://github.com/folke/snacks.nvim/commit/efc96996e5a98b619e87581e9527c871177dee52))
* **notifier:** added global keep config option ([f32d82d](https://github.com/folke/snacks.nvim/commit/f32d82d1b705512eb56c901d4d7de68eedc827b1))
* **notifier:** added minimal style ([b29a6d5](https://github.com/folke/snacks.nvim/commit/b29a6d5972943cb8fcfdfb94610d850f0ba050b3))
* **notifier:** allow closing notifs with `q` ([97acbbb](https://github.com/folke/snacks.nvim/commit/97acbbb654d13a0d38792fd6383973a2ca01a2bf))
* **notifier:** allow config of default filetype ([8a96888](https://github.com/folke/snacks.nvim/commit/8a968884098be83acb42f31a573e62b63420268e))
* **notifier:** enable wrapping by default ([d02aa2f](https://github.com/folke/snacks.nvim/commit/d02aa2f7cb49273330fd778818124ddb39838372))
* **notifier:** keep notif open when it's the current window ([1e95800](https://github.com/folke/snacks.nvim/commit/1e9580039b706cfc1f526fea2e46b6857473420b))
* quickfile ([d0ce645](https://github.com/folke/snacks.nvim/commit/d0ce6454f95fe056c65324a0f59a250532a658f3))
* rename ([fa33688](https://github.com/folke/snacks.nvim/commit/fa336883019110b8f525081665bf55c19df5f0aa))
* statuscolumn ([99b1700](https://github.com/folke/snacks.nvim/commit/99b170001592fe054368a220599da546de64894e))
* terminal ([e6cc7c9](https://github.com/folke/snacks.nvim/commit/e6cc7c998afa63eaf126d169f4702953f548d39f))
* **terminal:** allow to override the default terminal implementation (like toggleterm) ([11c9ee8](https://github.com/folke/snacks.nvim/commit/11c9ee83aa133f899dad966224df0e2d7de236f2))
* **terminal:** better defaults and winbar ([7ceeb47](https://github.com/folke/snacks.nvim/commit/7ceeb47e545619dff6dd8853f0a368afae7d3ec8))
* **terminal:** better double esc to go to normal mode ([a4af729](https://github.com/folke/snacks.nvim/commit/a4af729b2489714b066ca03f008bf5fe42c93343))
* **win:** better api to deal with sizes ([ac1a50c](https://github.com/folke/snacks.nvim/commit/ac1a50c810c5f67909921592afcebffa566ee3d3))
* **win:** custom views ([12d6f86](https://github.com/folke/snacks.nvim/commit/12d6f863f73cbd3580295adc5bc546c9d10e9e7f))
* words ([73445af](https://github.com/folke/snacks.nvim/commit/73445af400457722508395d18d2c974965c53fe2))


### Bug Fixes

* **config:** don't change defaults in merge ([6e825f5](https://github.com/folke/snacks.nvim/commit/6e825f509ed0e41dbafe5bca0236157772344554))
* **config:** merging of possible nil values ([f5bbb44](https://github.com/folke/snacks.nvim/commit/f5bbb446ed012361bbd54362558d1f32476206c7))
* **debug:** exclude vimrc from callers ([8845a6a](https://github.com/folke/snacks.nvim/commit/8845a6a912a528f63216ffe4b991b025c8955447))
* **float:** don't use backdrop for splits ([5eb64c5](https://github.com/folke/snacks.nvim/commit/5eb64c52aeb7271a3116751f1ec61b00536cdc08))
* **float:** only set default filetype if no ft is set ([66b2525](https://github.com/folke/snacks.nvim/commit/66b252535c7a78f0cd73755fad22b07b814309f1))
* **float:** proper closing of backdrop ([a528e77](https://github.com/folke/snacks.nvim/commit/a528e77397daea422ff84dde64124d4a7e352bc2))
* **notifier:** modifiable ([fd57c24](https://github.com/folke/snacks.nvim/commit/fd57c243015e6f2c863bb6c89e1417e77f3e0ea4))
* **notifier:** modifiable = false ([9ef9e69](https://github.com/folke/snacks.nvim/commit/9ef9e69620fc51d368fcee830a59bc9279594d43))
* **notifier:** show notifier errors with nvim_err_writeln ([e8061bc](https://github.com/folke/snacks.nvim/commit/e8061bcda095e3e9a3110ce697cdf7155e178d6e))
* **notifier:** sorting ([d9a1f23](https://github.com/folke/snacks.nvim/commit/d9a1f23e216230fcb2060e74056778d57d1d7676))
* simplify setup ([787b53e](https://github.com/folke/snacks.nvim/commit/787b53e7635f322bf42a42279f647340daf77770))
* **win:** backdrop ([71dd912](https://github.com/folke/snacks.nvim/commit/71dd912763918fd6b7fd07dd66ccd16afd4fea78))
* **win:** better implementation of window styles (previously views) ([6681097](https://github.com/folke/snacks.nvim/commit/66810971b9bd08e212faae467d884758bf142ffe))
* **win:** dont error when augroup is already deleted ([8c43597](https://github.com/folke/snacks.nvim/commit/8c43597f10dc2916200a8c857026f3f15fd3ae65))
* **win:** dont update win opt noautocmd ([a06e3ed](https://github.com/folke/snacks.nvim/commit/a06e3ed8fcd08aaf43fc2454bb1b0f935053aca7))
* **win:** no need to set EndOfBuffer winhl ([7a7f221](https://github.com/folke/snacks.nvim/commit/7a7f221020e024da831c2a3d72f8a9a0c330d711))
* **win:** use syntax as fallback for treesitter ([f3b69a6](https://github.com/folke/snacks.nvim/commit/f3b69a617a57597571fcf4263463f989fa3b663d))


### Performance Improvements

* **win:** set options with eventignore and handle ft manually ([80d9a89](https://github.com/folke/snacks.nvim/commit/80d9a894f9d6b2087e0dfee6d777e7b78490ba93))
