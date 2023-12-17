# start
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

source $HOME/.cargo/env

rustup install stable

rustup update stable

rustup default stable

git clone https://github.com/AleoHQ/leo
cd leo.

apt install clang gcc libssl-dev pkg-config

cargo install --path .

git clone https://github.com/AleoHQ/snarkOS.git --depth 1
cd snarkOS.

./build_ubuntu.sh


