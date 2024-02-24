# Nightly Windows builds of SBCL

# How to install
1. Go to the releases page and download the latest ZIP file.
2. Extract it somewhere on your computer.
3. Create an environment variable called `SBCL_HOME` with the value `<path to sbcl directory>/lib/sbcl`.
4. Add a new entry to the `Path` environment variable with the value `<path to sbcl directory>/bin`.

# Running on older Windows versions
These builds of SBCL are linked against the Universal C Runtime (UCRT). This comes included with Windows 10 and later, but might not be present on older Windows versions. If your system does not include UCRT, you should try running Windows Update, as this may install it for you. Otherwise, you can manually download UCRT [here](https://support.microsoft.com/kb/3118401). More information is available at Microsoft Learn: https://learn.microsoft.com/en-us/cpp/windows/universal-crt-deployment.
