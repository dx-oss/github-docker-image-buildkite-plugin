# Pack docker image and push them to a registry

Buildkite plugin that pack docker project(s) and push them to a registry

## TODO

* Rewrite it to use go instead as version 2

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: ls
    plugins:
      dx-oss/dockerimage#v1:
        version: '0.0.1'
```

## Configuration

### `name` (Required, string)

The file name pattern, for example `*.ts`. Supports any pattern supported by [find -name](http://man7.org/linux/man-pages/man1/find.1.html).

## Developing

To run the tests:

```shell
docker-compose run --rm tests
```

## Contributing

1. Fork the repo
2. Make the changes
3. Run the tests
4. Commit and push your changes
5. Send a pull request