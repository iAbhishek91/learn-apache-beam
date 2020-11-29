# About Beam

## Why beam was created

Most of the distributed system have separate API for batch & stream processing.

Apache beam provides common API for both.

VISION of apache beam, is to look at data as it is not as batch or stream.

## Two main feature

- UNIFIED PROGRAMMING MODEL: common API for stream and batch.
- PORTABLE  big data processing pipeline. Means beam code can be executed over any framework like Flint, Spark, Apex and Cloud dataflow or many more.

## Beam Architecture

> Ref: 0x-beam-architecture.png

It **provide SDK in multiple languages**. Currently supports JAVA and PYTHON. With help of SDK we can create beam pipelines.

Internally beam comes with **runner workers** to make sense of the pipelines, hence each language have its own language specific APIs.

**Fn API** are used by workers to communicate with the runners.

It can **run on multiple runner** of your choice. Currently supports: Spark, Flint, Cloud dataflow and few more. **Runner** sits in between beam API and fn API. Refer 0x-beam-architecture-3.png

> Apache beam is extended on AWS using AWS kinesis (https://www.youtube.com/watch?v=eCgZRJqdt_I)
