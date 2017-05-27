# POC for Apache Nutch 2.3 with Cassandra on Docker

Make sure you have docker installed on your system.

### Build the images
```
./bin/build.sh
```

### Start all containers
```
./bin/start.sh
```

### Stop all containers
```
./bin/stop.sh
```


### Sample Crawling


Run the command:
```
docker exec NUTCH01 /opt/nutch/bin/crawl /opt/nutch/testUrls test_crawl 3
```
or

```
docker exec -it  NUTCH01 /bin/bash
root@9ec43c388769:/# cd opt/nutch
root@9ec43c388769:/opt/nutch# ./bin/crawl
Usage: crawl <seedDir> <crawlID> [<solrUrl>] <numberOfRounds>
root@9ec43c388769:/opt/nutch# ./bin/crawl testUrls test_crawl 3

```

### NOTES:

Nutch 2.3 Container name : NUTCH01

Cassandra Container name : CASS01
