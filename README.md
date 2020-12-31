# GitHub Action for Sleeping 💤

This action allows you to wait a specified amount of time before moving on in your workflow.

Input follows the Linux `sleep` syntax for time units: a number followed by `s` for seconds, `m` for minutes, etc. [Man page for `sleep` here.](https://linux.die.net/man/1/sleep)

## Usage

```yaml
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
    - name: Sleep for 30 seconds
      uses: kibertoad/wait-action@1.0.1
      with:
        time: '30s'
```


## License

This project is distributed under the [MIT license](LICENSE.md).
