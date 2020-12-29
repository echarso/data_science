# Apache Hudi
https://hudi.apache.org/docs/concepts.html#copy-on-write-table


update - delete records ( how do i change recordss in a table)

change streams ( how do i fetch changged records )

Copy on write :

Stores data using exclusively columnar file formats (e.g parquet).
Updates simply version & rewrite the files by performing a 
synchronous merge during write

Merge On Read :

Stores data using a combination of columnar 
(e.g parquet) + row based (e.g avro) file formats. 
Updates are logged to delta files & later compacted
to produce new versions of columnar files synchronously
or asynchronously.

Query types
Hudi supports the following query types

Snapshot Queries : 
Queries see the latest snapshot of the table as of a given commit or compaction action. 
In case of merge on read table, it exposes near-real time data(few mins) by merging the base and delta files 
of the latest file slice on-the-fly.

For copy on write table, it provides a drop-in replacement for existing parquet tables, 
while providing upsert/delete and other write side features.


Incremental Queries :
Queries only see new data written to the table, since a given commit/compaction. 
This effectively provides change streams to enable incremental data pipelines.

Read Optimized Queries : 
Queries see the latest snapshot of table as of a given commit/compaction action. 
Exposes only the base/columnar files in latest file slices and guarantees the same columnar query performance compared to a non-hudi columnar table.
