# fuzzbench-lava-assets

A place to store various Fuzz Bench binaries that have had LAVA bugs injected.

I chose six binaries from the [FuzzBench repo](https://github.com/google/fuzzbench/tree/master/benchmarks).
I provide the direct external link for the tarball for confirmation of the package

1. [lcms v2.19.1](https://github.com/mm2/Little-CMS/releases/download/lcms2.19.1/lcms2-2.19.1.tar.gz)
2. [libxml v2.15.3](https://gitlab.gnome.org/GNOME/libxml2/-/archive/v2.15.3/libxml2-v2.15.3.tar.gz)
3. [openssl v3.0.7](https://github.com/openssl/openssl/archive/refs/tags/openssl-3.0.7.tar.gz). I chose this to match the branch implying it used 3.0.7
4. [sqllite](https://sqlite.org/src/tarball/sqlite.tar.gz?r=c78cbf2e86850cc6), I used the same tarball as FuzzBench, see the container.
5. [libpng v.1.6.53](https://github.com/pnggroup/libpng/archive/refs/tags/v1.6.53.tar.gz)
6. [freetype2](git clone git://git.sv.nongnu.org/freetype/freetype2.git), I used the same tarball as FuzzBench, see the container.

To complete the experiment, the only thing I had to do was update the docker files in the fork I created shown [here](https://github.com/andrewQuijano/fuzzbench).

## To inject bugs from scratch
Follow the instructions on both [installing and setting up LAVA](https://github.com/panda-re/lava/wiki/LAVA-Wiki).
