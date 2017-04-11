# medical_imaging
#### DICOM Image Text Mining using the Hive Connector for DICOM Image Files

##### DICOM images contain 2 main sections:
###### 1. Text header : patient, study and other image characteristics
###### 2. Binary image: the actual image

I wanted to investigate how easy it would be to process a set of DICOM images and store it on a Hadoop cluster with the following additional benefits:
###### 1. Store text header in a structured manner within Hive metastore as Hive tables.
###### 2. Store original DICOM (.dcm) file on HDFS (thereby bypassing need of a dedicated Image Store).
###### 3. Ability to make distributed queries against the Hive table using in-memory SQL engine like Impala to make valuable insights from the text.
###### 4. Ability to select and view the binary DICOM image right from this interface as required.

This work was an extension of our work using Apache SOLR on a Cloudera Hadoop Distribution to index, store and retrieve DICOM images, found here: https://software.intel.com/sites/default/files/managed/4c/21/Indexing%20DICOM%20Images%20on%20CDH%20v0%201%2000.pdf

The reason for extending the cited work was indexing inside Apache SOLR was a black box and it was difficult to do what-if queries as well as be able to scale over billions of images with the flexibility to be able to correlate with additional data sources and datasets already present in Hive metastore.


All code and other instructions coming here soon ....
