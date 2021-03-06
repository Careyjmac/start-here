1,000 Genomes
=============

This dataset comprises roughly 2,500 genomes from 25 populations around the world.  See the `1,000 Genomes project website <http://www.1000genomes.org/>`_ and publications for full details:

Pilot publication

| `An integrated map of genetic variation from 1,092 human genomes <http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3498066/>`_
| The 1000 Genomes Project Consortiuma
| Published: November 1, 2012
| DOI: 10.1038/nature11632
|

Phase 1 publication

| `A map of human genome variation from population scale sequencing <http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3042601/>`_
| The 1000 Genomes Project Consortium
| Published: October 28, 2010
| DOI:  10.1038/nature09534
|

Phase 3 `announcement <http://www.1000genomes.org/announcements/phase-3-variant-set-additional-allele-frequencies-functional-annotation-and-other-data>`_.

Google Cloud Platform data locations
------------------------------------

* Google Cloud Storage folders
   * These files were loaded into Google Genomics datasets:
      * `gs://genomics-public-data/1000-genomes <https://console.developers.google.com/storage/genomics-public-data/1000-genomes/>`_
      * `gs://genomics-public-data/1000-genomes-phase-3 <https://console.developers.google.com/storage/genomics-public-data/1000-genomes-phase-3/>`_
   * A full mirror of http://ftp-trace.ncbi.nih.gov/1000genomes/ftp/ `gs://genomics-public-data/ftp-trace.ncbi.nih.gov/1000genomes/ftp/ <https://console.developers.google.com/storage/browser/genomics-public-data/ftp-trace.ncbi.nih.gov/1000genomes/ftp/>`_.
* Google Genomics Dataset IDs
   * `10473108253681171589 <https://developers.google.com/apis-explorer/#p/genomics/v1beta2/genomics.datasets.get?datasetId=10473108253681171589>`_ phase 3 reads and phase 1 variants
   * `4252737135923902652 <https://developers.google.com/apis-explorer/#p/genomics/v1beta2/genomics.datasets.get?datasetId=4252737135923902652>`_ phase 3 variants
* Google BigQuery Dataset IDs
   * `genomics-public-data:1000_genomes <https://bigquery.cloud.google.com/table/genomics-public-data:1000_genomes.variants>`_ phase 1 variants and sample information
   * `genomics-public-data:1000_genomes_phase_3 <https://bigquery.cloud.google.com/table/genomics-public-data:1000_genomes_phase_3.variants>`_ phase 3 variants

Beacon
------

You can find a `Global Alliance for Genomics and Health Beacon`_ at http://webdev.dnastack.com/p/beacon/thousandgenomes?chromosome=1&coordinate=10177&allele=AC

Provenance
----------

The source files for this dataset include:
 * The mapped full-genome phase 3 BAM files listed at `the 1000 Genomes FTP site <ftp://ftp.1000genomes.ebi.ac.uk/vol1/ftp/alignment_indices/20130502.low_coverage.alignment.index>`_.
  * All of the phase 1 VCF files listed at `the 1000 Genomes FTP site <ftp://ftp.1000genomes.ebi.ac.uk/vol1/ftp/phase1/analysis_results/integrated_call_sets/>`_.
  * All of the phase 3 VCF files listed at `the 1000 Genomes FTP site <ftp://ftp.1000genomes.ebi.ac.uk/vol1/ftp/release/20130502>`_.
* These files were copied to Google Cloud Storage, uploaded to Google Genomics, and the variants were exported to Google BigQuery.
