# maven-bi-app-layout

Small Maven project for testing Harness Build Intelligence restore.

`mvn package` compiles `target/classes` and copies those class files to `target/app/classes`. Build Intelligence writes `.mvn` at runtime.

Run the same `mvn clean install` twice against the cache. The first run compiles and saves. The second run should be a cache hit.
