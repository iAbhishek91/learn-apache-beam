# Terminologies associated with beam

## Pipeline

Encapsulate entire data processing task from start to finish(input, process and output data).

Its mandatory to execute a beam pipeline.

Pipeline is a program construct.

## PCollection

It represent a distributed data set that  beam pipeline operates on.

*Its similar to RDD in spark*.

Unlike spark & flint, PCollection works on both bounded and unbounded data stream.

spark: DataFrame for bounded | DStream for unbounded.
flink: DataSet for bounded | DataStream for unbounded.

CHARACTERISTICS:

- **Immutable**: every operation on PCollection creates a new PCollection.
- **Element Type**: all element in a PCollection should be same.
- **Operation Type**: Grain operation is not supported. Cant apply operation on partial or individual element. Its applied to the entire PCollection as a whole.
- **Time stamp**: each element in  a PCollection has an associated timestamp with it. Its very crucial part in beam processing (for implementing watermarking, windowing, and for handling late arrival of data). Time stamp can be assigned in many ways (source can provide, beam can provide, user can provide)

## PTransform

Represent a data processing operation or a step in our pipeline.

We can say: PTransform are applied on one or more PCollection objects and outputs zero, one or multiple PCollection.

Common PTransform object: ParDo, Filter, combine etc
