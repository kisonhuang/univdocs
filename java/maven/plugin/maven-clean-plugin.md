# maven-clean-plugin

maven-clean-plugin用于删除构建时生成的文件。

## 目标

### clean:clean



```
<excludeDefaultDirectories> boolean 
<failOnError>               boolean
<fast>                      boolean
<fastDir>                   File
<fastMode>                  String
<filesets>                  Fileset[]
<followSymLinks>            boolean
<retryOnError>              boolean
<skip>                      boolean
<verbose>                   boolean
```







project.build.directory
project.build.outputDirectory
project.build.testOutputDirectory
project.reporting.outputDirectory













```xml
<plugin>
    <artifactId>maven-clean-plugin</artifactId>
    <version>3.2.0</version>
    <configuration>
        <skip>true</skip>
    </configuration>
</plugin>
```



```xml
<plugin>
    <groupId>org.apache.maven.plugins</groupId>
    <artifactId>maven-clean-plugin</artifactId>
    <version>3.2.0</version>
    <configuration>
        <failOnError>false</failOnError>
    </configuration>
</plugin>
```


```xml
<plugin>
    <artifactId>maven-clean-plugin</artifactId>
    <version>3.2.0</version>
    <configuration>
        <filesets>
            <fileset>
                <directory>some/relative/path</directory>
                <includes>
                    <include>**/*.tmp</include>
                    <include>**/*.log</include>
                </includes>
                <excludes>
                    <exclude>**/important.log</exclude>
                    <exclude>**/another-important.log</exclude>
                </excludes>
                <followSymlinks>false</followSymlinks>
            </fileset>
        </filesets>
    </configuration>
</plugin>
```









## 参考文档

+ https://maven.apache.org/plugins/maven-clean-plugin
+ https://maven.apache.org/plugins/maven-clean-plugin/clean-mojo.html
+ https://maven.apache.org/plugins/maven-clean-plugin/usage.html
+ https://maven.apache.org/plugins/maven-clean-plugin/faq.html
+ https://maven.apache.org/plugins/maven-clean-plugin/examples/delete_additional_files.html
+ https://maven.apache.org/plugins/maven-clean-plugin/examples/ignoring-errors.html
+ https://maven.apache.org/plugins/maven-clean-plugin/examples/skipping-clean.html




