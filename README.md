# gnu-cross

This is a simple, lightweight project for making cross-compilation toolchain with gnu libc.

## Supported targets

| Target                        | Kernel  | Binutils | GCC    | Glibc |
|-------------------------------|---------|----------|--------|-------|
| aarch64-unknown-linux-gnu     | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| arm-unknown-linux-gnueabi     | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| arm-unknown-linux-gnueabihf   | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| armv7-unknown-linux-gnueabi   | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| armv7-unknown-linux-gnueabihf | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| i586-unknown-linux-gnu        | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| i686-unknown-linux-gnu        | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| loongarch64-unknown-linux-gnu | 5.19.16 | 2.44     | 15.1.0 | 2.41  |
| m68k-unknown-linux-gnu        | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| microblazeel-xilinx-linux-gnu | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| microblaze-xilinx-linux-gnu   | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| mipsel-unknown-linux-gnu      | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| mipsel-unknown-linux-gnusf    | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| mips-unknown-linux-gnu        | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| mips-unknown-linux-gnusf      | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| mips64el-unknown-linux-gnu    | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| mips64-unknown-linux-gnu      | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| powerpc-unknown-linux-gnu     | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| powerpc64-unknown-linux-gnu   | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| riscv32-unknown-linux-gnu     | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| riscv64-unknown-linux-gnu     | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| s390x-ibm-linux-gnu           | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| sh4-multilib-linux-gnu        | 5.4.293 | 2.44     | 15.1.0 | 2.41  |
| x86_64-unknown-linux-gnu      | 5.4.293 | 2.44     | 15.1.0 | 2.41  |

## How to use

Download the tarball from the [release page](https://github.com/cross-tools/gnu-cross/releases) and extract it to `/opt/x-tools`:

```sh
sudo mkdir -p /opt/x-tools
sudo tar -xf ${target}.tar.xz -C /opt/x-tools
```

## How to build

Fork this project and create a new release, or build manually:

```sh
./scripts/make ${target}
```

## License

MIT

## Acknowledgements

We would like to express our gratitude to the following individuals and projects:

- [crosstool-ng](https://github.com/crosstool-ng/crosstool-ng)
- [glibc](https://www.gnu.org/software/libc)
