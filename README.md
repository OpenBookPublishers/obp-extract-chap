# obp-extract-chap
Wrapper to split PDF books by the chapter.

## How to run this tool
### Setup
This wrapper requires `pip3, pyvenv-3.5, pdftk and exiftool` to be installed on your system. On Debian (or Debian-based distributions) this package can be installed via

`apt-get install pip3 pyvenv-3.5 pdftk exiftool`

To perform the setup, run:

`bash setup`

The setup contains the necessary instruction to initialise the submodule.

### Run
To run the process, place a copy of the **PDF edition of the book** and a json file (as shown in the `example.json` file) in the _obp-extract-chap_ folder. Finally, run:

`bash run prefix`

where _prefix_ is the name of the book and the DOI deposit files; i.e.: `bash run Screpanti-Labour-Value`.

### Clean-up

`bash clean [-y]`

would remove temporary files (untracked files and folders stored in the _obp-extract-chap_ folder). The script asks for the user's confirmation before removing the files, but if you are running this as part of a script you might want to use the`-y` flag to bypass the confirmation.