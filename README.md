# seed

This repository contains seed files that almost every repository of Flamego middleware module should have.

## Using the content

1. Create an empty repository on GitHub.com.
1. [Download ZIP](https://github.com/flamego/seed/archive/refs/heads/main.zip) of this repository, unzip to a directory, then rename the directory to match the middleware name.
1. Update the Go module name in the `go.mod` file to match the middleware repository path, e.g.:
    ```diff
    -module github.com/flamego/seed
    +module github.com/flamego/bilibili
    ```
1. Update the package name in the `main.go` and rename the file to match the middleware name, e.g.:
    ```diff
    -package seed
    +package bilibili
    ```
1. Update the `github.repository` in the `.github/workflows/lsif.yml` to match the middleware repository, e.g.:
    ```diff
    -github.repository == 'flamego/seed'
    +github.repository == 'flamego/bilibili'
    ```
1. Update the `import_root` in the `.deepsource.toml` to match the middleware repository, e.g.:
    ```diff
    -import_root = "github.com/flamego/seed"
    +import_root = "github.com/flamego/bilibili"
    ```
3. Update the `README.md` to be about your middleware, a good example is [flamego/template's README](https://github.com/flamego/template/blob/main/README.md).

## Getting help

- Please [file an issue](https://github.com/flamego/flamego/issues) or [start a discussion](https://github.com/flamego/flamego/discussions) on the [flamego/flamego](https://github.com/flamego/flamego) repository.

## License

This project is under the MIT License. See the [LICENSE](LICENSE) file for the full license text.
