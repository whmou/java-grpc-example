# java-grpc-example

```bash
$ mvn clean instll

# Start the server in a command terminal:
$ mvn exec:java -Dexec.mainClass="com.example.grpc.GrpcServer"

# Start the client in another command terminal:
$ mvn exec:java -Dexec.mainClass="com.example.grpc.GrpcClient"

# output:
Hi Hi, Dirk Nowitzki
```



For the compiling error of the generated code:
"@javax.annotation.Generated"
Fix solution:
```xml
<dependency>
    <groupId>javax.annotation</groupId>
    <artifactId>javax.annotation-api</artifactId>
    <version>1.2</version>
</dependency>
```
reference: 
1) https://stackoverflow.com/questions/60968250/i-use-grpc-to-generate-java-code-javax-annotation-generated-and-it-reports-e
2) https://www.programmersought.com/article/9857789866/
3) https://www.baeldung.com/grpc-introduction
