# CAASPP Test Results

This dataset is a simple combination of multiple years of California Assessment of Student Performance and Progress
(CAASPP) results, for the years 2015 on. The CAASPP was conducted in 2014, but the 2014 file has a different
structure from other years ( it's a "pp" file, see below) so it is excluded from this package.

## Download Structure

The `Base Download` documentation link points to an FTP-like web directory of files, which contain the downloadable
files. The other download pages have links to the files in these directories. These directories, as well as the
dataset webpages are a bit complex. There seems to be a few different sorts of test result files, but there isn't a
clear distinction between them. These fiels include:

* "Paper Based" results , for 2014 and 2015
* Tests in Spanish, marked "STS" for 2016 and 2017
* Files with code 'pp'. Some 'pp' files have additional codes 'p2' or 'p3'
* Files with 'sb', often also with 'p2' or 'p3'

I think 'sb' means 'Smarter-Balanced'. 

The main page for accessing test results, https://caaspp.cde.ca.gov/, has an inconsistent set of links to result
pages for each year. For some years, the links are to "STS" results, others are to "Paper-Based" and for 2018, the
links are to the "STS" and "Smarter Balanced" results.

## Versions

1. Initial version
2. ``total_tested_with_scores`` datatype changed from 'unknown' to 'integer' with 'robust_int' transform

<!-- start_license -->
## License

The source data, from the California Department of Education, does not
explicitly reference a license, but since the top-level website for California
indicates that data published on the State of California website [is
generally in the public domain](https://www.ca.gov/use/),  we assume it is in
the public domain. Derived data included in this package is also in the public domain. Metadata in this package ( contained in the ``metadata.csv`` file ) is
derived from metadata for the source package, and is also in the public domain. 

Programs used for data transformation (contained in the ``notebooks`` directory), are Copyright 2021 Civic Knowledge, and
are relased under the [Creative Commons Attribution-ShareAlike 4.0 International
License.](https://creativecommons.org/licenses/by-sa/4.0/)

<!-- end_license -->

