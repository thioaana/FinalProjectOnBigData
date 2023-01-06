# Final Project on Big Data COMP-548
Contains a short desription of the Final Assessement Project of the course Big Data COMP548 and also the submission code in Python.

## Dataset
In the context of the project a semi structure dataset named OpeStreetMap is used.<br>
Open Steet Map is an Open Source common provider for maps. Their raw datastructure is composed of Nodes, Ways and Relations.

## Methodology
The total world dataset is 98 GB. Part of it contains data for Greece (650 MB) downloaded locally.<br>
The code is written in PySpark on Jupyter Notebook.<br>
When the testing succedeed locally it is uploaded on a Dataproc cluster on Google Cloud, and tested successfully there too.

## Details
<ol>
<li>The raw data are in a PBF format.<br>
In order to be used with Spark it is transformed into parquet format using an [osm parquetizer](https://github.com/adrianulbona/osm-parquetizer)</li>
<li>The data cleaned and transformed (ie from Binary to String types) so to be used properly as  PySpark Dataframes</li>
<li>The schemas and the content is verified.</li>
<li>Two queries applied on different files (Nodes and Ways) and the relevant graphs are plotted.</li>
</ol>
