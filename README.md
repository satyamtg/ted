<h1 align="center">ted2zim</h1>

<div align="center">
  <strong>Get the best :bulb: TED videos offline :arrow_down:</strong>
</div>
<div align="center">
  An offliner to create ZIM :package: files from TED talks
</div>

<br />

<div align="center">
  <!-- PyPI version -->
  <a href="https://pypi.org/project/ted2zim/">
    <img alt="PyPI" src="https://img.shields.io/pypi/v/ted2zim?style=for-the-badge">
  </a>
  <!-- Codefactor grade -->
  <a href="https://www.codefactor.io/repository/github/openzim/ted">
    <img alt="CodeFactor Grade"
     src="https://img.shields.io/codefactor/grade/github/openzim/ted/master?label=codefactor&style=for-the-badge">
  </a>
  <!-- License -->
  <a href="https://www.gnu.org/licenses/gpl-3.0">
    <img alt="GitHub" src="https://img.shields.io/github/license/openzim/ted?color=blueviolet&style=for-the-badge">
  </a>
</div>


TED (Technology, Entertainment, Design) is a global set of conferences under the slogan "ideas worth spreading". They address a wide range of topics within the research and practice of science and culture, often through storytelling. The speakers are given a maximum of 18 minutes to present their ideas in the most innovative and engaging ways they can. One can eaisly find all the TED videos [here](https://ted.com/talks).

This project is aimed at creating a sustainable solution to make TED accessible offline by creating ZIM files providing these videos in a similar manner like online.  


## Getting started :rocket:

#### Install the dependencies
Make sure that you have python3, unzip, ffmpeg, wget and curl installed on your system before running the scraper (otherwise you'll get a warning to install them). 

#### Setup the package
One can eaisly install the PyPI version but let's setup the source version. Firstly, clone this repository and install the package as given below.

```
python3 setup.py install
```

That's it. You can now run `ted2zim` from your terminal

```
ted2zim --topics [TOPICS] --name [NAME]
```
For the full list of arguments, see [this](ted2zim/entrypoint.py) file or run the following
```
ted2zim --help
```
Example usage
```
ted2zim --topics="augmented reality" --max-videos-per-topic=10 --debug --name="augumented_reality" --format=mp4 --title="Augmented Reality" --description="TED videos in AR category" --creator="TED" --publisher="openzim" --output="output" --keep --low-quality
```

## License

[GPLv3](https://www.gnu.org/licenses/gpl-3.0) or later, see
[LICENSE](LICENSE) for more details.
