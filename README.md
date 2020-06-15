![crab pet](https://i.imgur.com/LbZJgmm.gif)

# Solutions for [Rustlings](https://github.com/rust-lang/rustlings) 

This repo contains solutions for exercies in rust.

## Getting Started

_Note: If you're on MacOS, make sure you've installed Xcode and its developer tools by typing `xcode-select --install`._

_Note: If you have Xcode 10+ installed, you also need to install the package file found at `/Library/Developer/CommandLineTools/Packages/macOS_SDK_headers_for_macOS_10.14.pkg`._

You will need to have Rust installed. You can get it by visiting https://rustup.rs. This'll also install Cargo, Rust's package/project manager.

## MacOS/Linux

Just run:

```bash
curl -L https://git.io/rustlings | bash
# Or if you want it to be installed to a different path:
curl -L https://git.io/rustlings | bash -s mypath/
```

This will install Rustlings and give you access to the `rustlings` command. Run it to get started!



To install Rustlings. Same as on MacOS/Linux, you will have access to the `rustlings` command after it.

## Manually

Basically: Clone the repository, checkout to the latest tag, run `cargo install`.

```bash
git clone https://github.com/rust-lang/rustlings
cd rustlings
git checkout tags/3.0.0 # or whatever the latest version is (find out at https://github.com/rust-lang/rustlings/releases/latest)
cargo install --force --path .
```

If there are installation errors, ensure that your toolchain is up to date. For the latest, run:
```bash
rustup update
```

Then, same as above, run `rustlings` to get started.

## Doing exercises

The exercises are sorted by topic and can be found in the subdirectory `rustlings/exercises/<topic>`. For every topic there is an additional README file with some resources to get you started on the topic. We really recommend that you have a look at them before you start.

The task is simple. Most exercises contain an error that keep it from compiling, and it's up to you to fix it! Some exercises are also run as tests, but rustlings handles them all the same. To run the exercises in the recommended order, execute:

```bash
rustlings watch
```

This will try to verify the completion of every exercise in a predetermined order (what we think is best for newcomers). It will also rerun automatically every time you change a file in the `exercises/` directory. If you want to only run it once, you can use:

```bash
rustlings verify
```

This will do the same as watch, but it'll quit after running.

In case you want to go by your own order, or want to only verify a single exercise, you can run:

```bash
rustlings run myExercise1
```

In case you get stuck, you can run the following command to get a hint for your
exercise:

``` bash
rustlings hint myExercise1
```

## Testing yourself

After every couple of sections, there will be a test that'll test your knowledge on a bunch of sections at once. These tests are found in `exercises/testN.rs`.

