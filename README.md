# A Simple Spark Scala WordCount on MAC

Brew install Hadoop on mac - https://dtflaneur.wordpress.com/2015/10/02/installing-hadoop-on-mac-osx-el-capitan

Install spark and scala on mac - https://medium.freecodecamp.org/installing-scala-and-apache-spark-on-mac-os-837ae57d283f

Integration of github and Eclipse - https://www.youtube.com/watch?v=LPT7v69guVY 

How to create a spark project on local Machine - https://www.youtube.com/watch?v=aB4-RD_MMf0&list=FL6WnnU6XBhpE0jGcaUFW7yw

Build the jar from SCALA - mvn package

spark-submit --class org.test.WordCount \
--master local --deploy-mode client --executor-memory 1g \
--name wordcount --conf "spark.app.id=wordcount" \
target/spark-0.0.1-SNAPSHOT-jar-with-dependencies.jar hdfs://localhost:9000/tmp/food.txt hdfs://localhost:9000/tmp/foodcounts 2

