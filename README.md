# medical_imaging
#### DICOM Image text mining

#####DICOM images contain 2 main sections:
######1. Text header : patient, study and other image characteristics
######2. Binary image: the actual image

I wanted to investigate how easy it would be to process a set of DICOM images and store it on a Hadoop cluster with the added benefits:
1. Store text header in a structured manner within Hive metastore as Hive tables.
2. Store original DICOM (.dcm) file on HDFS.
3. Ability to query against the Hive table using in-memory SQL engine like Impala to make valuable insights from the text.
4. Ability to select and view the binary DICOM image right from this interface as required.

This work was an extension of our work using Apache SOLR on a Cloudera Hadoop Distribution to index, store and retrieve DICOM images, founnd here:
