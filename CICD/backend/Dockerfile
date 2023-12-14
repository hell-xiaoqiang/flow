FROM ggcnitabt-prod-cr-registry.cn-hangzhou.cr.aliyuncs.com/product_similarity/aibuying_tool:java
COPY ./similarity.tool-1.0-SNAPSHOT.jar /mnt/
ENTRYPOINT ["/usr/bin/java" , "-Dfile.encoding=utf-8" , "-jar" , "/mnt/similarity.tool-1.0-SNAPSHOT.jar"]
