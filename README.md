# OpenWrt packages feed

## Description

This is the OpenWrt "packages"-feed containing community-maintained build scripts, options and patches for applications, modules and libraries used within OpenWrt.

Installation of pre-built packages is handled directly by the **opkg** utility within your running OpenWrt system or by using the [OpenWrt SDK](https://openwrt.org/docs/guide-developer/using_the_sdk) on a build system.

## Package Directory

The feed is organized into the following categories:

- **admin**: System administration tools and utilities
- **devel**: Development tools, compilers, and debug utilities
- **fonts**: Font packages for various languages and use cases
- **ipv6**: IPv6 related packages and utilities
- **kernel**: Kernel modules and extensions
- **lang**: Programming languages, interpreters, and language-specific libraries
- **libs**: General purpose libraries used by other packages
- **mail**: Mail servers, clients, and mail-related utilities
- **multimedia**: Audio/Video applications, codecs, and multimedia tools
- **net**: Networking applications, protocols, and utilities
- **sound**: Sound applications, drivers, and audio utilities
- **utils**: Various utilities and tools for system management

For a comprehensive list of available packages and their descriptions, see [PACKAGES.md](PACKAGES.md).

## Usage

This repository is intended to be layered on-top of an OpenWrt buildroot. If you do not have an OpenWrt buildroot installed, see the documentation at: [OpenWrt Buildroot – Installation](https://openwrt.org/docs/guide-developer/build-system/install-buildsystem) on the OpenWrt support site.

### Adding the packages feed

This feed is enabled by default. To install all its package definitions, run:
```
./scripts/feeds update packages
./scripts/feeds install -a -p packages
```

### Installing specific packages

To install a specific package:

1. Update the packages feed:
   ```
   ./scripts/feeds update packages
   ```

2. Install the package definition:
   ```
   ./scripts/feeds install <package_name>
   ```

3. Configure the package in the OpenWrt buildroot:
   ```
   make menuconfig
   ```
   Navigate to the appropriate category to find your package.

4. Build the package:
   ```
   make package/<package_name>/compile
   ```

5. Install the compiled package on your OpenWrt device:
   ```
   opkg install <package_name>
   ```

### Using pre-compiled packages

On a running OpenWrt system, you can directly install packages using the `opkg` package manager:

```
opkg update
opkg install <package_name>
```

## Building custom packages

To create a new package, please follow the guidelines in the [CONTRIBUTING.md](CONTRIBUTING.md) file. The basic structure of a package includes:

- Makefile: Contains metadata and build instructions
- Patches (optional): Modifications to the upstream source
- Files (optional): Additional files needed by the package

## License

See [LICENSE](LICENSE) file.
 
## Package Guidelines

See [CONTRIBUTING.md](CONTRIBUTING.md) file.

