# **`Test Automation Framework`**

This is a test automation framework designed for from NASA Image and Video Library's Search API endpoint. 
It provides a structured approach for automating tests and streamlining the testing process.

**`Features`**
Search API endpoint from NASA Image and Video Library

## **Getting Started**
**Prerequisites**
`JAVA 20, MAVEN, TestNG, OkHttp3`

**Third party library used**
`OkHttp` is a popular open-source HTTP client library for Java and Android applications. It provides a simple and efficient way to make HTTP requests, handle responses, and interact with web services.

**Key files description**
`pom.xml` has all the dependencies that are being used by this application. Some of the dependencies are - org.apache.logging.log4j, com.squareup.okhttp3, org.json, org.testng, org.slf4j.

**Usage**
`suite.xml` in `src/test/resources` can be run in a TestNG configuration. This suite has the test class.

**Framework Structure**
|--`src/main/java`
 |--`com.NASA`
  |--`Client`
    |--`NASAClient.java` has the OkHttp client and the `sendGetRequest` method and other methods required to fetch data from response
  |--`Utils`
    |--`Constants.java` has all the constants that will be used within this framework
    |--`JSONHelper.java` has all the utility methods to retrieve JSONObject and/or JSON arrays from OkHttp response

|--`src/test/java`
 |--`com.NASA.tests`
  |--`verifyNasaAPISearchTest.java` has all the tests to verify the `/search` endpoint with different params
 |--`resources`
  |--`suite.xml` has the test and class name

**Contact**
Please reach out to Akhila Janapareddy(akhilaj.0831@gmail.com) for questions or queries.
