# C Starter Project Template 

This is a C / TIC-80 starter template.  To build it:

```
export WASI_SDK_PATH=/where/you/installed/WASI
make
```

To import the resulting WASM to a cartridge:

```
tic80 --fs . --cmd 'new wasm & import binary build/cart.wasm & save'
```

Or from the TIC-80 console:

```
new wasm
import binary build/cart.wasm
save
```

This is assuming you've run TIC-80 with `--fs .` inside your project directory.


Alternatively, you can change the script tag of an existing cartridge and then import.

For WASM cartridges the script tag should be written as such:

```
-- script: wasm
```

