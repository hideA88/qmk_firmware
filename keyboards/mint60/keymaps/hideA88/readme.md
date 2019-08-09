# The default keymap for Mint60

see https://shanpu.hatenablog.com/entry/2018/11/15/105238#QMK-Firmware%E3%81%AE%E3%83%AA%E3%83%9D%E3%82%B8%E3%83%88%E3%83%AA%E3%82%92%E3%82%AF%E3%83%AD%E3%83%BC%E3%83%B3%E3%81%99%E3%82%8B

## modify keymap

see https://docs.qmk.fm/#/keycodes

## build mint60 firmware

`docker run --rm -e KEYMAP=hideA88 -e KEYBOARD=mint60 -v $('pwd'):/qmk_firmware edasque/qmk_firmware`
`cp .build build`

## write firmware

1. install from homebrew

```
brew tap osx-cross/avr
brew tap PX4/homebrew-px4
brew update
brew install avr-gcc
brew install dfu-programmer
brew install gcc-arm-none-eabi
brew install avrdude
```

2. install qmk_toolbox

https://github.com/qmk/qmk_toolbox/releases

3. run app

-   select build hex file. and check auto flash.
-   push reset button of keyboard.
