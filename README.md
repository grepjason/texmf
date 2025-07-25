# ~/texmf

My personal, `local`, additions to the `texmf` directory tree.

## Preliminaries

Download and install a TeX distribution (e.g., [TeX Live](https://www.tug.org/texlive/) or [MiKTeX](https://miktex.org/)) on your device.

### Install TeX Live

**macOS:** install MacTeX using [Homebrew](https://brew.sh):

```bash
brew install --cask mactex
```

**Windows:** download and invoke the TeX Live installer [install-tl-windows.exe](http://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe). Or install TeX Live using [Chocolatey](https://chocolatey.org):

```powershell
choco install texlive --params="'/scheme:full'"
```

**Linux:** manual installation:

```bash
wget -O - http://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz |
    tar -xz --strip-components=1 --one-top-level=install-tl-unx &&
    cd install-tl-unx &&
    sudo ./install-tl
```

**Linux:** alternative method — use [install-tl-ubuntu](https://github.com/scottkosty/install-tl-ubuntu/tree/master):

```bash
wget https://github.com/scottkosty/install-tl-ubuntu/raw/master/install-tl-ubuntu &&
     chmod +x ./install-tl-ubuntu
```

This script uses the TeX Live installer to install TeX Live so that LaTeX packages can be updated through CTAN with tlmgr. To do this, the official TeX Live installer is downloaded and used and apt is informed that TeX dependencies are satisfied. Thus, when you want to install a program with apt-get that depends on TeX Live, apt will not try to install the TeX Live packages from the Ubuntu repositories.

### (Optional) Install dependencies for `minted` and `latexindent`

```bash
# Install Pygments for code highlighting with minted in LaTeX
pip3 install Pygments  # for Windows / macOS / Linux
brew install pygments  # for macOS

# Install dependencies for latexindent
cpan -i -T File::HomeDir Log::Log4perl Log::Dispatch::File \
        YAML::Tiny Unicode::GCString
```

## License

Public domain. (Quite obviously this only applies to stuff I've written, i.e., things without an explicit attribution.)

Happy **TeX**ing!
