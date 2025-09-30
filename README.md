License
-------
PyBLOCK is released under the terms of the MIT license.
See [COPYING](COPYING) for more information or see https://opensource.org/licenses/MIT.

git clone https://github.com/PyBLOCK-Bitcoin/bitcoin.git
cd bitcoin
mkdir build
cd build
cmake .. -DCMAKE_INSTALL_PREFIX="" -DBUILD_DAEMON="ON" -DBUILD_CLI="ON" -DBUILD_GUI="ON"
cmake --build . --target install --parallel $(nproc)
cd bin
./bitcoin-qt
