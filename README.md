# dkr-intel
This is a Dockerfile with Intel Parallel Studio XE Composer Edition for C++ in a Debian base image. It also includes [tini](https://github.com/krallin/tini/) to protect from software that accidentally creates zombie processes.

### Build
I'm not sharing the pre-build image since it requires a Intel personal license, however you can build your own image.
1. Download your license file from here https://registrationcenter.intel.com/en/products/
2. Rename your license to `license.lic` and put it in the same folder along with the `Dockerfile` and  `config.cfg` files.
3. Build with `docker build -t dkr-intel .`
