# Sublime Text 4 Development Setup

### Integrated Terminal Setup
1. Install Terminus Package
2. `Preferances` » `Package Settings` » `Terminus`  » `Terminus`
3. In `terminus.sublime-Settings--User` paste code from **terminusSettings.js**
4. Save the file and restart Sublime Text


### Key Binding Setup
1. `Preference` » `Package Settings` » `Terminus` » `Key Bindings`
2. In right tab paste code from **terminusKeyBindings.js**
3. Save the file and restart Sublime Text



### Sublime Settings

1]Install fonts from fonts folder
2]Goto Preferences » Settings
3]Copy code from settings.json and paste it in Preference.sublime-Settings --User
4]Save the file and restart Sublime Test


### LSP Clangd(c/c++)
1. install the `LSP package`
2. `$ pip install compiledb`
3. **compiledb** -- *used to generate compile_commands.json file used by clangd and LSP*
4. run command   compile_commands.json file will be generated
`$ compiledb -n make`
5. now start the sublime text

###  Extensions / Packages Used

- A File Icon
- Babel -- Javascript
- Gruvbox -- Color Scheme
- ReactJs
- Typescript
- Emmet
- LSP


### Selection Color
1. Install package resource viewer
2. `ctrl + shift +v `» `search prv` » `package resource viewer : open resources` » `search color scheme` » `themes` »


## Premake5 Visual Studio 2022 setup for c++ development
1. Install [Premake5](https://premake.github.io/)
2. Update the script path of premake5
```sh
$ premake5 /systemscript="C:\Users\Akash Pandit\.premake" vs2022
```
2. Add the lua folder in repo to `C:/Program Files/premake`
3. Run the following command in c++ working project folder to generate compile_commands.json
```sh
$ premake5 compiledb
```