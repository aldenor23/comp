Pre-processing BIO bases
1) Installation of BIO databases (datamicroarray) as at https://github.com/ramhiser/datamicroarray
2) Installation of filter genefilter (Bioconductor) at http://bioconductor.org/packages/release/bioc/html/genefilter.html
3) Transformation of matrix dataframe
4) Removal of the control probes according to the descriptive tables of each base
5) Transpose the matrix
6) Uses the filter genefilter in the transposed matrix
7) The resulting matrix goes through transpose and generates the filter matrix
8) Creates a discrete matrix, from the filter matrix where all values ??smaller than the 1st quartile are labeled "b" (low), higher than the 3rd quartile as "a" (high) and the others as "m" ( Medium / normal)
9) The discrete matrix receives the attribute "y" where the majority class is considered "p" (positive) and the other "n" (negative)
10) Transforms the discrete matrix into .CSV

Pre-processing UCI bases
1) Download the UCI databases at http://archive.ics.uci.edu/ml/
2) Insert the attribute "y" where the majority class is considered "p" (positive) and the other "n" (negative)
3) Save to .CSV

Software
1) For APRIORI-SD an SD-Map download and install KEEL tool in http://keel.es/ 
2) For RCS download CAREN tool in http://www4.di.uminho.pt/~pja/class/caren.html

Processing
1) Section 01:
Minimum Confidence: 1.0 , 0.8 , 0.6 , 0.4 , 0.2
Minimum Support: 0.1

2) Section 02:
Minimum Confidence: 0.8
Minimum Support:1.0 , 0.8 , 0.6 , 0.4 , 0.2 , 0.1

