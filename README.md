## Scala Examples for "Stream Processing with Apache Flink"

This repository hosts Scala code examples for ["Stream Processing with Apache Flink"](http://shop.oreilly.com/product/0636920057321.do) by [Fabian Hueske](https://twitter.com/fhueske) and [Vasia Kalavri](https://twitter.com/vkalavri).

<a href="http://shop.oreilly.com/product/0636920057321.do">
  <img width="240" src="https://covers.oreillystatic.com/images/0636920057321/cat.gif">
</a>

### Starting a local flink cluster

1. Go to the [Flink website](https://flink.apache.org/downloads/) and download the Flink binary for Scala 2.12.
2. Extract the archive file

```shell
tar xvfz flink-1.17.1-bin-scala_2.12.tgz
```

3. Start a local Flink cluster

```shell
cd flink-1.17.1/
./bin/start-cluster.sh
```

4. Open the Flink web UI by entering [http://localhost:8081](http://localhost:8081)
5. Run the example:

```shell
./bin/flink run -c io.github.streamingwithflink.chapter1.AverageSensorReadings examples-scala.jar
```
