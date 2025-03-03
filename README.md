# DocGen4
Document Generator for Lean 4

## Usage
You can call `doc-gen4` from the top of a Lake project like this:
```sh
$ /path/to/doc-gen4 Module
```

where `Module` is one or more of the top level modules you want to document.
The tool will then proceed to compile the project using lake (if that hasn't happened yet),
analyze it and put the result in `./build/doc`.
You could e.g. host the files locally with the built-in Python webserver:
```sh
$ cd build/doc && python -m http.server
```

## Develop

Enable auto loading dependencies into the shell with `direnv allow` or manually with `nix develop`.

## Building

Build with `nix build .`

## Tests

Run tests with `nix run .#test`

