# sure_species
## Introduction
Count the species information annotated in the genome annotation results.
## Fossil Calibration Database
[https://fossilcalibrations.org/Browse.php](https://fossilcalibrations.org/Browse.php)  
[http://www.timetree.org/](http://www.timetree.org/)  
## Installation
<pre><code>
wget -c https://github.com/zxgsy520/fullampl/sure_species/v1.1.0.tar.gz
tar -zxvf v1.1.0.tar.gz
cd v1.1.0
chmod 755 sure_species
sure_species -h
or(windows user)
python sure_species.pyc -h
</code></pre>
or
<pre><code>
git clone https://github.com/zxgsy520/sure_species.git
cd sure_species
chmod 755 sure_species
fullampl -h
or(windows user)
python sure_species.pyc -h
</code></pre>
./sure_species -h
usage: sure_species [-h] [--top INT] input

name:

    sure_species -- Confirm species by annotation results in the database

attention:
    sure_species refseq.tsv > species.tsv
    sure_species refseq.tsv --top 100 > species.tsv

positional arguments:
  input       Input the species annotation file.

optional arguments:
  -h, --help  show this help message and exit
  --top INT   Output top x, default:x=10.
</code></pre>
### Example
<pre><code>
./sure_species refseq.tsv
#Species name   Protein number
Streptomyces    3961
Streptomyces albidoflavus       1876
Streptomyces sp. HK1    50
unclassified Streptomyces       38
Streptomyces albidoflavus group 24
Streptomyces sp. B29(2018)      12
Streptomyces sp. GF20   9
Streptomyces sp. SM8    8
Streptomyces wadayamensis       8
Streptomyces sp. FR-008 8
<pre><code>

