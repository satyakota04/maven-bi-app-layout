# maven-bi-app-layout

Small Maven project for testing Harness Build Intelligence restore.

`mvn package` compiles `target/classes` and copies those class files to `target/app/classes`. `.mvn/maven-build-cache-config.xml` asks the Maven build cache extension 1.2.0 to save and restore `target/app`.

Run the same `mvn clean install` twice against the cache. The first run compiles and saves. The second run should be a cache hit. After that hit, `target/classes` and `target/app/classes` should both exist.
