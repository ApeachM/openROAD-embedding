# OpenROAD Embedding



This repository is just an example of using OpenROAD as a submodule for an individual repository.

## How to Build

```shell
git clone --recursive https://github.com/ApeachM/openROAD-embedding.git
cd openROAD-embedding
git submodule update --force --recursive --init --remote
cd submodule/OpenROAD/
git fetch
git checkout -b mpl2_library origin/mpl2_library
cd ../../
```

```shell
mkdir build
cd build
cmake ..
make -j openroad-embedding
./openroad-embedding
```

