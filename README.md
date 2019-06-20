# Java classes from wsdl

This is an illustration how to use Apache CXF tool that generates Java classes (SOAP-based client/server and corresponding message files)
from an existing service.

In this example, we used service [GetCityWeatherByZIP](http://wsf.cdyne.com/WeatherWS/Weather.asmx?WSDL) that provides a weather information for a given US city by its zip code.

First we need to save the content of the wsdl file from the service:

```
src/main/resources
```


Run the maven plugin by typing:

```
mvn generate-source
```

Then, in folder

```
target/cxf-codegen-plugin-markers
```

you'll find all the files.

For more details, see the plugin's official [web page](https://cxf.apache.org/docs/maven-cxf-codegen-plugin-wsdl-to-java.html).