# Python beam program

```py
# REQUIRED STEP: import apache beam and creating a alias called beam
import apache_beam as beam


# REQUIRED STEP: Creating a pipeline and giving it a name, and where to run
p1 = beam.Pipeline()

# final result set is written to final_collection
final_collection(
  p1
    | beam.io.ReadFromText('data.txt') # REQUIRED STEP: input data
    | beam.Map(lambda record: record.split(',')) # REQUIRED STEPS: this can be any transformation, but atleast one is required. Either use it is pipe format or us apply.
    | beam.io.writeToText('data/output') # REQUIRED STEP: write data to source
)

# REQUIRED STEP: run the PCollection
p1.run()
```

Very important: https://beam.apache.org/releases/pydoc/2.25.0/