# Demo for fastText
This repository contains a demo for text representation using fastText. A walkthrough for text representation is givin in the included notebook. The data needs to be downloaded and preprocessed.

### Downloading the data:
We need to download the first 1 billion bytes of English Wikipedia. They can be found on Matt Mahoney's [website](http://mattmahoney.net/).
`$ mkdir data`
`$ wget -c http://mattmahoney.net/dc/enwik9.zip -P data`
`$ unzip data/enwik9.zip -d data`

### Preprocessing the data:
A raw Wikipedia dump contains a lot of HTML / XML data. We pre-process it with the wikifil.pl script bundled with fastText (this script was originally developed by Matt Mahoney, and can be found on his [website](http://mattmahoney.net/)).
`$ perl wikifil.pl data/enwik9 > data/fil9`

### Checking the data:
We can check the file by running the following command
`$ head -c 80 data/fil9`
`anarchism originated as a term of abuse first used against early working class`

### Video Link:
