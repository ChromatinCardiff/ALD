# ALD
Further material for Pass et. al 2017, "Genome-wide chromatin mapping with size resolution reveals a dynamic sub-nucleosomal landscape in Arabidopsis"

BAM2SizePlot.py script used for 2D and 3D figure generation from Paired-End sequence date from MNase digested genomic DNA.

```
BAM2SizePlot.py -h
usage: BAM2SizePlot.py [-h] [-i I] [-d D] [-o O] [-B B] [-b B] [-g G] [-G G]
                       [-e E] [-s S] [-S S] [-q Q] [-r R] [-p P] [-z Z] [-t]

Import Bam file and extract defined region for 2D or 3D plotting

optional arguments:
  -h, --help  show this help message and exit
  -i I        Input a Bam file or a list of comma-separated Bam files to merge
              (format: one.bam,two.bam,three.bam)
  -d D        Optional: Directory where bamfiles are (saves on typing!)
  -o O        Output prefix
  -B B        One individual set of co-ordinates in bed format
              (Chr1:1000-1510)
  -b B        Bed file of regions to extract (Bed file)
  -g G        Gene transcript to get positional information from | REQUIRES
              GTF FILE (-G)
  -G G        gtf file to get gene model information from | REQUIRES
              GENE/TRANSCRIPT ID
  -e E        Integer for upstream/downstream extension
  -s S        Minimum size of particle
  -S S        Maximum size of particle
  -q Q        Integer for rounding counts (fragment size, default: 10)
  -r R        Integer for rounding counts (bases, default: 50)
  -p P        Choose plot type (2D or 3D, default:2D)
  -z Z        Change zmax for plot (Mainly to look at low abundance things)
              (Default 1000, 'None' allows dynamic assignment)
  -t          Use default co-ordinates for testing
```
