1. In etc/hadoop/hadoop-env.sh 
    export JAVA_HOME = /root to Java/ (excluding jre)
    
2. Following Environment variables:
    export JAVA_HOME = /root to Java/ (excluding jre)
    export PATH=${JAVA_HOME}/bin:${PATH}
    export HADOOP_CLASSPATH=${JAVA_HOME}/lib/tools.jar
    
3. bin/hadoop com.sun.tools.javac.Main WordCount.java
   jar cf wc.jar WordCount*.class
   
4. bin/hadoop jar wc.jar WordCount wordcount/input wordcount/output

5. bin/hadoop fs -cat wordcount/output/part-r-00000
