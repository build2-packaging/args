# build2 Package for args

This project builds and defines the build2 package for [args](https://github.com/taywee/args), which is a simple, small, flexible, single-header C++11 argument parsing library.

[![Official](https://img.shields.io/website/https/github.com/taywee/args.svg?down_message=offline&label=Official&style=for-the-badge&up_color=blue&up_message=online)](https://github.com/taywee/args)
[![build2](https://img.shields.io/website/https/github.com/build2-packaging/args.svg?down_message=offline&label=build2&style=for-the-badge&up_color=blue&up_message=online)](https://github.com/build2-packaging/args)
[![cppget.org](https://img.shields.io/website/https/cppget.org/args.svg?down_message=offline&label=cppget.org&style=for-the-badge&up_color=blue&up_message=online)](https://cppget.org/args)
[![queue.cppget.org](https://img.shields.io/website/https/queue.cppget.org/args.svg?down_message=empty&down_color=blue&label=queue.cppget.org&style=for-the-badge&up_color=orange&up_message=running)](https://queue.cppget.org/args)

## Usage
Make sure to add the stable section of the `cppget.org` repository to your project's `repositories.manifest` to be able to fetch this package.

    :
    role: prerequisite
    location: https://pkg.cppget.org/1/stable
    # trust: ...

If the stable section of `cppget.org` is not an option then add this Git repository itself instead as a prerequisite.

    :
    role: prerequisite
    location: https://github.com/build2-packaging/args.git

Add the respective dependency in your project's `manifest` file to make the package available for import.

    depends: args ^6.4.7

The library can be imported by the following declaration in a `buildfile`.

    import args = args%lib{args}

## Configuration
There are no configuration options available.

## Issues
Currently, there are no known issues.

## Contributing
Thank you in advance for your help and contribution to keep this package up-to-date.
Please, file an issue on [GitHub](https://github.com/build2-packaging/glm/issues) for questions, bug reports, or to recommend updating the package version.
If you're making a pull request to fix bugs or update the package version yourself, refer to the [`build2` Packaging Guidelines](https://build2.org/build2-toolchain/doc/build2-toolchain-packaging.xhtml#core-version-management).
