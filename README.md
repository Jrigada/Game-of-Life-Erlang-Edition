# Game of Life: Erlang Edition

## Installation

### Binary Distributions

Erlang/OTP is available as pre-built binary packages by most OS package managers.

```sh
apt-get install erlang
```

### Compiling from source

To compile Erlang from source, run the following commands. The complete building and installation instructions [can be found here](HOWTO/INSTALL.md).

```sh
git clone https://github.com/erlang/otp.git
cd otp
```

Checkout the branch or tag of your choice

```sh
git checkout maint-24    # current latest stable version
```

Configure, build and install

```sh
./configure
make
make install
```

Alternatively, you can use [Kerl](https://github.com/kerl/kerl), a script that lets you easily build Erlang with a few commands.

## Execution

Start the Erlang console
```sh
erl
```

Load game of life module
```sh
c(gol).
```

Create a demo_grid already loaded (you can make your custom grid later if you like)
```sh
Grid = gol:demo_grid().
```

Start the simulation specifying the amount of generations you want to simulate (each one is a one second).
```sh
gol:run_simulation(Grid, 60).
```

# TODO
Elixir implementation
