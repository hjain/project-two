# project-two

Add jetty plugin to pom.xml

Step 1: Add the following to pom.xml
    <plugins>
      <plugin>
        <groupId>org.eclipse.jetty</groupId>
        <artifactId>jetty-maven-plugin</artifactId>
        <version>9.2.11.v20150529</version>
        <configuration>
          <scanIntervalSeconds>10</scanIntervalSeconds>
          <webApp>
            <contextPath>/abc</contextPath>
          </webApp>
          <httpConnector>
            <port>8888</port>
            </httpConnector>
          </configuration>
      </plugin>
    </plugins>

Step 2: mvn package
Step 3: mvn jetty:run
Step 4: http://localhost:8888/abc/
