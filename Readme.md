# How to use sphinxdoc on github

[see also](https://github.com/sphinx-doc/sphinx/issues/3382)

## Steps

1. Create folder `docs` in root directory of `main` branch
2. Go `docs` directory and enter and keep all the defaults

    ```bash
    $ sphinx-quickstart
    ```
3. Create file `docs/index.html` with the following content

    ```html
    <meta http-equiv="refresh" content="0; url=./html/index.html" />
    ```

4. Create empty file `docs/.nojekyll`
5. In `docs` generate docs with `make html`
6. In github, change *GitHub Pages* settings to source to _master branch /doc folder_

## The result

[Generated Documentation](https://jradek.github.io/sphinxdoc-test/_build/html/index.html)
