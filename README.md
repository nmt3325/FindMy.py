<div align="center">
  <img alt="FindMy.py Logo" src="https://raw.githubusercontent.com/malmeloo/FindMy.py/refs/heads/main/assets/icon.png" width="500">
  <h1>FindMy.py</h1>
</div>

<div align="center">

_Query Apple's FindMy network with Python!_

  <h5>
      <a href="https://docs.mikealmel.ooo/FindMy.py">
        Docs
      </a>
      <span> | </span>
      <a href="examples/">
        Examples
      </a>
      <span> | </span>
      <a href="https://pypi.org/project/FindMy/">
        PyPI
      </a>
      <span> | </span>
      <a href="https://discord.gg/EF6UCG2TF6">
        Discord
      </a>
</div>
[![DeepWiki](https://img.shields.io/badge/DeepWiki-nmt3325%2FFindMy.py-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAyCAYAAAAnWDnqAAAAAXNSR0IArs4c6QAAA05JREFUaEPtmUtyEzEQhtWTQyQLHNak2AB7ZnyXZMEjXMGeK/AIi+QuHrMnbChYY7MIh8g01fJoopFb0uhhEqqcbWTp06/uv1saEDv4O3n3dV60RfP947Mm9/SQc0ICFQgzfc4CYZoTPAswgSJCCUJUnAAoRHOAUOcATwbmVLWdGoH//PB8mnKqScAhsD0kYP3j/Yt5LPQe2KvcXmGvRHcDnpxfL2zOYJ1mFwrryWTz0advv1Ut4CJgf5uhDuDj5eUcAUoahrdY/56ebRWeraTjMt/00Sh3UDtjgHtQNHwcRGOC98BJEAEymycmYcWwOprTgcB6VZ5JK5TAJ+fXGLBm3FDAmn6oPPjR4rKCAoJCal2eAiQp2x0vxTPB3ALO2CRkwmDy5WohzBDwSEFKRwPbknEggCPB/imwrycgxX2NzoMCHhPkDwqYMr9tRcP5qNrMZHkVnOjRMWwLCcr8ohBVb1OMjxLwGCvjTikrsBOiA6fNyCrm8V1rP93iVPpwaE+gO0SsWmPiXB+jikdf6SizrT5qKasx5j8ABbHpFTx+vFXp9EnYQmLx02h1QTTrl6eDqxLnGjporxl3NL3agEvXdT0WmEost648sQOYAeJS9Q7bfUVoMGnjo4AZdUMQku50McDcMWcBPvr0SzbTAFDfvJqwLzgxwATnCgnp4wDl6Aa+Ax283gghmj+vj7feE2KBBRMW3FzOpLOADl0Isb5587h/U4gGvkt5v60Z1VLG8BhYjbzRwyQZemwAd6cCR5/XFWLYZRIMpX39AR0tjaGGiGzLVyhse5C9RKC6ai42ppWPKiBagOvaYk8lO7DajerabOZP46Lby5wKjw1HCRx7p9sVMOWGzb/vA1hwiWc6jm3MvQDTogQkiqIhJV0nBQBTU+3okKCFDy9WwferkHjtxib7t3xIUQtHxnIwtx4mpg26/HfwVNVDb4oI9RHmx5WGelRVlrtiw43zboCLaxv46AZeB3IlTkwouebTr1y2NjSpHz68WNFjHvupy3q8TFn3Hos2IAk4Ju5dCo8B3wP7VPr/FGaKiG+T+v+TQqIrOqMTL1VdWV1DdmcbO8KXBz6esmYWYKPwDL5b5FA1a0hwapHiom0r/cKaoqr+27/XcrS5UwSMbQAAAABJRU5ErkJggg==)](https://deepwiki.com/nmt3325/FindMy.py)
## 🚀 Overview

The current "Find My-scene" is quite fragmented, with code
being all over the place across multiple repositories,
written by [several authors](#-credits). This makes it hard to
integrate FindMy functionality with your project. FindMy.py
aims to make it easy for you to query the location of your
AirTags, iDevices and DIY tags with an easy to use Python library.

## 🧪 Features

- [x] Cross-platform: no Mac needed
- [x] Fetch and decrypt location reports
  - [x] Official accessories (AirTags, iDevices, etc.)
  - [x] Custom AirTags (OpenHaystack)
- [x] Apple account sign-in
  - [x] SMS 2FA support
  - [x] Trusted Device 2FA support
- [x] Scan for nearby FindMy-devices
  - [x] Decode their info, such as public keys and status bytes
- [x] Import or create your own accessory keys
- [x] Both async and sync APIs

## 📥 Installation

The package can be installed from [PyPi](https://pypi.org/project/findmy/):

```shell
pip install findmy
```

For usage examples, see the [examples](examples) directory.
We are also building out a CLI. Try `python -m findmy` to see the current state of it.
Documentation can be found [here](http://docs.mikealmel.ooo/FindMy.py/).

## 🤝 Contributing

Want to contribute code? That's great! For new features, please open an
[issue](https://github.com/malmeloo/FindMy.py/issues) first so we can discuss.

This project uses [Ruff](https://docs.astral.sh/ruff/) for linting and formatting.
Before opening a pull request, please ensure that your code adheres to these rules.
There are pre-commit hooks included to help you with this, which you can set up as follows:

```shell
pip install uv
uv sync  # this installs ruff & pre-commit into your environment
pre-commit install
```

After following the above steps, your code will be linted and formatted automatically
before committing it.

## 🧠 Derivative projects

There are several other cool projects in the FindMy space!
You can check them out [here](http://docs.mikealmel.ooo/FindMy.py/related/index.html).

## 🏅 Credits

While I designed the library, the vast majority of actual functionality
is made possible by the following wonderful people and organizations:

- @seemo-lab for [OpenHaystack](https://github.com/seemoo-lab/openhaystack/)
  and their [research](https://doi.org/10.2478/popets-2021-0045);
- @JJTech0130 for [Pypush](https://github.com/JJTech0130/pypush), providing the breakthrough necessary
  for getting this to work without a Mac;
- @biemster for [FindMy](https://github.com/biemster/FindMy), which is the main basis of this project;
- @Dadoum for [pyprovision](https://github.com/Dadoum/pyprovision/) and
  [anisette-v3-server](https://github.com/Dadoum/anisette-v3-server);
- @nythepegasus for [GrandSlam](https://github.com/nythepegasus/grandslam/) SMS 2FA;
- And probably more, so let me know! :D
