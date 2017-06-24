<h1>Sparkjava example</h1>

<h3>Add dependency in pom file</h3>

```xml
<dependencies>
        <dependency>
            <groupId>com.sparkjava</groupId>
            <artifactId>spark-core</artifactId>
            <version>2.5.5</version>
        </dependency>
        <dependency>
            <groupId>org.slf4j</groupId>
            <artifactId>slf4j-simple</artifactId>
            <version>1.7.21</version>
        </dependency>
</dependencies>
```

<h3>In your java file</h3>

```java
//Set the port
port(7676);

//Methods in the path will be executed when the call contains the path
path("/data", () ->{

});

//It will executed before the method
before("/*",(request, response) -> {

});
  
//Get method
get("/getAllCars",(((request, response) -> /*your message*/)));
  
//It will executed after the method(post, get, put)
after("/*",((request, response) -> {
  //your code  
}));

post("/add", ((request, response) -> {
  //your code         
});
```


        
