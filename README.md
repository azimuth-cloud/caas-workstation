# caas-workstation

## Developing locally

To run the GitHub Actions linters locally, use:

```sh
docker run --rm \
    -e RUN_LOCAL=true \
    --env-file "super-linter.env" \
    -v "$(pwd)":/tmp/lint \
    ghcr.io/super-linter/super-linter:v7.3.0
```

```sh
ansible-lint -c .ansible-lint.yml
```
