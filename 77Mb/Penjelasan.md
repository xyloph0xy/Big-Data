1. git clone https://github.com/xyloph0xy/Big-Data
2. cd Big-Data/77Mb
3. sudo docker container ls, output : ![container](https://github.com/xyloph0xy/Big-Data/assets/92715425/95a6bdd9-86ba-400c-8d77-91f3a4a586d9)
4. sudo docker cp D77mb.txt b56fe19ec6d0:gabung.txt
5. sudo docker exec -it namenode bash
6. hadoop fs -rm input/*
7. hadoop fs -ls input/
8. hadoop fs -put gabung.txt input
9. hadoop jar hadoop-mapreduce-examples-2.7.1-sources.jar org.apache.hadoop.examples.WordCount input output77
10. hadoop fs -ls output77/, output: ![map reduce](https://github.com/xyloph0xy/Big-Data/assets/92715425/e2f02516-0a4c-4041-b699-48d44e6616da)
11. hadoop fs -cat output77/part-r-00000, hasil : 
