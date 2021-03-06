# Docs template.

This repository
contains a template for documentation, using Pandoc.

To see a live HTML version, go [here](https://marcofavorito.me/docs-template).

## Build

We use [Pandoc](https://pandoc.org/) to build the document in PDF and HTML formats.

In particular, on Ubuntu, you will need the following packages:

```
sudo apt-get install -y pandoc pandoc-citeproc latexmk texlive-xetex
```

Then, just call `make`.

Otherwise, you can use the Docker image with all the needed dependencies:
```
docker build -t pandoc .
docker run -v$(pwd):/build -it pandoc /bin/bash -c "cd /build && make"
```

The output is in HTML format in `index.html` and 
in PDF format in `main.pdf`.

## Contribute

To contribute, please 
[open an issue](https://github.com/marcofavorito/tl-grammars/issues),
[submit a PR](https://github.com/marcofavorito/tl-grammars/pulls),
or [contact the maintainer](mailto:favorito@diag.uniroma1.it) for a discussion.


## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

