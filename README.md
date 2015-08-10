# Miscellaneous

Some random day to day useful stuff I wrote a hundred times. Finally decided to centralize all of this in one place. If you have some code snippets or ideas, feel free to contribute/suggest.

### Converter

Convert a number from base n to m, with n and m between 2 and 62

```sh
/home/hackndo/misc $ ./converter 1c2 16 2
1c2 from base 16 to base 2
111000010
```

### ExecShellcode

Shellcode execution made simple (no perl/python needed)

```sh
/home/hackndo/misc $ ./execshellcode32 "0x31 0xc0 0x50 0x68 0x2f 0x2f 0x73 0x68 0x68 0x2f 0x62 0x69 0x6e 0x89 0xe3 0x89 0xc1 0x89 0xc2 0xb0 0x0b 0xcd 0x80 0x31 0xc0 0x40 0xcd 0x80"
Shellcode Length: 28
$ 
```

### FindAddr

Retrieve any environment variable address

```sh
/home/hackndo/misc $ ./findaddr SHELL
SHELL address: 0x7fff0417d64c
```

### Hex2Str

Converts some hex ascii codes to string (usefull for char like 0x90 in shellcodes, which are not printable)

```sh
/home/hackndo/misc $ ./hex2str "0x68 0x61 0x63 0x6b 0x6e 0x64 0x6f"
hackndo
```
