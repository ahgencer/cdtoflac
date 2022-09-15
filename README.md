<h1 align="center">Automated CD Ripping and Encoding Tool</h1>

<p align="center">
    <img alt="Commit Activity" src="https://img.shields.io/github/commit-activity/m/ahgencer/cdtoflac?label=Commit%20Activity">
    <img alt="GitHub Stars" src="https://img.shields.io/github/stars/ahgencer/cdtoflac?label=GitHub%20Stars">
    <img alt="Issues" src="https://img.shields.io/github/issues/ahgencer/cdtoflac/open?label=Issues">
    <img alt="License" src="https://img.shields.io/github/license/ahgencer/cdtoflac?label=License">
</p>

- GitHub: https://github.com/ahgencer/cdtoflac
- Releases: https://github.com/ahgencer/cdtoflac/tags
- Issues: https://github.com/ahgencer/cdtoflac/issues

*cdtoflac provides a POSIX shell script for ripping music CDs using cdparanoia and losslessly encoding them as FLACs.*

*cdtoflac* is a small wrapper utility around `cdparanoia` and `flac` for digitizing your CD collection. It handles:

- Detection and accurate extraction of all the tracks on a CD.
- Encoding the extracted WAV files as FLACs.
- Managing the owner and group of the outputted track files.

Interested? [Here's how to get started.](#getting-started)

## Getting started

### Installation

*cdtoflac* depends on both the `cdparanoia` and `flac` CLI programs to be installed and available in the `$PATH`.

Otherwise, you can run *cdtoflac* directly after downloading a copy of it.

### Usage

To get help on using *cdtoflac*, run:

    # cdtoflac --help

You may also refer to the manpage [cdtoflac(1)](docs/cdtoflac.1). Additionally, it might be worth reading
through [cdparanoia(1)](https://manpages.org/cdparanoia) and [flac(1)](https://manpages.org/flac).

To rip a CD, place it into a compatible CD-ROM drive and run:

    $ cdtoflac -d <DEVICE> -o <OUTPUT>

where `DEVICE` is the device path to the CD-ROM drive and `OUTPUT` is the directory to output the extracted tracks.

## License

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
details.

You should have received a copy of the GNU Lesser General Public License along with this program. If not,
see <https://www.gnu.org/licenses/>.
