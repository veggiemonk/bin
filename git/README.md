# git

## Usage

Executes git with arguments listed in the Action's `args`.

```workflow
action "Shell" {
  uses = "actions/bin/git@master"
  args = [ "status" ]
  secrets = [ "GITHUB_TOKEN" ]
  env = {
    "GIT_USERNAME" = "Al Gore-Rythim"
    "GIT_EMAIL"    = "alex.blaine@layder.io"
  }
}
```

## License

The Dockerfile and associated scripts and documentation in this project are released under the [MIT License](LICENSE).

Container images built with this project include third party materials. See [THIRD_PARTY_NOTICE.md](THIRD_PARTY_NOTICE.md) for details.
