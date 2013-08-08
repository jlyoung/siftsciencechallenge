# Sift Science Challenge

This is my solution to the challenge question posed by Sift Science.

I wrote a Hadoop Map Reduce job to count the characters and emit the number of occurrences in the 1000 most common words word list.
I later pipe the output through a few unix utilities to get the output format I want.

I include a "FatJar" jar file that also wraps and includes its dependency hadoop-core-0.20.205.0.jar
Sorry for the old Hadoop version...it's what I happend to have on my machine when I wrote this.

## Usage
If you have a Hadoop installation handy (I used Cloudera CDH3), you can execute the MapReduce job from the jar file as follows:

```bash
hadoop jar charactercount.jar /hdfs/input/wordfile/directory /hdfs/results/output/directory
```

Note: The wordfile needs to already exist in HDFS.

Feel free to contact me on Twitter: @josephlyoung