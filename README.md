![Noto](images/noto.png)

# Noto Source

Source files for generating Noto fonts.

Note that as of February 2016, no sources are available for the released Noto fonts in [github.com/googlei18n/noto-fonts](https://github.com/googlei18n/noto-fonts). 
The files in this repository are work-in-progress for future versions of the fonts that have not been released yet. 
The designs and glyph sets are not final.

## Building

To build everything from source:

```
$ git clone --recursive https://github.com/googlei18n/noto-source.git
$ cd noto-source
$ make setup
$ make
```

other build options exist:

```bash
$ make -B src/NotoSansUIRoman-MM.glyphs  # build a single source
$ make force  # continue building even when some sources fail
```

be sure to update this repository and its dependencies on subsequent runs:

```
$ git pull
$ git submodule update --recursive
$ make setup
$ ...
```

## License

Noto source (under the src subdirectory) is under the [SIL Open Font License, version 1.1](src/LICENSE).

Build scripts are under the [Apache license, version 2.0](LICENSE).

## Contributing

To contribute to this project, please read [CONTRIBUTING](CONTRIBUTING.md) 

## News

* 2015-12-07: first release, covering Noto Sans UI {Italic, Mono, Roman}, Noto Sans Display {Italic, Roman}, Noto {Sans, Serif} {Armenian, Georgian}.
