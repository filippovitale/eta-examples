# Apache Spark Example

This example demonstrates how you can write an Apache Spark job in Eta.

## Building

To build the program, execute the following in this directory:

`$ epm build`

## Running

- Let `SPARK_HOME` refer to the directory which contains your `Spark` installation.
- Let `EXAMPLE_HOME` refer to the absolute path to this directory.

```
$ cd $SPARK_HOME/bin/spark-submit
                     --class eta.main
                     --master local
                     $EXAMPLE_HOME/dist/build/eta-spark/eta-spark.jar
```

## Limitations
You will get runtime exceptions if you allow Spark to use multiple threads, see 
[this issue](https://github.com/typelead/eta/issues/132). This is a limitation in 
the current RTS that will be lifted relatively soon.

## Contact Us

If you had trouble with this tutorial, you can give us feedback by:

- filing an [issue](https://github.com/typelead/eta-examples/issues/new)

- discussing with us on [Gitter](https://gitter.im/typelead/eta) 