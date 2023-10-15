# Flash Common Torizon to SDCard for x86_64

## Prerequisites

- SDCard Class 10 or better, 8GB or more;
- [Balena Etcher](https://github.com/balena-io/etcher/releases/);
- [intel-corei7-64 pre-built Common Torizon Image](https://github.com/commontorizon/meta-common-torizon/releases/download/v6.3.0-common/torizon-core-common-docker-dev-intel-corei7-64.zip);

## Steps

- Unzip the pre-built Common Torizon Image;
  - This will unzip to a `.wic` file;
- Insert the SDCard into your computer;
- Open Balena Etcher;
- Select the `.wic` file clicking on the `Flash from file` button;
- Select the SDCard clicking on the `Select target` button;
- Click on the `Flash!` button;
