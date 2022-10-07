# tuwien_prog_vscode_c_template

## How to use

1. Install all recommended extensions.

2. Open either `task1.c` or `task2.c`.
3. Open `Run and Debug` in the `Activity bar`.
4. There you can select either `GDB Debug` or `LLDB Debug`.

* To use `GDB Debug` install `gdb`.
* To use `LLDB Debug` install `clang`.
* To use `clangd` install `clang`.

Note:
You may move the task files anywhere you want.
You may rename them to anything you like.
However, they must not use other `*.c` files header files are fine though.

## How it works

There are two files at work:
* `.vscode/tasks.json`:
This file defines a vscode task to automatically build the currently open `*.c` file.
It is automatically called by `launch.json`.

* `.vscode/launch.json`:
This file defines two debug configurations.
You may use either one of them.
I personally like `lldb` better. </br>
It runs the build task.
Then it launches the built executable and attaches a debugger.