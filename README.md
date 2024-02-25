# Nightly Windows builds of SBCL

[![Build and release](https://github.com/olnw/sbcl-builds/actions/workflows/workflow.yml/badge.svg)](https://github.com/olnw/sbcl-builds/actions/workflows/workflow.yml)

The official Windows build of SBCL tends to be a bit outdated. I created this repository for those who need or prefer to use a newer version. Builds are done daily at 01:15 UTC.

N.B. These are not official SBCL builds. Official releases can be obtained from https://www.sbcl.org/platform-table.html.

## Installation
Download and run the [latest MSI installer](https://github.com/olnw/sbcl-builds/releases/latest). That's it!

## Manual installation
1. Download and extract the ZIP file from the [latest release](https://github.com/olnw/sbcl-builds/releases/latest). It should have a name like `sbcl-ucrt64-<some numbers and letters>.zip`.
2. Create an environment variable called `SBCL_HOME` with the value `<path to sbcl directory>/lib/sbcl`.
3. Add a new entry to the `Path` environment variable with the value `<path to sbcl directory>/bin`.

## Running on older Windows versions
These builds of SBCL are linked against the Universal C Runtime (UCRT). This comes included with Windows 10 and later, but might not be present on older Windows versions. If your system does not include UCRT, you should try running Windows Update, as this may install it for you. Otherwise, you can manually download UCRT [here](https://support.microsoft.com/kb/3118401). More information is available at Microsoft Learn: https://learn.microsoft.com/en-us/cpp/windows/universal-crt-deployment.
