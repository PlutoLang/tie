# Tie

A tool to pack Pluto code and assets into a standalone executable.

## Usage

1. Your code and assets go in `app`.
2. Run **build.pluto** to create the app executables.

## How it works

The [tie runtime](https://github.com/PlutoLang/tie-runtime) is designed in such a way that an entrypoint as well as any other files can be appended, which is what the build script does. The entrypoint then hooks some functions before loading the app's main.pluto.
