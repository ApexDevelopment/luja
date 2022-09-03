# Luja
Luja (lou-yah) is a Lua virtual machine written in the excellent [Jakt](https://github.com/SerenityOS/jakt/) programming language.

It cannot currently interpret `.lua` files directly, they must first be translated to Lua bytecode using `luac <input file>`, which will yield a Lua bytecode file. This can be run with `luja luac.out`.

## Building
Luja can be built on Linux using:
```
> jakt src/main.jakt -I <path to Jakt runtime> -o luja
```
On Windows:
```
> jakt src\main.jakt -I <path to Jakt runtime> -o luja.exe
```

## Etc...
Luja cannot read Lua scripts directly and probably won't for a little while. I plan to implement this eventually. I have never written a Lua parser before, but I hope that this can be my first time.

This project is the first thing I have ever built using Jakt, and so is more of a learning tool for me than something I want to turn into a polished product.