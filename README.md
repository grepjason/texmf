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
