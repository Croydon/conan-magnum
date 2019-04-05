[![Download](https://api.bintray.com/packages/bincrafters/public-conan/magnum%3Abincrafters/images/download.svg) ](https://bintray.com/bincrafters/public-conan/magnum%3Abincrafters/_latestVersion)
[![Build Status Travis](https://travis-ci.com/bincrafters/conan-magnum.svg?branch=stable%2F2019.01)](https://travis-ci.com/bincrafters/conan-magnum)
[![Build Status AppVeyor](https://ci.appveyor.com/api/projects/status/github/bincrafters/conan-magnum?branch=stable%2F2019.01&svg=true)](https://ci.appveyor.com/project/bincrafters/conan-magnum)

## Conan package recipe for [*magnum*](https://magnum.graphics)

Magnum — Lightweight and modular C++11/C++14                     graphics middleware for games and data visualization

The packages generated with this **conanfile** can be found on [Bintray](https://bintray.com/bincrafters/public-conan/magnum%3Abincrafters).


## Issues

If you wish to report an issue or make a request for a package, please do so here:

[Issues Tracker](https://github.com/bincrafters/community/issues)


## For Users

### Basic setup

    $ conan install magnum/2019.01@bincrafters/stable

### Project setup

If you handle multiple dependencies in your project is better to add a *conanfile.txt*

    [requires]
    magnum/2019.01@bincrafters/stable

    [generators]
    cmake

Complete the installation of requirements for your project running:

    $ mkdir build && cd build && conan install ..

Note: It is recommended that you run conan install from a build directory and not the root of the project directory.  This is because conan generates *conanbuildinfo* files specific to a single build configuration which by default comes from an autodetected default profile located in ~/.conan/profiles/default .  If you pass different build configuration options to conan install, it will generate different *conanbuildinfo* files.  Thus, they should not be added to the root of the project, nor committed to git.


## Build and package

The following command both runs all the steps of the conan file, and publishes the package to the local system cache.  This includes downloading dependencies from "build_requires" and "requires" , and then running the build() method.

    $ conan create . bincrafters/stable


### Available Options
| Option        | Default | Possible Values  |
| ------------- |:----------------- |:------------:|
| shared      | False |  [True, False] |
| fPIC      | True |  [True, False] |
| build_deprecated      | True |  [True, False] |
| build_multithreaded      | True |  [True, False] |
| build_plugins_static      | False |  [True, False] |
| target_gl      | True |  [True, False] |
| target_gles      | False |  [True, False] |
| with_anyaudioimporter      | False |  [True, False] |
| with_anyimageconverter      | False |  [True, False] |
| with_anyimageimporter      | False |  [True, False] |
| with_anysceneimporter      | False |  [True, False] |
| with_audio      | False |  [True, False] |
| with_debugtools      | True |  [True, False] |
| with_distancefieldconverter      | False |  [True, False] |
| with_eglcontext      | False |  [True, False] |
| with_fontconverter      | False |  [True, False] |
| with_glfwapplication      | False |  [True, False] |
| with_glxapplication      | False |  [True, False] |
| with_glxcontext      | False |  [True, False] |
| with_gl_info      | False |  [True, False] |
| with_imageconverter      | False |  [True, False] |
| with_magnumfont      | False |  [True, False] |
| with_magnumfontconverter      | False |  [True, False] |
| with_meshtools      | True |  [True, False] |
| with_objimporter      | False |  [True, False] |
| with_opengltester      | False |  [True, False] |
| with_primitives      | True |  [True, False] |
| with_scenegraph      | True |  [True, False] |
| with_sdl2application      | True |  [True, False] |
| with_shaders      | True |  [True, False] |
| with_text      | True |  [True, False] |
| with_tgaimageconverter      | False |  [True, False] |
| with_tgaimporter      | False |  [True, False] |
| with_vk      | False |  [True, False] |
| with_wavaudioimporter      | False |  [True, False] |
| with_windowlesseglapplication      | False |  [True, False] |
| with_windowlessglxapplication      | False |  [True, False] |
| with_xeglapplication      | False |  [True, False] |


## Add Remote

    $ conan remote add bincrafters "https://api.bintray.com/conan/bincrafters/public-conan"


## Conan Recipe License

NOTE: The conan recipe license applies only to the files of this recipe, which can be used to build and package magnum.
It does *not* in any way apply or is related to the actual software being packaged.

[MIT](https://github.com/Croydon/conan-magnum/blob/stable/2019.01/LICENSE.md)
