# conan-configuration
Stores Conan configuration which is common to all our build images.

The configuration from this repository can be installed using the `conan config install` command, see
https://docs.conan.io/en/latest/reference/commands/consumer/config.html#conan-config-install

**Beware, installing this configuration will delete any other other remotes you may have configured.**

The important things done by installing this configuration are:
- setting the remotes to the ones we use in our projects
- adding the compiler.libc setting for gcc and clang, so that packages can be built against glibc or musl, this is useful for builds on Alpine Linux where musl is used.
