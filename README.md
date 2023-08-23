# conan-configuration
Stores Conan configuration which is common to all our build images.

The configuration from this repository can be installed using the `conan config install` command:
```
conan config install http://github.com/ess-dmsc/conan-configuration.git
```

**Beware, installing this configuration will delete any other other remotes you may have configured.**

The important things done by installing this configuration are:
- setting the remotes to the ones we use in our projects
- adding distro setting for CentOS and AlmaLinux
