### Durable Function
Pretty much same as Function only difference is, it will run for longer period time than azure's default time out (something like 30min)
and it shows where you can see the result of call.

* see the Function example [here](https://github.com/allthatjava/azure-function-example-in-java)

* Need to add local.settings.json file after download the code
![img/local.settings.json.png](img/local.settings.json.png)
Then need to update the Storage connection string as yours

* After the durable function call, you will get the path where you can see the progress and result
![img/status-get.png](img/status-get.png)

### Update
* updated following dependency with latest version(1.5.0) but, it still has a vulnerability... What can you do ¯\\(ツ)_/¯
```properties
        <dependency>
            <groupId>com.microsoft</groupId>
            <artifactId>durabletask-azure-functions</artifactId>
            <version>${durabletask.azure.functions}</version>
        </dependency>
```