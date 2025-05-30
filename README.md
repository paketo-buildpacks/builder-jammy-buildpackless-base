# Paketo Jammy Buildpackless Base Builder

## `paketobuildpacks/builder-jammy-buildpackless-base:latest`

This builder uses the [Paketo Jammy Base
Stack](https://github.com/paketo-buildpacks/jammy-base-stack) (an Ubuntu Jammy
base image) and contains **no buildpacks nor order groups**. To use this
builder, you must specify buildpacks at build time using whatever mechanisms
your CNB platform of choice offers.

For example, with the `pack` CLI, use `--buildpack` as follows:
```bash
pack build dotnet-with-buildpackless-builder \
--buildpack index.docker.io/paketobuildpacks/dotnet-core \
--builder paketobuildpacks/builder-jammy-buildpackless-base:latest
```

To see which versions of build and run images and the lifecycle are contained
within a given builder version, see the
[Releases](https://github.com/paketo-buildpacks/builder-jammy-buildpackless-base/releases)
on this repo. This information is also available in the `builder.toml`.

For more information about this builder and how to use it, visit the [Paketo
builder documentation](https://paketo.io/docs/builders/).  To learn about the
stack included in this builder, visit the [Paketo stack
documentation](https://paketo.io/docs/stacks/).

