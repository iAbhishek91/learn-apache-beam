# Architecture of distributed data processing system

>NOTE: here we are not talking about architecture of Hadoop or spark. We will look at architectural components required to create a distributed data processing system.

## Data flow stages and components

1; **Data sources**: twitter, facebook, IoT, satellite etc.

PURPOSE: These systems creates the data and push it to the next layer.

2; **Data collection & preparation layer**:

PURPOSE:

- Collects data from different external sources.
- Transform the data into consistent format.

There are **couple of stages** generally:

- SECURITY LAYER: looks for vulnerability, apply security protocols (like encryption etc).
- STORAGE LAYER: Data to be persisted (may be in-memory or disk). *read about "in-memory distributed cache" used by spark*.
- PROCESSING LAYER: main layer, its for processing and transform the data into information. There are different type based on business use cases: *Machine learning, predictive analysis, decision modelling* etc.
- VISUALIZATION LAYER: processed data is passed on to visualization layer. *Kibana, grafana* are good example of these.
