# Beam API

> API Names are only mentioned, detail about the method can be found on docs.

https://beam.apache.org/releases/pydoc/2.25.0/

## Input

- Create()
- ReadFromText()
- ReadFromAvro() # data def in JSON and the data in binary - IBM
- ReadFromParquet() # open sourcefile format for any project on hadoop
- ReadFromTFRecord() # tensor flow data
- ReadFromPubSub() # topic, subscription provide any one,(both are not allowed)

## Output

- WriteToText()
